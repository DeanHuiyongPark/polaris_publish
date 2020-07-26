# coding list
/polaris/codingLIst.html : [LINK](http://localhost:8080/polaris/codingLIst.html)

# components
- components로 불러오는 경우
- components- 로 시작하는 클래스로 영역생성.
- components- 에는 스타일을 주지 않는다.
- components- 부분은 안에 코드를 불러온 후 삭제된다.   
(react와 비슷한 구조를 만들기 위해 처리) 
```    
<div class="components-name"></div>
```
```
//스크립트
var callbackItem1 = function(v){
    $('[components-name] > *').unwrap();
};

$plugins.uiPageLoad('[root]', '[components-name]', callbackItem1)
.then($plugins.uiPageLoad('[root]', '[components-name]', callbackItem2));
```

