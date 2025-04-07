# 리눅스 가상머신 사용
## 우분투
오늘 리눅스 운영체제를 실습해보기 위해<br/>
'우분투'라는 가상머신을 사용해 볼 것이다.<br/>
<br/>

![리눅스로고](https://github.com/user-attachments/assets/c1d4a225-f49c-444c-bec2-309ecd378195)

<br/>
<br/>

## Copyright(저작권)

보통 홈페이지나, 회사의 저작물들을 보면,<br/>
"Copyright" 라는 단어를 볼 수 있다.<br/>
이는, 저작권이라는 뜻인데,<br/>
<br/>
저작권은 만든이의 권리를 보호하며<br/>
문화를 발전시키는 법이다.<br/>
<br/>
어떤 사람이 무언갈 만들고,<br/>
그것에 관한 지식 재산권을 부여한다.<br/>
<br/>
그렇게 저작권이 주어졌을 때,<br/>

![저작권사기](https://github.com/user-attachments/assets/3c2a7a18-9ee6-4fa9-9df4-80c71dd9a04b)


저작물을 타인이 사용할 때, 그에 대한 비용을<br/>
지불하고 사용하여야 한다.<br/>
<br/>
<br/>
<br/>

## 리누스 토르발즈와 Copyleft.

이러한 저작권에 관한 법에 불만을 가진<br/>
"리누스 토르발즈" 라는 사람이,<br/>
저작물에 관한 새로운 법을 주장하여<br/>
미국 법에 등록시킨다.<br/>
<br/>
Copyright에서 right만 left로 바꿔 법을 만들었다.<br/>
(심지어 right뜻이 오른쪽이 아님.)<br/>
<br/>
Copyright는 창작물에 관한 권리를 보호한다면,<br/>
Copyleft는 창작물은 뭐든 공유해야한다는 법이다.<br/>
<br/>
이러한 법을 만든 이유가 나름 있다.<br/>

```
인간의 자산인 지식과 정보는 소수만 독점하면 안된다.
```
라는데, 필자는 나름 멋지다고 생각한다.<br/>

## Copyleft를 따르는 리눅스

리눅스 운영체제는 이 법을 따르고 있는데,<br/>
그 덕분에 소스코드가 오픈소스이다.<br/>
<br/>
그래서 여러 곳에서 리눅스의 배포판이 많이 나오고 있다.<br/>
Red Hat, CentOS, Debian, Fedora, Linux Mint 등이 있는데,<br/>
<br/>

![우분투로고](https://github.com/user-attachments/assets/bd0e11c0-41fa-426f-a0a4-5e5b3501620a)

<br/>
<br/>
오늘 배울 우분투도 이 배포판중 하나이다.<br/>
지금부터 우분투 설치 후 환경 설정을 해보자.
<br/>

## Ubuntu 설치

```
https://ubuntu.com/download
```
이 링크로 접속하면 우분투 홈페이지로 넘어가게된다.<br/>
<br/>

![우분투데탑](https://github.com/user-attachments/assets/9496edbc-777b-4520-b78a-d3d51961a590)

필자는 윈도우11 운영체제를 사용하고 있다.<br/>
<br/>
사진 속에서는 데스크탑용이라고 써있지만,<br/>
필자는 노트북을 사용하며 이 버전을 다운받아써도<br/>
문제 없이 잘 돌아가고 있다.<br/>
<br/>
각자의 운영체제를 파악한 후 다운로드 하도록 하자.<br/>

## Ubuntu 의 정규버전과 LTS

![우분투LTS](https://github.com/user-attachments/assets/2791403b-e09c-4838-8d08-c773a57d12ba)


(Ubuntu 24.04.2 LTS 버전)<br/>
24년 4월에 출시된 장기 지원 버전이다.<br/>


![그냥우분투](https://github.com/user-attachments/assets/6c9f2b9b-9f6b-4147-a9d9-5d6eb4383ebe)

(Ubuntu 24.10 버전)<br/>
24년 10월에 출시된 정규 버전이다.<br/>
<br/>
다운로드 버튼을 누르면 이렇게 두 가지 버전이 있다.<br/>
LTS냐, 정규 버전이냐 차인데<br/>
어떤 차이인지 알아보도록 하자.<br/>
<br/>
<br/>

``
LTS : Long Term Support
``
<br/>
LTS 버전은 단어 뜻 처럼<br/>
'장기 지원' 버전이다.<br/>
<br/>

먼저 LTS 가 붙지 않은 '정규 버전'을 알아보도록 하겠다.<br/>
정규 버전은 6개월마다 신 버전을 배포하며,<br/>
배포일로부터 9개월간 업데이트를 지원한다.<br/>
<br/>
이제 LTS가 붙은 '장기 지원 버전'을 알아보도록 하겠다.<br/>
장기 지원 버전은 2년마다 새로운 버전을 배포하며,<br/>
업데이트는 배포일로부터 5년동안 지원한다.<br/>
<br/>
<br/>

## 버전을 나눈 이유 및 특징

알다시피 리눅스는 '리누스 토발즈'라는 사람에 의해 개발되었다.<br/>
이 개발자는 리눅스를 만듦과 동시에 'Copyleft'법을<br/>
널리 전파하여 오픈소스 문화를 만든 장본인이기도 하다.<br/>
<br/>
많은 사람들이 리눅스의 보안이 좋다고 하는데,<br/>
리눅스라는 운영체제의 소스코드는 오픈되어 있어서,<br/>
해커들에게도 노출되어 더 위험할 수 있는 시스템이다.<br/>
<br/>
그러나 해커들의 공격에도 윈도우보다 더 보안이 철저할 수 있는 이유는,<br/>
리눅스의 시스템을 유지보수하는 전세계의 수많은 개발자가 있기 때문.<br/>
<br/>

![블랙해커](https://github.com/user-attachments/assets/97cbc10f-216c-409e-aa52-dce0af896d19)

아무리 해커들이 오픈소스의 운영체제를 노려<br/>
나쁜 짓을 하려고 해도,<br/>
<br/>

![개발자들](https://github.com/user-attachments/assets/4f069314-6901-4d4b-a388-35d6299dfda6)

전 세계의 수많은 개발자들 앞에서는 어림 없다.<br/>
<br/>
그래서 리눅스는 보안이 중요한 서버컴퓨터 등에 널리 쓰인다.


![서버실](https://github.com/user-attachments/assets/cf5b9c61-3d88-4123-98d9-22aa6dd5fd96)

LTS 가 쓰이는 컴퓨터는 주로 서버 컴퓨터이다.<br/>
<br/>
정규 버전과 LTS는 각각 장점이 있는데,<br/>
LTS는 새로운 기능을 쓰기엔 오랜 시간이 걸리지만,<br/>
버그 및 크래시 수정이 빠르고, 그만큼 보안 패치도 빠르다.<br/>
그래서 LTS버전은 안정적으로 쓸 수 있다.<br/>
<br/>
<br/>

정규 버전은 리눅스의 새로운 기능을 쓰고 싶어하는<br/>
개인 데스크탑을 사용하는 개발자들에게 인기가 좋다.<br/>
<br/>
비록 업데이트 기간은 9개월로 매우 짧지만,<br/>
새로운 기능을 빨리 접할 수 있기에<br/>
데스크탑 이용자들에게 인기가 좋다.<br/>
<br/>
<br/>
정규버전이나 LTS 중 하나를 고르고<br/>
다운로드를 누르면, 약 5GB정도되는 실행 파일이 설치된다.<br/>
<br/>
설치하는데 생각보다 오래 걸리니,<br/>
눌러놓고 커피한잔하고 오자.<br/>
<br/>

## VirtualBox 설치

이제 이 iso 파일을 VirtualBox 로 실행해보겠다.<br/>
<br/>
<b>오라클</b>에서 배포중인 가상머신 소프트웨어이다.

<i>https://www.virtualbox.org/wiki/Downloads</i><br/>
<br/>
이 링크로 접속하면 이러한 화면이 뜬다.<br/>

![버추얼홈피전체](https://github.com/user-attachments/assets/c2796a28-6b36-4179-8167-3031bef99005)

여기서 왼쪽 밑 운영체제별 다운로드 양식이 뜨는데,<br/>

![버추얼홈피양식](https://github.com/user-attachments/assets/9ceb58eb-3485-4ade-9c6f-ab2d8c7a3d41)

각자의 운영체제에 맞춰 다운로드 하면 된다.<br/>
다운로드 후에 exe 파일을 실행시키면,<br/>

![버추얼1](https://github.com/user-attachments/assets/df0a1554-38df-417b-815b-f52cdcfdf3a4)

창이 열린다. next를 누른다.<br/>
<br/>
<br/>
<br/>

![버추얼2](https://github.com/user-attachments/assets/0654cbe6-f917-4c9f-91cf-9888707717dd)

사용자 약관 동의 후 다음으로 넘어간다.<br/>
<br/>
<br/>
<br/>

![버추얼3](https://github.com/user-attachments/assets/5c9df834-9871-434c-81aa-160e63f0fd8d)

기본세팅 건들지 말고 넘어간다.<br/>
<br/>
<br/>
<br/>

![버추얼4(네트워크 리셋)](https://github.com/user-attachments/assets/54822009-c201-4c59-a44b-188cf1594ecc)

빨간 글씨로 네트워크가 리셋된다고 나오지만 넘어간다.<br/>
<br/>
<br/>
<br/>

![버추얼5](https://github.com/user-attachments/assets/03fad3fd-6b0e-40a3-aad1-cca1eab37819)

의존성 프로그램 Python Core와 win32api 가 없다고 뜬다.<br/>
계속 넘어간다.<br/>
<br/>
<br/>
<br/>

![버추얼6](https://github.com/user-attachments/assets/1ac91b72-f692-41ba-ad46-c995e40bffd6)

바탕화면 아이콘 등 편한대로 선택하면 된다.<br/>
대신 맨 밑 항목은 꼭 체크한다.<br/>
<br/>
<i><b>Register File Associations : 파일 연결을 등록하는 작업.</i></b><br/>
<br/>
<br/>
<br/>

![버추얼7(설치중)](https://github.com/user-attachments/assets/c958c066-26e3-4f41-87b6-939c67c782f8)

설치 중

![버추얼컴플리트](https://github.com/user-attachments/assets/f5e25cf9-9fea-4140-b2fb-508cff7d756b)

쭈욱 next , install 만 누르면 이렇게<br/>
설치가 완료된다.<br/>
<br/>
<br/>

이제 실행시켜보자.<br/>
<br/>



