# 반복문


## While 문
```
while(조건식){
    실행문;
    }
```
while 문은 조건식의 조건이 참인동안 실행문의 코드를<br/>
반복해서 실행시킨다.<br/>
비유를 하자면 , 방 스위치의 버튼이 ON인동안,<br/>
방 전등을 키고 있는 것.<br/>
<br/>
이번에는 반복문에 관해서 공부해 볼 것이다.<br/>
저번에는 철수 몸무게와 영희의 시험점수를 알아보았다.<br/>
<br/>
이번에는 조금 마음 아프지만 영희의 시험점수 값을 활용해<br/>
무한으로 잔소리하는 프로그램을 만들 것이다.

```
while(영희시험점수 <= 80){
    console.log('공부 좀 해라!!!');
}
```
영희시험점수 값이 80 이하일 때,<br/>
공부 좀 해라!! 를 반복시키는 코드이다.<br/>

![공부 좀 해라 무한반복](https://github.com/user-attachments/assets/ca61a2ed-1923-46c9-9c3f-c9e8aac9755a)

이렇게 조건에 부합하므로 실행문의 값이 반복된다.<br/>
하지만 콘솔에 출력하는 실행문에<br/>
명령을 종료시키는 코드를 작성하지 않아서 무한반복이 되어 버린다.<br/>
<br/>
크롬 브라우저 콘솔에서 작업한다고 쳤을 때,<br/>
탭을 아예 닫고 다시 새로운 탭으로 콘솔을 열어야하는 불상사가 생긴다.<br/>
반복은 하되, 한계치를 두어 적당히 반복시키는 방법이 있다.<br/>


```
let i = 1;
while(영희시험점수 <= 80 || i<=1000){
 console.log('공부 좀 해라!!');
 i++;
}

```
변수 i를 선언하고 그 변수 값을 1로 설정한다.<br/>
조건문에 있는 조건은, 영희시험점수가 80 이하거나<br/>
i값이 1000 이하일때 실행되는 코드이다.<br/>
<br/>
한번 실행시킬 때 마다 i값이 1씩 오르지만,<br/>
영희시험점수에는 변동이 없으므로 i가 1000이하가 될 때 까지<br/>
실행문의 코드를 반복한다.<br/>
실행문의 '공부 좀 해라!' 를 1000번 들어야 하는 셈이다.<br/>
(그래도 무한히 듣는 것 보단 양반이지 않는가.)<br/>
<br/>

이번엔 1~100까지 출력하는 코드를 간단히 만들어 보겠다.

```
let i = 0;
while(i < 100){
    console.log(i + 1);
    i++;
}
```

이 코드를 실행 했을 때 출력 결과는 이렇다.

![1부터100처음](https://github.com/user-attachments/assets/870b9ca9-43e5-4ff6-bb19-a2470c5c61db)

![1부터100끝'](https://github.com/user-attachments/assets/b20e7356-c233-4896-af52-05b9f015ff64)


콘솔 값 출력 후 마지막 부분에 99가 한번 더 출력되는<br/>
사소하지만 거슬리는 문제가 발생했다.<br/>
어떤 원리로 99가 한번 더 나오는지는 파악하기 어렵지만,<br/>
크롬 콘솔창을 개발환경으로 썼을 때만 이러한 문제가 발생하는걸 보니,<br/>
단순히 개발환경 때문일거라 생각된다.<br/>
(이 문제의 원인을 아무리 검색하고 알아봤지만 답이 안나온다.)

## for문

for문은 조건식 작성이 약간 복잡하다.

```
for (시작; 조건식; 종료식;){
    실행문;
}
```

for 문은 예약어 뒤 소괄호안에 (식 , 변수선언) , 조건식 , 종료식이 한번에 들어간다.<br/>
중괄호에는 실행문이 들어간다.<br/>
식 형태만 봤을 때 굉장히 복잡해 보이지만 의외로 간단하다.<br/>
<br/>
아까 while 예약어를 이용해 1부터 100을 세는<br/>
코드를 작성해보았다.<br/>
똑같은 목적으로 이 코드를 출력하면 이러한 코드가 완성된다.

```
for(let i = 0; i < 100; i++){
    console.log(i+1)
}
```

![포문으로1부터100처음](https://github.com/user-attachments/assets/f236e75c-409f-43e8-bc74-99243b574467)

![포문으로1부터100끝](https://github.com/user-attachments/assets/65b4d161-1752-4169-8dc8-a60246497a2e)

출력 순서는<br/>

#### 1. 시작(식이나 변수 작성)
#### 2. 조건식
#### 3. 실행문
#### 4. 종료식

순으로 진행된다.<br/>
예약어 바로 뒤에 왠만한 코드가 다 들어가서<br/>
코드 배치가 훨씬 깔끔하다.<br/>
<br/>
이렇게 아까 while문으로 썼던 코드는<br/>
출력 값이 무언가 부자연스러웠지만<br/>
for문은 이러한 오류도 없다.<br/>
(그 원인을 몰라서 설명은 못 했다...)<br/>
<br/>
다음에는 함수에 관해 공부해보겠다.
