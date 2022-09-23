<h1>Contents</h1>

- [수업 내용](#수업-내용)
  - [외부 참조](#외부-참조)
  - [참조](#참조)
- [*Matlab*의 배열](#matlab의-배열)
- [*Matlab*에서 배열 선언하기](#matlab에서-배열-선언하기)
- [특수한 배열 만들기](#특수한-배열-만들기)
  - [단위 행렬 (idnetity matrix)](#단위-행렬-idnetity-matrix)
- [배열 원소 다루기](#배열-원소-다루기)
- [배열 입력하기](#배열-입력하기)
- [연산자](#연산자)
  - [전치 연산자 (`'`)](#전치-연산자-)

## 수업 내용

지난 수업에 이어서 *배열 만들기*를 진행합니다.

### 외부 참조

- [Portland State University, Matlab 정리](http://web.cecs.pdx.edu/~gerry/MATLAB/masterOutline.html)
- [홍익대학교 _Matlab_ 정리](https://huniv.hongik.ac.kr/~shittc/matlab.htm)
- [Mathworks 공식 API 문서](https://kr.mathworks.com/help/thingspeak/channels-and-charts-api.html)

### 참조

- [Matlab Onramp Tutorial](https://matlabacademy.mathworks.com/kr/details/matlab-onramp/gettingstarted?s_tid=course_mlor_start1) <br>
  *Matlab*의 문법을 설명하는 *Matlab*의 공식 인강입니다.,

## *Matlab*의 배열

- 문자, 기호 자료 등의 수치 정보를 순서에 따라 무리 지어 표시하는 자료형
- 하나의 행과 열로 구성된 벡터를 각각 `행 벡터`, `열 벡터`라고 부름.
- 2차원 배열을 `행렬 (matrix)`라고 하고, 배열과 교환하여 사용함.
- *Matlab*에서 정의하는 배열은 수학적 정의와 거의 동일하게 사용됨.
  - 선형대수에서는 배열 연산이 항목별로 이루어지는 것을 허용하지 않지만, *Matlab*에서는 배열 연산자를 통해 항목별로 계산하는 것이 가능함.

## *Matlab*에서 배열 선언하기

```matlab
x=[1 2;3 4];
```

```matlab
y=[1,2;3,4];
```

위의 2가지 방법 중 하나를 사용해 아래와 같은 배열을 만들 수 있음.

$$
x=\begin{pmatrix}
  1,  2 \\
  3,  4
\end{pmatrix}
$$

## 특수한 배열 만들기

### 단위 행렬 (idnetity matrix)

```matlab
eye(m, n)
```

> 누락 부분 있음!

## 배열 원소 다루기

_콤마(,)_ 사용

- 배열의 동일한 행에 포함되는 원소를 분리하는데 사용됨.
- 배열의 색인을 형성하는 것에 사용됨.

> 누락 부분 있음!

## 배열 입력하기

- *콜론(:)*의 사용
  - 주어진 배열에 대한 각 원소, 행, 열 및 부분 배열을 다양한 방법으로 표시하는데 사용됨.
  - 콜론은 전체 행 혹은 열에 대해 와일드 카드의 역할을 함.
    - v(:)은 벡터 v의 모든 행과 열의 원소를 표기함.
    - v(2:5)는 벡터 v의 두 번째부터 다섯 번째 원소인 v(2), v(3), v(4), v(5)의 값을 모두 가져옴.

## 연산자

### 전치 연산자 (`'`)

- 생성된 *Matlab*의 변수의 행과 열을 교환함.
- 생성된 변수에 아포스트로피를 하여 사용.
