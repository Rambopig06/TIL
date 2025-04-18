# 자료형
## 문자열과 숫자열의 계산
```
'3'+14
```
문자열과 숫자열을 이렇게 합치면 과연 값이 성립될까?

![3플러스14](https://github.com/user-attachments/assets/279afe40-f1cc-4259-bfed-46fff032ba11)

놀랍게도 성립된다.<br/>
하지만 이것은 숫자열이 아니다.<br/>
3 + 14는 17이 나와야 하는데, '314' 가 출력된다.<br/>
<br/>
이 명령어가 구동되는 원리는<br/>
숫자열을 문자열로 변환된 후 계산된 값을 띄우는 것이다.<br/>
<br/>
이러한 과정을 "형 변환(Typecasting)" 이라고 한다.<br/>
그렇다면 아예 정수가 아닌 문자열을 입력후 숫자를 더해보자.<br/>

![문자플러스14](https://github.com/user-attachments/assets/e1a79b7f-4500-4c54-9478-d3f850350c90)

이렇게 '문자14'로 출력된다.<br/>
더하기를 할 때는 문자열이 숫자보다 우선순위가 높다는걸 기억하자.<br/>
<br/>
반대로 서로다른 자료형끼리 뺄셈을 시켜보면,

![3마이너스14](https://github.com/user-attachments/assets/44cd61e3-79a1-4d76-8b9f-83fae603dad0)

이렇게 문자열이었던 '3'이 숫자로 바뀌고,<br/>
3 - 14 = -11 로 성립된다.<br/>
똑같이 형 변환이 일어나지만 빼기를 할땐, 숫자가 문자열보다 우선순위가 높다.<br/>
<br/>
그렇다면 정수가 아닌 문자열과 숫자끼리 뺄셈은 어떻게 이루어질까?

![문자마이너스14](https://github.com/user-attachments/assets/b0ad0501-5c5f-4256-9353-cb3f1860a905)

식이 성립되지 않고 NaN(숫자가 아님) 이라는 오류를 출력한다.<br/>
'문자'라는 문자열이 숫자로 바뀔 때, 이미 NaN으로 바뀌기 때문에,<br/>
식을 계산할 수가 없게 된다.

<br/>
<br/>
<br/>
<br/>

## 불 값
활활 타오르는 그 불 아니다.<br/>
<br/>
이 자료형은 true와 false를 나타내는 불 값(boolean)이다.<br/>
영국의 수학자 조지 불(George Boole)에서 따온 이름이다.<br/>
<br/>
불 값은 따옴표로 감싸지 않고 그냥 입력해야<br/>
온전한 불 값으로 나타낼 수 있다.<br/>
따옴표로 감싸면 그냥 문자열이 될 뿐이다.

![불 값 스트링](https://github.com/user-attachments/assets/53eb22c8-558e-4923-9c16-72e057d54d18)

이렇게 말이다.<br/>
<br/>
그렇다면 온전히 불 값의 자료형을 구하는 명령어를 콘솔에 쓰면<br/>
뭐라고 출력할까?<br/>

![불 값 불린](https://github.com/user-attachments/assets/c1d672a5-283f-4eee-8b1c-366fdbe89ecf)

'boolean' 자료형 이라는 것을 출력한다.<br/>
<br/>

true는 참 , false는 거짓인데,<br/>
이러한 불 값을 이용하여, 맞는식과 틀린식을 구분할 수 있다.<br/>

<br/>
<br/>
<br/>
<br/>

## 불 값 - 비교연산자 사용

```
3>1
```
3과 1을 비교하여 3이 크다고 식을 작성하였다.<br/>
맞는말이다.<br/>

![3과1트루](https://github.com/user-attachments/assets/f7aaa0fa-0ea0-4592-8e14-2ab8a896f785)

맞는 식 이므로 콘솔에서 true를 출력한다.

```
3<1
```

이번에는 3이 1보다 작다는 식을 콘솔에 작성하니<br/>

![3과1펄스](https://github.com/user-attachments/assets/89eef120-f169-4a83-8b1a-afd7f9c65186)

틀린 식 이므로 false를 출력한다.<br/>
<br/>

```
3 == 3
```
3과 3의 일치 여부를 보는 식이다.

![3는는3](https://github.com/user-attachments/assets/5217f9c0-0b9b-47e1-bce4-6544b77ea736)

성립되므로 true 출력.<br/>
<br/>
<br/>
```
'3' == 3;
```
이번에는 서로 다른 자료형끼리 붙여서<br/>
비교해 보았다.<br/>
결과는 어떨까<br/>

![문자3는는3](https://github.com/user-attachments/assets/9e21a4c7-e799-4977-a97a-0117c52d3621)

서로 다른 자료형을 비교하는데 true로 성립된다.<br/>


<br/>

```
3 != 3
```
이 식은 무엇일까..

![3!는3](https://github.com/user-attachments/assets/aab1db8b-5fc5-46cc-b1da-9be97c9942d2)

성립되지 않아 false를 출력한다.<br/>
== 는 양쪽의 값이 같으면 true를 출력하고,<br/>
!= 는 양쪽의 값이 다르면 true를 출력하는 청개구리같은 존재다.<br/>
<br/>

```
3 >= 1
```
이 식은 3이 1이상의 값이면 성립되는 식이다.<br/>

![3왼는1](https://github.com/user-attachments/assets/51250191-b21e-4846-9c73-677a4e12293a)

성립되므로 true 출력.<br/>
<br/>

```
3 <= 1
```
이 식은 3이 1이하일 때 성립되는 식이다.<br/>

![3오는1](https://github.com/user-attachments/assets/8070a266-3da2-4073-9602-7b699e577db5)

성립되지 않으므로 false가 출력된다.<br/>
<br/>
<br/>
<br/>

## NaN == NaN

이번에도 NaN은 신선한 충격을 가져다준다.

![NaN는는NaN](https://github.com/user-attachments/assets/ab1e5b0c-0a47-41db-a68e-511d41af5a5d)

양쪽이 모두 NaN으로 같지만, 식이 성립되지 않는다.<br/>
NaN은 비교연산에서 false를 출력한다고 알면된다.<br/>
하지만 != 를 썼을 때는 true가 출력된다.<br/>
<br/>
<br/>
<br/>

## 문자열의 비교

```
true > false
```
불 값인 true와 false 를 비교한 식이다.

![트루와펄스](https://github.com/user-attachments/assets/0bf35ca0-5d17-45c7-a89b-ed192e5ed9f9)

식이 성립되어 true가 나온다.<br/>
true가 false보다 큰 값이라는걸 외워두자.<br/>
<br/>
그렇다면, 일반 문자열끼리도 비교가 될까?
<br/>

```
'a' > 'b'
```
식이 성립되지 않아서

![a왼b](https://github.com/user-attachments/assets/95b929ad-69e8-4ed0-8bba-ee0e1943adf7)

false가 출력된다.<br/>
문자열은 문자의 번호를 따른다.<br/>
알파벳은 a\~z까지 차례대로 세고,<br/>
한글은 ㄱ~ㅎ 까지 차례대로 센다.<br/>
<br/>
학교를 다닐때, ㄱ을 가진 성을을 쓰는 친구들이<br/>
출석번호가 빠른 걸 생각하면 이해하기 쉽다.<br/>
<br/>
<br/>
<br/>

## 문자의 번호를 알고 싶을 때
콘솔창에 'charCodeAt' 을 쓰면 된다.<br/>
알고 싶은 문자를 먼저 쓰고, .charCodeAt(); 을 붙이면 된다.

```
'하'.charCodeAt();
```
이런식으로 콘솔에 작성 후, 실행시키면

![하코드](https://github.com/user-attachments/assets/824ce770-6e89-42af-a063-d766f0e4af41)

54616이라는 번호를 출력한다.<br/>
이것이 '하'라는 문자의 고유번호이다.<br/>

<br/>
<br/>
<br/>
<br/>

## 문자열과 숫자열의 비교

```
'3' > 14
```
이것을 계산했을 때 어떻게 출력될까?<br/>

![문자3왼14](https://github.com/user-attachments/assets/f88c46e2-f91e-403b-ad24-3ca7b80fb9fb)

서로 다른 자료형을 비교할 때,<br/>
빼기와 똑같이 숫자열 자료형이 우선시 되어<br/>
문자열이 숫자로 바뀐후 비교된다.<br/>
<br/>
3보다 14가 크므로 이 식은 성립되지 않는다.<br/>
<br/>

```
'math' > 314
```
이번엔 정수가 아닌 문자열을 숫자와 비교하는 식을 작성하였다.<br/>
당연히 'math'는 숫자가 아니므로,<br/>
연산도중 math가 NaN으로 변하고,<br/>
NaN의 비교는 false이므로 식이 성립되지 않아서

![매쓰왼314](https://github.com/user-attachments/assets/33354eea-90be-4494-8dba-aea58f498354)

false가 출력된다.<br/>

![매쓰오314](https://github.com/user-attachments/assets/7121b0b4-904a-444f-a9be-c73693a713c4)

반대의 경우도 마찬가지로 false가 출력된다. <br/>
각 열의 대소관계와 상관없이, 비교 자체가 성립되지 않아서 나오는 결과다.<br/>
<br/>
<br/>
<br/>
<br/>

## 조금 더 깐깐한 비교 연산자( === , !== )

아까까지 배웠던 비교 연산자는 기호를 1개나 2개만 사용하여<br/>
각 열을 비교하였다. 다만 어떤 상황에서는<br/>
문자열 -> 숫자열<br/>
숫자열 -> 문자열<br/>
이런식으로 형 변환이 이루어져서 원치않는 결과가 나오기도 하였다.<br/>
<br/>
이젠 === , !== 를 배워볼 것이다.<br/>

```
'3' === 3;
```

아까 '3' == 3; 의 식에서<br/>
true가 출력되었다.<br/>
이번에는 어떨까.

![문자3는는는3](https://github.com/user-attachments/assets/c1729b95-561d-43ff-ba0d-b7fc31e3c35b)

식이 성립되지 않아서 false가 출력되었다.<br/>
이 연산자는 각 열의 대소관계 및 자료형의 일치 유무까지 보기 때문에,<br/>
==와 달리 자료형이 같이 같은 위의 식에 false를 출력한 것이다.<br/>
<br/>
```
'3' !== 3;
```
위에서 썼던 === 는 자료형과 각 열의 대소유무의 참을을 보는 연산자였지만,<br/>
이 연산자는 자료형 , 열의 대소유무의 거짓을 보는 연산자이다.
<br/>
<br/>
<br/>
<br/>

## 논리 연산자 사용 ( && : AND )

이번에 알아볼 연산자는 && 이다.<br/>
'그리고' 라는 뜻인데,<br/>
두 열의 참과 거짓여부가 모두 참이여야 성립된다.<br/>

```
3>1 && 8>6;
```

3>1 은 참이고, 8>6도 참이다.<br/>
두 열의 참과 거짓여부가 동시에 맞아야<br/>
식이 성립되어 true가 출력된다.<br/>
<br/>
```
3>1 && 8<6;
```

3>1은 참이고, 8<6은 거짓이다.<br/>
두 열의 참이 동시에 참이여야 true가 성립된다.<br/>
왼쪽의 열은 참이지만 , 오른쪽 열은 거짓이기 때문에,<br/>
식이 성립되지 않으므로 false가 출력된다.<br/>
<br/>
<br/>
<br/>
<br/>

## 논리 연산자 사용 ( | | : OR )

```
3>1 || 8<6;
```
이번에 알아볼 연산자는 | | 이다.<br/>
'또는' 이라는 뜻 인데,<br/>
위의 식에서 3>1은 참이고, 8<6은 거짓이다.<br/>
하지만 이 연산자는 두 열중 하나만 참이어도 성립되는 연산자이다.<br/>

```
3<1 || 8<6;
```
이 식은 성립이 될까?<br/>
양쪽의 열이 둘 다 거짓일 경우,<br/>
식이 성립되지 않아 이 식은 false가 출력된다.<br/>
<br/>
다음에는 변수를 알아볼 예정이다.









