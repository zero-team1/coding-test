### 프로그래머스_멀리뛰기
```java
class Solution {
    public long solution(int n) {
        int[] dp = new int[2000];
        dp[1] = 1;
        dp[2] = 2;

        for (int i = 3; i <= 2000; i++) {
            dp[i] = (dp[i-2] + dp[i-1]) % 1234567;
        }

        return dp[n];
    }
}
```

### 프로그래머스_표현 가능한 이진트리
```java
```

### 프로그래머스_귤 고르기
```java
// 같은 종류끼리 묶기
// 각 종류의 길이를 비교해서 큰 길이부터 작은 길이 순서대로 length값 저장하기
// k크기만큼 반복문 돌리면서 길이 순서대로 비교하며 종류가 다른 길이값이 나오면 count up
```

### 프로그래머스_단어 변환
```java
// 
```