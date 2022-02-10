---
layout: single
title:  "[CSS] Selector" 
---

   
#### Selector 종류    
1. id Selector : #     
2. class Selector : .     
3. tag Selector : li{}     
※id는 한번만 사용, class는 여러번 사용 할 수 있다.   

##### 부모자식 Selector   
ul li{} <- ul밑의 모든 li
ol>li <- ol바로 밑의 li만 적용  
ul, ol <- ul, ol 공통된 부분일 때 사용   
   
Tip: Selector 연습: flukeout.github.io  
 
##### Pseudo Class Selector
element의 상태에 따라 선택되고 안되는 것   
```
a:link{		<--방문 안한 것
    color:black
}
a:visited{	<-- 방문 한것(visited는 보안적 문제로 인해 속성이 제한적이다)
    color:red;
}
a:hover{
    color:yellow;
}
a:active{
    color:green;
}
a:focus{
    color:white;
}
```
동시에 될 때 뒤쪽에 있는 선언을 선택   
      
##### 다양한 Selector     
orange.small   
모든 오렌지에 대해서 class 값이 small   
   
plate, bento <- 모든 plate와 모든 bento 선택   
   
**  
모든 태그 선택   
    
plate *  
plate 밑 모든 것    
   
plate+apple  
plate에 인접한 apple   
   
bento~pickle   
bento에 인접한 모든 pickle 선택   
   
plate > apple  
plate 직계 자식인 apple   
   
:first-child   
plate orange:first-child  
plate밑에 첫번째로 등장하는 orange   
   
:only-child  
only element 다른 요소 내부의 유일한 요소를 선택   
   
:last-child   
다른 요소 내부의 마지막 자식 요소를 선택   
   
:nth-child(A)   
다른 요소 내부의 A번째 요소 선택   
   
:nth-last-child(A) 
다른 요소 내부의 뒤에서 A번째 요소 선택   
   
:first-of-type  
특정 타입이 처음 등장하는 곳   
   
:nth-of-type(A)  
odd,even의 경우 홀,짝수에 해당하는 모든 것   
   
:nth-of-type(An+B)   
ex) 2n+1 1,3,5해당하는 것   
   
:only-of-type    
ex)li:only-of-type 자기 자신 타입만 있을 경우   
   
:empty  
자식이 없는 요소 선택   
   
:not(X)  
X가 아닌 모든것을 선택   
