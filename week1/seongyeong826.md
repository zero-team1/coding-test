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