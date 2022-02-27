# solve_nonogram

C/C++을 이용하여 노노그램을 완성해주는 프로그램을 만들어보려 한다.
노노그램의 재미를 알려준 침착맨에게 감사하다. 

## 어떻게 문제를 풀것인가?


아래를 반복한다.

1. 각 행/열의 단서와 이미 채워진 칸을 참고하여 모든 경우의 수를 생각한다. 
    1. 이미 채워진 칸을 참고한다.
    2. 모든 경우의 수를 계산한다.
2. 모든 경우의 수에서 무조건 칠해지는 칸과 무조건 안 칠해지는 칸을 특정한다.


---

모든 칸이 비워져있다고 가정하면,

- 각 단서 사이에는 한 칸 이상을 비워야 할 것이다.
- 양 끝은 비우지 않아도 되지만 띄워질 수도 있을 것이다.
- 따라서 단서의 양 끝과 그 사이사이에는 공간이 있을 것이다.
- 행/열에 단서와 최소한의 공간을 집어넣으면 남는 공간이 있을 것이다.
이 남는 공간을 단서의 양 끝과 그 사이사이에 나누어 넣어야 할 것이다.

정리하면, 일렬로 놓인 몇개의 주머니에 몇개의 구슬을 나누어 넣는 경우의 수를 계산해야 할 것이다. 그런데, 위는 ‘모든 칸이 비워져있을 때’만 적용할 수 있다.

---
