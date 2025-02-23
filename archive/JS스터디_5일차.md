## 변수(variable)
### 변수 - 변수의 개념
코딩을 하다보면 많은 값들을 저장해야하는 순간이 있다.<br/>
그러한 행위를 하기위해, '변수'라는 개념이 있다.<br/>
<br/>
변수는 특정 값을 저장하고 나중에 필요한 순간에 다시 끌어 쓸 수 있다.<br/>
변수를 만들기 위해 쓰는 키워드가 몇가지 있다.<br/>
js에서 쓰는 대표적인 변수 예약어는,<br/>
<br/>
(let , var , const)가 있다.<br/>
let , var는 변수를 만든 후, 변수 값을 재할당 할 수 있고,<br/>
const는 변수를 만든 후 변수 값을 재할당 할 수 없다.<br/>
<br/>
<br/>
<br/>

### 변수 - 선언(declaration)
변수를 만드는 과정을 '선언'이라고 한다.<br/>
먼저 첫번째로 let을 이용한 선언문을 작성해보자.

```
let hi = "Hello js!";
```
필자가 작성해본 변수 선언문이다.<br/>
변수를 선언할 때는<br/>
변수 선언 키워드 + 변수명 + "=" + 변수에 들어갈 값<br/>
순으로 입력한다.<br/>
<br/>
그리고 변수를 선언할 때 몇가지 주의할 점이 있는데,<br/>
#### 1 . 변수명은 숫자로 시작할 수 없다.
#### 2. 변수명에는 기호 , 마침표 , 공백이 포함될 수 없다.
#### 3. 변수명은 예약어를 사용 할 수 없다.(for , true , false 등
#### 자바스크립트에서 특정한 역할을 하는 언어)
<br/>
<br/>

위에 작성한 코드는 'let'연산자를 이용하여,<br/>
변수명은 hi로 하고, hi에 "Hello js!"라는 값을 저장한 선언문이다.<br/>
let과 var는 거의 비슷한 개념이지만, var를 이용하여<br/>
변수를 선언한 코드를 변수문이라고 한다.<br/>

![hi변수선언및출력](https://github.com/user-attachments/assets/4095e6de-2c4e-4133-85d1-f0224e00e628)

위 사진처럼, 변수 hi를 선언하고 hi를 콘솔에 입력했을 때,<br/>
hi에 저장한 "Hello js!"가 출력된 모습을 볼 수 있다.<br/>
<br/>
<br/>
<br/>

### 변수 - 변수 값 변경

let , var로 선언한 변수는 변수의 값을 변경하는 것이 가능하다.

![let으로 hi변경하기](https://github.com/user-attachments/assets/5b647882-1f27-4ea2-ab35-821f9c83326b)

![var으로 jsgood변경하기](https://github.com/user-attachments/assets/23bd9c2b-efe7-42fc-a63e-ad3d924e1d9f)

이처럼 let 과 var는 변수 값을 변수명 입력후 바로 대입하여<br/>
중간에 변경 하는것이 가능하다.<br/>
<br/>
하지만 const 키워드는 중간에 변수명에 다른 변수 값을 대입하여<br/>
변수 값을 바꾸는 것이 불가능하다.<br/>

![const로 bye 변경하기](https://github.com/user-attachments/assets/e3adcc44-943c-459c-9dac-2b4889f7202a)

변수를 선언하고, 변수를 다른 변수에 대입하는 것도 가능하다.<br/>
예를 들면,<br/>
철수의 몸무게는 97kg이고,<br/>
영희의 몸무게는 45kg이다.<br/>
변수에도 각각의 몸무게를 정확히 기재하고 출력하였다.<br/>

![철수와영희](https://github.com/user-attachments/assets/cbf11c4b-2573-4c1d-97a2-02a67a4d28b7)

이 값을 바꿔치기 해볼 것이다.<br/>

![철수몸무게의영희](https://github.com/user-attachments/assets/9a308601-e713-455e-b733-4ef45165882f)

이렇게 졸지에 영희는 철수의 몸무게를 가져버린 것이다.<br/>
<br/>

그리고 영희의 몸무게를 뻥튀기 시킬 수도 있다.<br/>
변수명을 '영희몸무게' , '철수몸무게' 로 수정하여 구해볼 것이다.<br/>


```
let 영희몸무게 = 45
```

```
let 철수 몸무게 = 97
```

그리고 영희 몸무게에 몸무게를 추가하였다.

![영희몸무게뻥튀기](https://github.com/user-attachments/assets/4db4498c-1e37-45f0-a34c-73ee97788f17)

변수 값이 잘 변경되었다.<br/>
<br/>
<br/>

### 변수 - let과 var

const는 바꿀 수 없는 변수를 만드는 예약어이다.<br/>
나머지 let , var는 중간에 변수 값을 바꿀 수 있다는 공통점이 있다.<br/>
<br/>
그렇다면 let과 var는 어떤점이 다른걸까?<br/>
<br/>
앞서 말한 변수명의 규칙에서는<br/>
예약어를 변수명으로 사용할 수 없었다.<br/>
하지만 var를 이용하여 변수 선언을 하면<br/>
예약어를 변수명으로 써도 에러가 발생하지 않는다.<br/>

![var예약어변수명](https://github.com/user-attachments/assets/2d338e8b-e974-4f2c-97a1-8f50e2e9de25)

<br/>
하지만 예약어를 변수명으로 사용하여 코딩을 한다면,<br/>
다른 개발자가 보기에 헷갈릴 수 있다.<br/>
<br/>

![let예약어변수명](https://github.com/user-attachments/assets/76b0f3ed-d643-47e9-87f7-b54cdfdb35c4)

let은 예약어를 변수명으로 사용하면 에러를 띄워<br/>
이러한 상황을 막아준다.
<br/>
<br/>
<br/>


## 상수(constant)

앞서 배운 '변수'는 변하는 수였지만, 이번에 배울 '상수'는 변하지 않는 수이다.<br/>
변수 선언때는 예약어 let을 사용하여 작성했지만<br/>
이번에는 상수의 특성을 가진 예약어 const를 이용하여<br/>
상수를 작성해볼 것이다.<br/>
<br/>
const는 상수의 특성을 가지고 있지만,<br/>
상수가 아니고 변수에 속한다.<br/>
<br/>
<br/>
<br/>
다음에는 조건문을 배워볼 것이다.
