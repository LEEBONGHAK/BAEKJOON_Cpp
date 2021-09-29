# [스택](https://www.acmicpc.net/problem/10828)  
  
### 문제  
  
정수를 저장하는 스택을 구현한 다음, 입력으로 주어지는 명령을 처리하는 프로그램을 작성하시오.  
명령은 총 다섯 가지이다.  
 - push X: 정수 X를 스택에 넣는 연산이다.  
 - pop: 스택에서 가장 위에 있는 정수를 빼고, 그 수를 출력한다. 만약 스택에 들어있는 정수가 없는 경우에는 -1을 출력한다.  
 - size: 스택에 들어있는 정수의 개수를 출력한다.  
 - empty: 스택이 비어있으면 1, 아니면 0을 출력한다.  
 - top: 스택의 가장 위에 있는 정수를 출력한다. 만약 스택에 들어있는 정수가 없는 경우에는 -1을 출력한다.  
  
### 입력  
  
첫째 줄에 주어지는 명령의 수 N (1 ≤ N ≤ 10,000)이 주어진다. 둘째 줄부터 N개의 줄에는 명령이 하나씩 주어진다. 주어지는 정수는 1보다 크거나 같고, 100,000보다 작거나 같다. 문제에 나와있지 않은 명령이 주어지는 경우는 없다.  
  
### 출력  
  
출력해야하는 명령이 주어질 때마다, 한 줄에 하나씩 출력한다.  
  
### 예제  
  
|입력|출력|
|---|---|
|14<br/>push 1<br/>push 2<br/>top<br/>size<br/>empty<br/>pop<br/>pop<br/>pop<br/>size<br/>empty<br/>pop<br/>push 3<br/>empty<br/>top|2<br/>2<br/>0<br/>2<br/>1<br/>-1<br/>0<br/>1<br/>-1<br/>0<br/>3|
|7<br/>pop<br/>top<br/>push 123<br/>top<br/>pop<br/>top<br/>pop|-1<br/>-1<br/>123<br/>123<br/>-1<br/>-1|

### stack<template> - 주요 함수
  
stack<template> - 주요 함수 (중요!)
 - stack<int> stk; => int형 자료를 담는 stack 생성  
 - stk.push(i) => stk의 맨 위에 원소 i를 추가  
 - stk.pop() => stk의 맨 위에 있는 원소를 삭제  
 - stk.top() => stk의 맨 앞에 있는 원소를 조회  
 - stk.size() => stk의 크기를 확인  
 - stk.empty() => stk가 비어있다면(size가 0이라면) true, 아니라면 false  