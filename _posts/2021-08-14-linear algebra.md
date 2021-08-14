# 선형대수(2주)

Tags: August 9, 2021
강사: 이병근

# Ⅰ. 선형대수 기초와 선형 시스템

[https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)

## 1. Elements in Linear Algebra: Vector와 Matrix 기본 개념 및 성질

### 1) Scalar, Vector, and Matrix

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled.png)

- R은 실수의 전체의 집합
- 벡터의 차원은 row의 개수와 R의 거듭제곱으로 표현

      - 1 차원의 행렬 꼴로 표현

- row(horizontal vector,

    column(vertical) vector = default

→ scalar : a /    vector : **a**   /    Matrix : A 

[과기대 김성훈 교수 추가]

scalar 0차원

vector 1차원

Matrix 2차원(3 x 2 행렬은 수평벡터 3개와 수직 벡터 2개로 이루어져있다)

n  - tensor(3차원 이상)

Shape - 각 element가 몇개로 이루어져 있는지

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%201.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%201.png)

- default인 column vector를 transpose하여 row vector로 만든다

### 2)  Vector, Matrix additions/  multiplication

 (1) element-wise addition

 (2) Scalar multiple of vector/matrix (상수배)

 (3) Matrix-matrix multiplication

    - 벡터끼리 곱할 때 수직 벡터가 앞에 있으면 결과 행렬 값이 커지고, 수직평벡터가 앞에 있으면 1x1 행렬로 나옴

[https://ghebook.blogspot.com/2010/07/vector.html](https://ghebook.blogspot.com/2010/07/vector.html)

벡터의 성질을 기하학적으로, 좌표상으로 이해하는게 기본이다.

- 벡터의 노름(norm) : 크기와 길이
- 벡터의 덧셈 : 두 벡터가 만드는 평행사변형의 대각선 화살표가 가르키는 꼭지점 (좌표상 x,y를 각각 더한 것)
- 벡터의 뺄셈: 두벡터 화살표 꼭지점 간의 거리(좌표상 x,y를 각각 뺀 것) ∥u-v∥
- 벡터의 상수배: 화살표 길이 두배 늘리기 cv
- 벡터의 곱

    (1) 내적(inner product, dot product) : ∥u∥∥v∥cos𝜽 → 특히 90도(직교)일 때 0

    (2) 외적(outer product) : 평행사변형의 넓이 x 벡터 방향

### 3) Properties of Matrix operations  ****

**v Matrix multiplication - NOT coummtative**

  **(교환법칙 성립 x)**

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%202.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%202.png)

분배법칙, 결합법칙 성립

Transpose 할 때는 순서가 뒤바뀐다는 점 유의

## 2. Linear System: 여러 개의 linear equation을 Matrix로 계산하기

### 1) Linear Equation(선형방정식)

- 차수가 1이어야 함(x+2y+3xy도 안됨)
- **Transpose a랑 x의 위치를 바꿔도 식이 나옴**

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%203.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%203.png)

### 2) Linear System: Set of Equations

(1) 정의

- A system of linear equations -> 같은 변수들을 가진 여러 선형연립방정식이 세트를 이루고 있는 것
- SIngle Matrix Equation으로 바꿔서 풀기

(2) 계산을 위해 알아야 하는 행렬

Identity Matrix(항등행렬) : I*X하면 그대로 출력, 대각선에만 1, 나머지는 0

Inverse Matrix(역행렬): square matrix(정사각 행렬)의 연산에서, 앞이나 뒤에서 곱했을 때 항등행렬이 나오게 하는 행렬

(commutative)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%204.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%204.png)

(3) 풀이

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%205.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%205.png)

### 3) Non-Invertible Matrix A for Ax = b

- 위의 풀이법은 역행렬이 존재할 때만 가능
- 역행렬이 존재하지 않는 경우 - determinant(판별식): ad-bc = 0

    → 3 x 3 행렬이면 abc def ghi가 있으면 (aei+ bfg +cdh) -( ceg + afh +  bdi)

    (대각이선랑 삼각형) 

    → 실제로 이걸 사용하진 않고 다른 알고리즘 이용

- 해가 아예 없거나 무수히 많거나 : 두 식의 직선이 평행하거나 겹치거나

### 4) Rectangular Matrix(직사각행렬 Ax = b)

- 역행렬 연산으로 해를 구하는 것은 정사각행렬을 전제함
- row의 개수 = 샘플 수(계수) / column의 개수 = 변수의 개수

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%206.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%206.png)

→ 해가 없을 경우, 모든 방정식을 만족시키는 해는 없을지라도 최대한 근사하게 만족시킬 수 있는 해를 찾아가는 작업을 함

→ 해가 무수히 많을 경우, regularization (최적의 가중치 찾기)

## 3. Linear Combination, Vector Equations, Four Views of Matrix Mulitplication: Span, linear combination, matrix multiplication의 4가지 관점

### 1) Linear Combinations의 정의

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%207.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%207.png)

### 2) Matrix Equation → Vector Equation

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%208.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%208.png)

### 3) Span

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%209.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%209.png)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2010.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2010.png)

ex) 1 V1 + 1 V1 = 첫번째 화살표

      1 V1 + 2 V2 = 두번쨰화살표

     벡터가 두개일 떄는 span은 평면

     해는 벡터값(화살표가 닿는 ) = 점

### 4) Geometric interpretation of Vector Eqation

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2011.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2011.png)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2012.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2012.png)

벡터가 세개 일때는 span은 공간

풀이의 해는 해당하는 벡터값이 저 평행사변형 평면에 맞게 하는 화살표의 값(분홍색화살표가 가리키는 점)

→ 위 Linear combination(선형결합을 푼다) 

  = 선형 결합의 가중치를 구한다

  = 주어진 세개의 백터의 길이를 잘 조절해서, 해당 꼭지점에 닿게 만들기

 ex) 위 사례처럼 3차원 공간상에 벡터값이 세개가 주어진다면(a1, a2, a3) b를 만족시키는 가중치(x1, x2, x3)는 무조건 있다(span이 전체 공간이 되므로)

만약 벡터값이 두개만 주어진다면, span은 평면에 한정. 평면 바깥쪽에 b가 위치하면 해가 없음

→ 각 벡터값의 차원수를 생각해보자. 방정식의 개수만큼 column 벡터가 생김 : 결국 방정식의 개수와 미지수의 개수를 비교하는것

### 5) Matrix Multiplication - 4 views

**Matrix Multiplications as Linear Combinations of Vectors**

행렬과 벡터의 곱을 따로따로 계산(inner product)해야되는 것으로 보는게 아니라 A**x** = B라는 하나의 방정식으로 생각할 수 있다.

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2013.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2013.png)

**Matrix Multiplications as Column Combinations**

[왼쪽 매트릭스가 base(벡터), 오른쪽 매트릭스가 coefficients(가중치)

매트릭스 x 벡터

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2014.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2014.png)

1. 좌항을 우항과 같이 이해할 수 있음(Matrix→ vector)
2. 우항을 각자의 식으로 보는게 아니라, 각 벡터값을 모아 하나의 인자로 생각하는 것이다.(3개의 컬럼벡터의 span 안에 포함되는 값)

매트릭스 x 매트릭스

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2015.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2015.png)

**Matrix Multiplications as Row Combinations**

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2016.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2016.png)

- 위의 AX = B를 transpose함
- xT(가중치) AT(base)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2017.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2017.png)

**Matrix Multiplicaitons as Sum of (Rank-1) Outer Products**

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2018.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2018.png)

랭크(기저벡터) - span을 형성하는 독립적인 벡터의 개수

[https://blog.naver.com/PostView.nhn?blogId=sw4r&logNo=221416614473&parentCategoryNo=&categoryNo=117&viewDate=&isShowPopularPosts=true&from=search](https://blog.naver.com/PostView.nhn?blogId=sw4r&logNo=221416614473&parentCategoryNo=&categoryNo=117&viewDate=&isShowPopularPosts=true&from=search)

→ 랭크 찾아내는 작업

low rank matrix factorization(행렬 인수분해)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2019.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2019.png)

# Ⅱ. Linear Independence, Span, Subspace, Linear Trasnformation(선형 독립과 선형 변환)

## 1. Linear Independence, Span, Subpace

### 1) Linear Indepedence

- 주어진 벡터들이 Linearly independent → 해가 하나 / 선형 의존인 경우 해가 무수
- 벡터를 하나씩 추가시킨다고 가정할 때, 겹치는 span이 하나도 없는 경우를 의미

### 2) Geometric Understanding of Linear Dependence

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2020.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2020.png)

v1, v2의 span을 다음과 같이 평면으로 표시할 수 있다.

이 내부의 임의의 점을 만족시키는 v1, v2, v3 값을 찾는다고 해보자(3차원말고 그냥 기존 2차원에서 v3를 추가시켜 다른 평면을 그려본다고 생각)

이 때 기존 녹색 평면 span과 다른 span이 생기게 되면 linear dependent(포함하면서 더 크거나 다르거나)

평행사변형이 하나여야 independent

### 3) Subspace

**Subspace**

- 어떤 집합이 어떤 연산에 대해서 닫혀 있다 - 해당 연산의 결과값이 모두 집합 안에 속한다(ex. 자연수는 덧셈 연산에 닫혀있다. 뺄셈에는 닫혀있지 않음)
- 어떤 벡터의 집합이 선형 결합에 닫혀 있는 경우 = subspace
- span은 당연히 선형결합에 닫혀있음

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2021.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2021.png)

Basis of Subspace

어떤 subspace가 주어졌을 때. 이게 기저벡터인지 확인하기(Basis - 기저벡터)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2022.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2022.png)

- 같은 subspace에 대해 다른 기저벡터는 있을 수 있어도(주어진 평면에서 basis를 뽀는다고 하면 이렇게도뽑을 수 있고 저렇게도 뽑을 수 있음), 기저벡터의 개수(=Dimension)는 동일

### 4) Dimension과 Rank

Subspace H에 대해 벡터의 개수(Dimension)은 unique

dim H

- 3차원공간 R³에서 제일큰 subspace는 R³

     → 선형결합에 닫혀있음

     → 이 공간 내 가장 간단한 basis는 

         [1 0 0] [0 1 0] [0 0 1]  

           - 3차원 전체공간 표현 가능

           - linear independent

5) column space - column들의 spanned subspace

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2023.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2023.png)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2024.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2024.png)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2025.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2025.png)

## 2. Linear Transformation

### 1) Linear Transformation

**intro**

정의역(domain)의 원소가 공역(codomain)에 하나씩만 대응되야함

- 정의역 원소에 대응되는 공역 원소가 없어선 안 됨
- 정의역 원소에 대응되는 공역 원소가 2개 이상이어도 안 됨
- 다른 두 정의역 원소에 대응하는 같은 공역 원소가 있는 건 상관없음

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2026.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2026.png)

image - function(x)의 결과 값 y

range(치역) - 모든 image의 집합

**Linear Transformation의 정의**

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2027.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2027.png)

**활용**

- y = ax + b처럼 상수가 붙어있으면 선형 변형이 안됨

    (R¹ → R¹)일때는

- 하지만 행렬 모양으로 변경해서 하면 선형 변형 가능

    R² → R¹로 바꾸면 가능

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2028.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2028.png)

### 2) Matrix of Linear Transformation

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2029.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2029.png)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2030.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2030.png)

→ 선형성을 만족하기 떄문에 각함수값을 먼저 변환시킨 후 더해도 상관없다

.. 정리하자면

1) 우리는 위의 예시에 등장하는 함수가 선형이라는 사실을 앎

2) 임의의 맵핑 벡터값 두개가 주어짐

이 두가지를 이용해서 함수의 full definition을 알아냄

v 벡터와 벡터들 간의 변환에서 선형성이 전제가 된다면,

행렬과 입력벡터의 곱으로 선형적 변환을 항상 표현할 수 있다는 것[벡터와 선형성의 연결고리]

'A**x**'의 형태로 **** 

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2031.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2031.png)

저렇게 1과 0을 이용해서 x를 분해하는 행렬을 standard matrix라고 함(𝑅2 공간에 있는 모든 vector들은 horizontal vector + vertical vector의 합으로 표현이 가능하기 때문에 (i.e., [𝑥,𝑦]=[𝑥,0]+[0,𝑦] ), 이 말은 즉 𝑅2 에 있는 모든 벡터들은 𝐢 와 𝐣 의 linear combination으로 나타낼 수 있다는 말이 됩니다. 이것이 𝐢,𝐣 의 이름이 basis vector인 이유입니다.)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2032.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2032.png)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2033.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2033.png)

### 3) Linear Transformation in Neural Networks

- bias가 있으면 Affine layer(↔︎linear layer)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2034.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2034.png)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2035.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2035.png)

- 왼쪽그림

왼쪽 초록 노드 - 고양이 사진 사분한 픽셀 값을 저장(4차원)

오른쪽 노드 - 분류 대상(3차원)

- 오른쪽그림

    -1번째줄, 2번째줄, 3번쨰줄

    (1) (3 x 4)  x (4x1- 초록노드)  + bias(상수값) = 3차원 벡터(스코어)

    (2) column vector로 나타내기

    (3) A**x**로 나타내기

### 4) Onto and One_to_One (전사함수와 일대일함수)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2036.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2036.png)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2037.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2037.png)

onto : 공역 = 치역(공역 중 함수값이 아닌 것이 없다)

one-to-one : 치역 원소에 정의역 원소가 하나씩만 대응할 때

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2038.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2038.png)

A**x**에서 **x**는 R²(이차원), 옆의 행렬을 모두 계산하면 건 R³

Onto? No. 두개(2차원)만 가지고 선형결합을 한게 R³(3차원)의 span을 포괄하지 못함 (공역의 원소의 개수가 정의역의 개수가 더 많으면 onto가 안 됨)

one-to-one? 

특정 결과 값을 만족시키는 x가 유일한가(linearly independent한가)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2039.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2039.png)

onto? yes (3차원 → 2차원) (물론 아닐수도 있음- 세개 백터가 일치하면)

one-to-one? no - linearly dependent

# Ⅲ. Least Squares

### 1. Ax = b의 해가 존재하지 않을 때, best approximation solution을 찾는 방법 - Least square

### 1) Inner Product(내적)

**정의**

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2040.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2040.png)

벡터들간의 수직 - 내적 연산 : u•v

(uᵀv와 같으나 column 간의 연산으로 표기한 것)

**Inner product의 properties**

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2041.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2041.png)

- 교환법칙, 분배법칙, 상수배 성립
- u•u(자기 자신과의 곱 - 제곱)은 0보다 크다

    (u = 0 일 경우에만 u•u = 0 : 0 벡터)

    → 공간을 생각해보면 당연한 것

- 선형결합시 내적을 먼저하거나 나중에 하거나 같음

### 2) Vector Norm, Orthogonal Vectors

(1) **Vector Norm의 정의** → 벡터의 길이

(2) **Geometric Meaning**

(3) **Unit Vector** - 길이 1 짜리 벡터

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2042.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2042.png)

→ 벡터를 1/vector norm로 상수배 하면 구할 수 있음

**(4) Distance between Vectors in Rⁿ**

**u**와 **v**사이의 거리 = **u** + -1 **v**의 절댓값(norm)(

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2043.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2043.png)

**(5) Inner Product와 Angle Between Vectors** 

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2044.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2044.png)

**(6) Orthogonal Vectors**

내적(u•v)한 값이 0인데, u와 v의 norm이 0이 아니라면 → cos𝜃이 값이 0 : 즉 angle은 직각 

### 3) Least Squares Problem

**(1) Least Square의 정의**

- Overdetermined System(방정식 개수 > 미지수 개수)에서
- **b** = 기존의 방정식 개수 = 미지수 개수인 A**x** = **b**에서의 해
- 새로운 방정식을 추가했을 때, 이 기존의 해가 맞지 않게 됨

    → 여기서 적절히 approximation을 하는 것(벡터 **b**와 A**x** 간의 distance 최소값 구하기**)**

  모든 **b** - A**x**의 절댓값의 합 = 제곱해서 더한 것의 sqaure root

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2045.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2045.png)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2046.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2046.png)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2047.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2047.png)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2048.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2048.png)

- Ax가 형성하는 span 안에 기존 벡터 b가 포함되지는 않지만 여하튼 col A (column space of A)로 표현 가능

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2049.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2049.png)

- Least Square 구하기 : **b**와 A**x** 사이의 distance 구하기

### 4) Geometric Interpretation of Least Squares

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2050.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2050.png)

- Ax가 형성하는 span과 벡터 b 사이의 거리 b-Ax^(b-b^)

    (수선의 발을 내린 지점 bˆ(b hat)까지의 거리)

    b^ = Ax^인 점 

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2051.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2051.png)

   ㄱ. Col A 안의 모든 벡터에 대해서도 수직이어야 함

   ㄴ. 원점에서부터 출발하는 어떤 벡터와도 수직

→ 어떤벡터와도 수직인 것을 분배법칙을 사용해서 하나하나 따지면 증명가능

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2052.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2052.png)

- basis vector(재료 벡터) 하나하나와 개별적으로 수직이면, 모든 linear combination과 수직
- 이걸 AX = 0의 꼴로 간편하게 행렬식으로 표현

     이걸 solution으로 구할 수 있다는게 포인트! 

수직 → 내적 → Matrix equation (AᵀX = 0벡터)

### 5) Normal Equation(기하학적으로 이해)

**x^** = (AᵀA)⁻¹ Aᵀ**b**

- 평면에 수직(normal)인 벡터(법선벡터)
- 좌행의 Aᵀ A**x**^에서 Aᵀ@A는 무조건 정사각행렬, 그 중에서도 row와 column의 개수는 미지수 수만큼 나옴
- 우행의 Aᵀ**b**도 미지수 개수에 해당하는 vector

여기선 구한 x^가 밑의 x^와 같아진다는 것

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2053.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2053.png)

즉, 최소화의 문제가 방정식을 푸는 것으로 바뀜

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2054.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2054.png)

### 6) Another Derivation of Normal Eqaution(미분으로 이해)

방정식을 생각해보자

x²-2x+3의 최솟값은 이 식의 미분값 2x-2=0일 때의 x값이다

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2055.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2055.png)

normal eqaution도 마찬가지의 개념을 적용할 수 있다.

최솟값을 구할 식을 미분해서, 해당 식(gradient vector) = 0벡터 이 성립하게 해주면됨

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2056.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2056.png)

(제곱하고나, 루트를 씌워도 최솟값은 마찬가지)

x^ = 원래식(앞에서 본 최소화식) = 원래식 제곱

     = 원래식 제곱을 Transpose를 이용해 표시 = 식 분해한 것

    위 식을 미분한 것 = 0  이것이  AᵀA**x** = Aᵀ**b**와 같다는 것

 우리가 geometric 개념으로 이해한 normal equation과 똑같이 나옴. 그래서 마찬가지로 AᵀA가 inversible이라면 x를 다음과 같이 정리할 수 있다.

**x** = (AᵀA)⁻¹ Aᵀ**b** 

[transpose 미분하는 방법]

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2057.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2057.png)

(1)

f(x) = 3x₁ + 5x₂ 를 행렬식으로 나타내면 위의 첫번째 줄

→ aᵀx(또는 xᵀa로도 표현 가능)

f´(x) = a

∴  aᵀx 또는 xᵀa를 미분하면 a

(2)

f(x)g(x)h(x)를 미분하면 위와 같음(하나씩 변수로 잡고 나머지는 변수로 안 잡고 편미분한걸 더한다고 생각하면 됨)

f(x) = xᵀAx 또한 이방식대로 한번은 xᵀ를 변수로, 다음한번은 x를 변수로 잡고 편미분한 걸 더하면 됨.

f´(x) = (A+Aᵀ)x

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2056.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2056.png)

이걸 이용해서 bᵀb  - xᵀAᵀb - bᵀAx +xᵀAᵀAx 미분하면 (각 항 1,2,3,4로 지칭) 1은 없어지고 2는 -Aᵀb, 3은 -bᵀA(=-Aᵀb), 4는 AᵀAx + xᵀAᵀA(=AᵀAx) = 2AᵀAx

→ normal equation 유도 가능

**7) Least square: when (A^T)A is not invertible**

linear combination의 해가 무한하든 없든(span되지 않는 벡터라도) 그 벡터에서와 subsapce를 연결하는 수선의 발은 무조건 존재하니깐

수선의 발은 항상 unique함(lin comb의 해가무한할때도 - 이 점을 표현할 수 있는 식이 많아질 뿐)

실제 데이터에서 invertible하지 않은 경우가 거의 없음

→ 자료가 linearly dependent하단 얘긴데, 데이터 선형결합이 정확히 상수배되기가 어려움

![Untitled](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2058.png)

AᵀA**x** = Aᵀ**b**

b = Ax + e(수선의 발을 내린 거리 벡터)

Aᵀb = Aᵀ(Ax+e) = AᵀAx +Aᵀe(항상 직교 =0)

        = AᵀAx

∴ invertible이든 아니든 항상 normal equation을 적용할 수 있음

## 2. Orthogornal Projection Perspctive

[https://ghebook.blogspot.com/2010/07/vector.html](https://ghebook.blogspot.com/2010/07/vector.html)

기하학적 이해가 바탕이 되어야 하는 파트이기에 위 자료를 참고하면 좋을 듯.

수선의 발 내리기

= b를 Ax^와 맵핑하기 

= f(b)

b^ = Ax^ 

f(b) = A(AᵀA⁻)¹Aᵀ**b** 

= C**b**

다음식이 linear transformation의 형식임에 착안해서

C = A(AᵀA)⁻¹Aᵀ

이걸 좀 간단하게 만들어보겠다는 것.

### Onthogonoal & Onthonormal Basis

orthogonal : 임의의 벡터 두개 뽑았을 때 서로 수직임

orthonormal: 길이가 1인 orthogonal

→ 각 벡터가 모두 linearly independent

(geometric으로 생각하면 직관적임 - 모든 벡터가 각자 서로 수직이니깐) 

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2059.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2059.png)

(3차원)

v**Orthogonal projection이 왜 필요한가?**

(직관적으로 이해하기)

→ normal equation을 보다 쉽게 구하려고

C = A(AᵀA)⁻¹Aᵀ 의 식이 까다로움 

특히, 역행렬부분 (AᵀA⁻)¹

을 처리하기가 어려움(나누기(1/ad-bc랑 비슷해서, 메모리에 소수점 처리가 잘 안 됨)

→ 작은 오차지만 머신러닝에선 큰 오류로 이어질 수 있음

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2060.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2060.png)

만약 A를 onthonormal한 u로 바꿔서 계산하면 훨씬 편함. 둘이 곱하면 대각선은 자기자신과 곱하기 때문에 1, 나머지는 수직인 벡터와 내적하기 때문에 0,  

uᵀu = 단위행렬

u(uᵀu)⁻¹uᵀ  = uuᵀ

∴b^ = uuᵀb 만 남는다. 

(주의: uuᵀ는 identity matrix가 아니다)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2061.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2061.png)

### Onthogonal Projection y^ of y onto Line, Plane

**1) onto Line**

[https://soohee410.github.io/orthogonal_projection](https://soohee410.github.io/orthogonal_projection)

(설명 지리게 잘 돼있음)

![Untitled](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2062.png)

**2) onto Planle**

![Untitled](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2063.png)

**3) onto Subspace (스스로가 속한 subspace에 projection)**

### Gram-Schmidt process

(QR

subspace를 유지하면서, orthogonal로 바꾸기

[그림으로 이해하기]

(1) v2에서 v1으로 수선의 발을 내린다

(2) 수선의 발까지 v1(v1')을 unit vector로 표현해준다(길이가 1이 되도록 v를 나눠준다 피타고라스 이용해서 계산한 길이로) - 같은 span을 커버하지만, 길이가 1인 v1'의 탄생

(3) v1'과 합이 v2가 되도록 하는 벡터(v2-v1')을 그려준다.  : 평행사변형 + 90도 

→ 이 벡터는 아까 내린 수선을 옆으로 옮긴거랑 똑같음

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2064.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2064.png)

식으로으로 이해하기

1)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2065.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2065.png)

2)u에 cos𝜃를 곱하면 y가 나온다는 성질 이용

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2066.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2066.png)

정리

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2067.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2067.png)

### QR Factorization(QR분해)

![%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2068.png](%E1%84%89%E1%85%A5%E1%86%AB%E1%84%92%E1%85%A7%E1%86%BC%E1%84%83%E1%85%A2%E1%84%89%E1%85%AE(2%E1%84%8C%E1%85%AE)%201ac9bceb0551451fa82e8f5a8c7bcb80/Untitled%2068.png)

→ upper triangular matrix 나옴

그램-슈미트, QR분해