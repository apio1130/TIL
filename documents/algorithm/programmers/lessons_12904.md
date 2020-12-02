# 해당 숫자 구간의 팰린드롬의 수를 구하는 문제

회문이라고도 하는 팰린드롬에 대한 문제.

## 회고
늦은 시간에 피곤한 상태로 해서인지(핑계😂) 해결을 위한 알고리즘을 생각하지 않고  
문제만 읽고 그대로 무식하게 풀어봤더니 보기 안좋게 코드를 작성한 것 같다.

처리 방법에 대해 굳이 중간 글자를 제외한 앞 뒤를 짤라서 하나를 뒤집어서 비교할게 아니라  
for문에서 글자의 앞과 뒤의 인덱스를 비교해서 일치하는 수에 대해 카운팅을 해주면 됐을거라고  
뒤늦게 떠올랐다. 😥

> 문제의 코드
```javascript  

function solution(n, m) {
  var answer = 0;
  
  for (let i = n; i <= m; i++) {
    if (i < 10) {
      answer++;
      continue;
    }
    let numLen = i.toString().length;
    let mid = Math.trunc(numLen / 2);
    let statWith = numLen % 2 == 0 ? 0 : 1;
    let prev = i.toString().substring(0, mid);
    let sufix = i.toString().substring(mid + statWith , numLen).split("").reverse().join("");
    if (prev == sufix) {
        answer++;
    }
  }
  return answer;
}

```

> 개선한 코드
```javascript
function solution(n, m) {
  let answer = 0;
  
  for (let i = n; i <= m; i++) {
    let numb = i.toString();
    let length = numb.length;  
    let addVal = 1;
    
    for (let j = 0; j < length / 2; i++) {
        if (numb.charAt(j) != numb.charAt(length -j -1)) {
          addVal = 0;
          break;
        }
    }
    
    if (addVal > 0) {
      answer += addVal;
    }
  }
  
  return answer;
}

```

