## 리눅스 명령어
오늘 배워볼 내용은 리눅스의 명령어다.<br/>
이 명령어들은 'Visual Studio code'에서 학습해 볼 것이다.<br/>
<br/>
오늘도 역시 철수와 영희를 이용한다.<br/>
<br/>
먼저, 이 블로그를 보는 사람들은 폴더와 파일의 정의를<br/>
당연히 알거라 생각 되지만, 그래도 간략하게 짚고 넘어가겠다.<br/>

(폴더)

폴더는 비유를 하자면, 학창시절 학습지같은거 모아두는<br/>
이러한 책을 생각하면 된다. 즉, 파일을 모아두는 것.<br/>

(파일)

위에 비유했던 학습지는 파일에 해당한다.<br/>
컴퓨터에서 파일은, 의미가 있는 정보를 담는 논리적인 단위이다.<br/>
<br/>
이제 VS code를 실행시켜서 터미널을 이용하여<br/>
폴더와 파일 생성 , 삭제 , 편집을 공부해 볼 것 이다.<br/>
<br/>
먼저 'Terminal'을 누른 뒤 'New Terminal'을 눌러<br/>
터미널 이라는 것을 띄운다.<br/>
<br/>
VS code에서 터미널은 '현재 작업중인 폴더에서' 명령어를 입력할 수 있는 창이다.<br/>
이 터미널이라는 곳에서 현재 위치를 알 수 있고, 파일이나 폴더를 편집할 수 있다.<br/>
<br/>
우리가 오늘 배울 명령어는 '리눅스'라는 운영체제의 명령어이므로,<br/>
리눅스 명령어를 사용하기 위해선 그에 맞는 '쉘 프로그램'을 써야한다.<br/>

#### 쉘 프로그램 - 명령어를 운영체제에 전달하여,
#### 그에 맞는 언어로 구동되게 하는 프로그램이다.

<br/>
<br/>
VS code 에서 터미널을 띄울 때 여러 옵션이 있는데,<br/>
우리는 'git bash' 라는 프로그램을 띄울 것이다.<br/>
<br/>
bash는 Bourne Again Shell의 줄임말로, 유닉스 쉘 프로그램 sh의 확장판이다.<br/>
유닉스가 갑자기 왜 나오냐고 하면,<br/>
간단하게 리눅스의 조상이 유닉스라는 언어이다.<br/>
<br/>
자세한건 추후 다른 블로그에서 서술하겠다.<br/>
<br/>

(깃배시)

이렇게 git bash 를 띄운다.<br/>
<br/>
<br/>
<br/>
<br/>

### 폴더 생성 - mkdir(make directory)


터미널을 띄우고 mkdir를 입력, 띄어쓰기 한번 하여<br/>
내가 원하는 이름의 폴더를 생성한다.<br/>

```
mkdir school
```
이 명령어를 입력하여 school이라는 폴더를 생성하였다.

(mkdir)

<br/>
<br/>
<br/>
<br/>

### 파일 생성 - touch

폴더를 생성했으면 이제 파일을 생성할 차례다.<br/>
메모장 파일을 생성할건데,<br/>
파일을 만들 땐, '확장자'라는 개념을 같이 설정해야한다.<br/>
<br/>
확장자는 파일이름 뒤에 파일의 종류를 나타내는 문자열을 같이 적는다.<br/>
ex ) index.html , readme.md , 교수님 말씀.txt <br/>
이제 본격적으로 파일을 생성해보려한다.<br/>

```
touch index.html
```

이 명령어를 사용하면 index.html라는 파일을 생성한다.<br/>
하지만 터미널은 '현재 작업중인 위치'에서 폴더,파일을 편집하는 공간이므로,<br/>
아까 만들어놓은 school 이라는 폴더안에 만들고 싶다면,<br/>
cd 라는 명령어를 사용하여야 한다.<br/>

#### cd - change directory 

cd 의 풀네임대로 폴더를 바꾼다라는 뜻이 있는 명령어인데,<br/>
현재 작업중인 폴더에서 cd 뒤에 부가적으로 붙은 명령어를 이용하여<br/>
작업 위치를 이동할 수 있다.<br/>

```
cd school
```
cd를 작성, 띄어쓰기 후 이동하고싶은 위치 (school)를 적으면,<br/>

(school로 이동)

이렇게 현재 작업하는 위치가 school로 이동한걸 볼 수 있다.<br/>
이제, 여기에 파일생성 코드를 입력하면,<br/>

(index생성)

index.html 파일이 school 폴더안에 성공적으로 만들어진걸 볼 수 있다.<br/>
(미완성)
### 

















