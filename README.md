# Data-Analysis

## Numpy
1. Numerical Python의 줄임말
- 행렬 연산이나 대규모 다차원 배열을 편리하게 처리할 수 있도록 지원하는 파이썬 라이브러리
- 데이터 구조 뿐 아니라 고성능의 수치 계산 함수를 제공
2. 특징
- N차원 배열 객체
- 기본적으로 array단위로 데이터 관리
- 큰 규모의 데이터 연산을 빠르게 수행(반복문 없이 배열에 대한 처리 지원)
- 정교한 브로드캐스팅(Broadcast)기능

3. `Scalar` vs `Vector` vs `Matrix`
- `Scalar` 는 숫자
- `Vector` 는 숫자들의 list(1D array, row or column)
- `Matrix` 는 숫자들의 2D array(rows, columns)

4. `ndarray` vs `list`
- `ndarray`
  - 메모리량이 상대적으로 작다
  - 서로 다른 타입의 데이터를 담을 수 없다!
  - 내부 반복문을 사용해서 속도가 빠르다
  - 배열 간에 산술 연산이 가능하다
- `list`
  - 사용되는 메모리량이 많다
  - 서로 다른 타입의 데이터를 담을 수 있다
  
5. Ndarray(다차원 array)
- Numpy는 다차원 배열을 지원하고 배열의 구조는 'shape'으로 표현
- 다차원 배열은 입체적인 데이터 구조를 가진다
- 데이터 방향은 axis로 표현한다
  - 행 방향 : axis = 0
  - 열 방향 : axis = 1
  - 채널 방향 : axis = 2
  
6. 브로드캐스팅
- 크기가 다른 배열 간의 연산 함수를 적용하는 규칙 집합
  - `m x n` 행렬과 `m x 1` 벡터 간의 연산
  - `m x n` 행렬과 `1 x n` 벡터 간의 연산
  - `m x 1` 벡터와 `1 x n`

### 자료형
1. python
- int,float, complex, string, bool, list, tuple, dict, set
2. numpy
단일 값을 메모리에 저장하는데 필요한 bit수를 의미합니다.
- int(8bit, 16bit, 32bit, 64bit) i1, i2, i4, i8
  - 부호가 있음
  - 비트수 만큼 크기를 가지는 정수형
- unit(8bit, 16bit, 32bit, 64bit) u1, u2, u4, u8
  - 부호가 없음
  - 비트수 만큼 크기를 가지는 정수형
- float(16bit, 32bit, 64bit, 128bit) f2, f4, f8, f16
  - 부호가 있음
  - 비트수 만큼 크기를 가지는 실수형
- 복소수형
  - complex64 : 두개의 32비트 부동 소수점으로 표시되는 복소수 c8
  - complex128 : 두개의 64비트 부동소수점으로 표시되는 복소수 c16
- unicode
  - 고정 길이 문자열 unicode
  - bool
  - True, False