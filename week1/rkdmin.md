### 프로그래머스_멀리뛰기
```java
class Solution {
    public static int dp[];
    
    public long solution(int n) {
        dp = new int[n + 1];
        return fibo(n) % 1234567;
    }
    
    
    public static int fibo(int n){
        // 이미 알고있는 f(n)이면 바로 리턴
        if(dp[n] != 0) return dp[n];
        
        if(n == 1){
            return 1;
        }
        if(n == 2){
            return 2;
        }
        dp[n] = (fibo(n - 1) + fibo(n - 2)) % 1234567;
        return dp[n];
    }
}
```

### 프로그래머스_표현 가능한 이진트리
```java
```