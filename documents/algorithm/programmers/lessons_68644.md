# 두개 뽑아서 더하기

```java 
import java.util.*;

class Solution {
    public int[] solution(int[] numbers) {
        int[] answer = {};
        if (numbers == null || numbers.length < 2) {
            return answer;
        }
        Set<Integer> numberSet = new HashSet<>();
        for (int i = 0; i < numbers.length-1; i++) {
            for(int j = i+1; j < numbers.length; j++) {
                numberSet.add(numbers[i] + numbers[j]);
            }
        }
        answer = numberSet.stream().sorted().mapToInt(Integer::intValue).toArray();
        return answer;
    }
}
```
