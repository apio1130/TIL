# 14. Longest Common Prefix
[소스코드](https://github.com/apio1130/algorithm-practice/blob/master/src/main/java/com/algorithm/leetcode/longestcommonprefix/Solution.java)


1. 문제 요약  
문자열 배열의 가장 긴 접두사 찾기

**Example 1**
```
Input: ["flower","flow","flight"]
Output: "fl" 
```  
**Example 2**
```
Input: ["dog","racecar","car"]
Output: ""
Explanation: There is no common prefix among the input strings.
```
2. 해결 방법
    1. 문자열 배열에 대해 사전순으로 정렬 후, 가장 긴 문자열과 짧은 문자열에 대해 짧은 문자열 기준으로 한글자씩 비교하는 방법
    1. 문자열 배열에 대해 한글자씩 비교해서 판단하는 방법
