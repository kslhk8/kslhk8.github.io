---
layout: single
title:  "[CSS] Display, Position" 
---

##### Inline vs Block  
Block   
새로운 라인(line)에서 시작하며, 해당 라인의 모든 너비를 차지   
   
Inline   
컨텐츠 크기만큼만 차지   
```
display:inline
컨텐츠 크기만큼만 사용
display: block
화면 전체를 사용
``` 
※inline방식은 width, height 값을 무시한다.   
   
box-sizing   
width, height를 지정할 때 border등으로 인해 설정이 헷갈릴 때   
box-sizing:border-box <- border의 경계에 맞춰서 width, height 설정   
   
마진겹침   
부모 태그가 시각적 효과 없을 경우(border X), 자식 tag와 부모 tag 마진이 합쳐짐   
Math.max(부모 마진, 자식 마진)이 자식 element의 위치로 사용된다.   
태그에 시각적 요소가 없을 경우 더 큰값이 그 태그의 margin이 된다.   

##### Position   
Relative   
원래 위치를 기준으로 상대적으로 이동시키고 싶을 때   
   
Static(position default)  
offset을 무시함(left,right등)   
   
Absolute
left와 top은 부모 element기준으로 원래 위치가 기본값 설정 돼있음    
static이 아닌 부모가 있을 때 부모의 위치를 기준으로 위치 지정   
컨텐츠 크기만큼 유지
      
Fixed   
화면에 고정시키 위한 것   
absolute와 비슷하다.   