### 프로그래머스_거스름돈
```java
class Solution {
    public int solution(int n, int[] money) {
        int[] arr = new int[100001];

        arr[0] = 1;

        for (int i = 0; i < money.length; i++) {
            for (int j = money[i]; j <= n; j++) {
                arr[j] += arr[j - money[i]];

                arr[j] %= 1000000007;
            }
        }

        return arr[n];
    }
}
```
money[i]에서 n을 표현한 경우의 수와  
money[i+1]에서 n - (i+1)을 표현한 경우의 수를 더해준다.

