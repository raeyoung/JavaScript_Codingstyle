# JavaScript_Codingstyle

개발자는 되도록이면 간결하고 읽기 쉽게 코드를 작성해야 한다.
<br><br><br>
## 문법
### 중괄호
    if  (condition)  {  
	    // 코드 1  
	    // 코드 2  
	    // ...코드 n...  
    }

<br><br>
### 가로 길이
    if  ( 
	    id ===  123  && 
	    moonPhase ===  'Waning Gibbous'  && 
	    zodiacSign ===  'Libra'  
    )  {  
	    letTheSorceryBegin();  
    }

80자나 120자로 제한하는 게 일반적이다.
<br><br>
### 들여쓰기

가로 들여쓰기: 스페이스 두 개 혹은 네 개를 사용해 만듦 

    show(parameters, 
	 aligned, // 스페이스 다섯 개를 이용해 들여쓰기 함
	 one, 
	 after, 
	 another
	 ) {  
	  // ...  
    }
  
  <br>
세로 들여쓰기: 논리 블록 사이에 넣어 코드를 분리해주는 새 줄

    function pow(x, n) {  
        let result = 1;  
        // 				<--  
        for (let i = 0; i < n; i++) { 
        result *= x;  
        }  
        // 				<--  
        return result;  
        }
    

 <br>
 
### 중첩 레벨 가능한 너무 깊은 중첩레벨을 사용 자제  
### 함수의 위치 
1. 헬퍼 함수를 사용하는 코드 위에서 헬퍼 함수를 모아 선언하기 
2. 코드를 먼저, 함수는 그 다음에 선언하기 
3. 혼합: 코드 바로 위에서 필요한 헬퍼 함수 그때그때 선언하기

대게 2번째 방법을 선호 이 코드가 '무엇을 하는지’를 생각하며 코드를 읽기 때문에 코드가 먼저 나오는 것이 자연스럽기 때문이다. 
이름만 보고도 헬퍼 함수의 역할을 쉽게 유추할 수 있게 헬퍼 함수 이름을 명명했다면 함수 본문을 읽을 필요도 없다.  
  
출처 :  [https://ko.javascript.info/coding-style](https://ko.javascript.info/coding-style)
