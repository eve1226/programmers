# programmers
* [이상한 문자 만들기](https://school.programmers.co.kr/learn/courses/30/lessons/12930)
```java
class Solution {
    public String solution(String s) {
        String answer = "";
        
        int index = 0;
        
        for(int i = 0; i < s.length(); i++){
            index++;
            char t = s.charAt(i);
            
            if(t == ' '){
                index = 0;   
            }
            if(index%2 == 1){ 
                t = Character.toUpperCase(t);
            }else {
                t = Character.toLowerCase(t);
            }
            
            answer += t;

        }
        return answer;
    }
}
```
