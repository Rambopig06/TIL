## 함수

### Function(함수)

함수를 영어로 표현하면 펑션 (function) 이다.<br/>
특정한 작업을 수행하는 코드인데<br/>
<br/>
특정한 기능을 만들어놓고 함수로 정한뒤, 원할 때 꺼내쓰는 개념이다.<br/>
예시를 들자면, 드라마 중증외상센터에서 나온적이 있던 '코드 블루'는<br/>
어떤 환자에게서 심정지가 발생하면 의사들에게 그 사실을 알려주는 암호인데,<br/>
<br/>
환자에게서 심정지가 발생했을 경우 의사들에게 주어지는 업무를<br/>
'코드 블루'라고 표현한 것, 함수의 개념과 일치하다.<br/>
<br/>
위에서 들었던 예시로 코드를 쓴다면 대략 이렇다.

```
function codeblue(){
    console.log('심정지 환자 발생!')
}
```

![함수 호출](https://github.com/user-attachments/assets/4c51ef22-65cd-44f7-a3cf-4497a78b3fe3)


위의 코드를 입력 후, 함수가 저장이 된다.<br/>
그런 다음 저장한 함수를 콘솔에 쓰면,<br/>
함수에서 정해놓았던 기능이 작동하여 '심정지 환자 발생!' 이<br/>
콘솔에 쓰이게 된다.<br/>
<br/>

![함수 여러번 호출](https://github.com/user-attachments/assets/2f89145a-4285-43e7-a082-a18d2208e564)

이렇게 함수를 여러번 입력후 실행하면,<br/>
같은 함수라도 여러번 출력할 수 있다.<br/>
<br/>

### return(반환 값)

함수 실행 후, 실행문 밑줄에 undifined가 같이 출력되는데,<br/>
console.log 의 기본 '반환 값'이 undifined라서 그렇다.<br/>
함수를 호출하면 결과 값이 표출되는데 이를 '반환 값'이라고 한다.<br/>
<br/>
그래서,

```
function a(){
    console.log('a');
}
```
와
```
function a(){
    console.log('a');
    return undifined;
}
```
는 동일하다고 할 수 있다.<br/>
처음보는 문법이 보이는데,<br/>
<br/>
반환 값(return value)의 기본 값은 undifined 이지만<br/>
return 문을 추가하면 반환 값도 임의로 지정할 수 있다.

```
function codeblue(){
    console.log('심정지 환자 발생!');
    return '안내방송 완료.';
}
```
이렇게 실행문 작성영역에 return문을 추가하면<br/>
return 문에 적었던 값이 반환 값 위치에 적용된다.

![반환값 한글](https://github.com/user-attachments/assets/5e7a624f-124d-48af-9a09-ed45745d4777)

### return 문의 특성

```
function fight(){
    console.log('철수 : 너가 나빴어!');
    console.log('영희 : 아니야 너가 더 나빴어!');
}
```

![철수영희말싸움](https://github.com/user-attachments/assets/fb7133ba-6c2e-4a44-b47b-f0d7cf50f4dc)

어머, 이번엔 철수와 영희가 싸우고 있다.<br/>
싸움은 말리라고 배웠는데 어떻게 말려야 할까..?<br/>
<br/>

![철수만 말하기](https://github.com/user-attachments/assets/284c3124-e0f3-4ee8-a13d-d96e84e9ec1d)

return이 끼어들며, 영희의 대화가 콘솔에 적용되지 않았다.<br/>
이렇게 영희만 억울한 엔딩이 되었지만,<br/>
우리는 영희를 공감하기 전에 왜 이런결과가 나왔는지 주목해야한다.<br/>
<br/>
console.log('영희 : 아니야 너가 더 나빴어!');<br/>
보다 return; 이 더 윗줄에 있기 때문인데,<br/>
<br/>
return은 반환 값(결과 값)을 출력하는 명령어이다.<br/>
그렇기 때문에, 영희가 콘솔에 대화를 하기도 전에<br/>
결과 값을 출력하여 이 대화 자체를 종료한 상황인거다.<br/>
<br/>
더욱 억울하겠지만<br/>
return 값까지 정하여 출력한다면<br/>

![리턴의 이간질](https://github.com/user-attachments/assets/2435d318-1e63-4e24-b6ce-adbed806aa19)

이렇게 return 문이 실행되면서 밑에있는 코드를 실행이 안되는 것이다.<br/>

하지만

```
function fight(){
    console.log('철수 : 너가 나빴어!');
    if(false){
    return '어 철수가 이겼다';
    }
    console.log('영희 : 아니야 너가 더 나빴어!');
}
```
이렇게 return문을 거짓으로 만들어 실행을 시키지 못하게 하면<br/>

![영희 구원해주기](https://github.com/user-attachments/assets/997460c4-5402-4988-93b9-1351ad22e33b)

영희의 대화가 방해받지않고 성공적으로 콘솔에 출력된다.<br/>

### parameter(매개변수)

변수문의 꽃이라고 할 수 있는 요소 중 하나인 '매개변수'에 돌입했다.<br/>
여기까지 따라온 나나 독자분들 전부 셀프 박수한번씩 쳐주자(짝짝)<br/>
<br/>
개인적으로 매개변수를 공부하면서 머리가 많이 깨질 것 같았지만,<br/>
매개변수를 배움으로써 본격적으로 자바스크립트 구동을 하는 느낌도 든다.<br/>
<br/>
예시로 또 들어서 미안하지만 철수와 영희를 이용하여 설명하겠다.<br/>

```
function fight()
```
(미완성 영역)
