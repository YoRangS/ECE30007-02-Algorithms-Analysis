# ECE30007-02_IAIP

## 2주차
### O-notation
$O(g(n))$은 모든 $n>=n_0$에서 $0<=f(n)<=cg(n)$을 만족하는 $c (c>0)$와 $n_0$이 있을 때 $f(n)$의 집합

ex) $2n^2 = O(n^3)$, with $c=1$ and $n_0 = 2$

### $\Omega$-notation
$\Omega(g(n))$은 모든 $n>=n_0$에서 $0<=cg(n)<=f(n)$을 만족하는 $c (c>0)$와 $n_0$이 있을 때 $f(n)$의 집합

ex) $\sqrt(n) = \Omega(lgn)$, with $c=1$ and $n_0 = 16$

### $\Theta$ -notation
$\Theta(g(n))$은 모든 $n>=n_0$에서 $0<=c_1g(n)<=f(n)<=c_2g(n)$을 만족하는 $c_1, c_2 (c_1>0, c_2>0)$와 $n_0$이 있을 때 $f(n)$의 집합

ex) $n^2/2-2n = \Theta(n^2)$, with $c_1=1/4$, $c_2=1/2$ and $n_0 = 8$

### o-notation
o(g(n))은 어떤 c>0에서든지 모든 $n>=n_0$에서 $0 <= f(n) < cg(n)$을 만족하는 $n_0>0$이 존재할 때 
$f(n)$의 집합

$o(f)=O(f)-\theta(f)$

### $\omega$-notation
$\omega$(g(n))은 어떤 c>0에서든지 모든 $n>=n_0$에서 $0 <= cg(n) < f(n)$을 만족하는 $n_0>0$이 존재할 때 $f(n)$의 집합

$\omega(f)=\Omega(f)-\theta(f)$

$g(n)=o(f(n))$ <=> $f(n)=\omega(g(n))$

### Proposition
1. $f(n)\in\Theta(f(n))$
2. $f(n)\in\Theta(g(n))$ <=> $g(n)\in\Theta(f(n))$
3. $f(n)\in\Theta(g(n))$ and $g(n)\in\Theta(h(n))$ => $f(n)\in\Theta(h(n))$

### 알고리즘의 시간복잡도
$O(n^2)$: 알고리즘의 worst case
$\Omega(n^2)$: 알고리즘의 best case
$\theta(n^2)$: 위의 2개 

## 3주차
### Recurrence vs Recursion
재귀(recursion)와 순환(recurrence)은 컴퓨터 과학과 수학에서 관련된 개념입니다. 그러나 두 개념은 서로 다릅니다.

순환(recurrence)은 이전 값에 기반하여 정의된 숫자나 다른 객체의 시퀀스를 나타냅니다. 흔한 예로는 각 항이 이전 두 항의 합인 피보나치 수열이 있습니다. 순환 관계는 해석적 또는 수치적으로 해결되어 시퀀스의 값을 임의의 인덱스에 대해 찾을 수 있습니다.

재귀(recursion)는 함수가 자신을 호출하여 문제를 해결하는 프로그래밍 기술을 말합니다. 함수는 일반적으로 기본 사례(base case)와 재귀적 사례(recursive case)를 가지며, 기본 사례는 직접 해결할 수 있는 간단한 경우이고, 재귀적 사례는 문제를 작은 하위 문제로 분해하고 재귀적으로 해결합니다. 재귀는 일반적으로 트리를 탐색하거나 팩토리얼을 계산하는 등 자연스러운 재귀적 구조를 가진 문제를 해결하는 데 사용됩니다.

따라서, 재귀와 순환 모두 이전 값이나 작은 하위 문제에 기반하여 문제를 정의하는 것은 유사하지만, 서로 다른 개념이며 다른 응용 분야가 있습니다.

- ChatGPT 참조

### Solving recurrence equations
#### Iteration method
#### Substitution method
#### Recursion-tree method
#### Master method
