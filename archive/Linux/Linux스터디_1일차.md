## 리눅스 명령어
오늘 배워볼 내용은 리눅스의 명령어다.<br/>
이 명령어들은 'Visual Studio code'에서 학습해 볼 것이다.<br/>
<br/>
오늘도 역시 철수와 영희를 이용한다.<br/>
<br/>
먼저, 이 블로그를 보는 사람들은 폴더와 파일의 정의를<br/>
당연히 알거라 생각 되지만, 그래도 간략하게 짚고 넘어가겠다.<br/>

![폴더](https://github.com/user-attachments/assets/d49b9a21-c974-44bd-ab4e-49670c9edd24)

폴더는 비유를 하자면, 학창시절 학습지같은거 모아두는<br/>
이러한 책을 생각하면 된다. 즉, 파일을 모아두는 것.<br/>

![파일](https://github.com/user-attachments/assets/fcef2a18-72c3-4b0f-b367-266844599373)

위에 비유했던 학습지는 파일에 해당한다.<br/>
컴퓨터에서 파일은, 의미가 있는 정보를 담는 논리적인 단위이다.<br/>
<br/>
이제 VS code를 실행시켜서 터미널을 이용하여<br/>
폴더와 파일 생성 , 삭제 , 편집을 공부해 볼 것 이다.<br/>
<br/>
VS code 프로그램 설치법까지 알려주기엔 너무 내용이 길어지니<br/>
각자 능력껏 프로그램을 설치하고 오길 바란다.<br/>

![vs코드 첫 실행](https://github.com/user-attachments/assets/542c9489-dc5f-4116-bae4-11b82457e6fb)

설치 완료 후 실행시키면 이러한 화면이 뜨는데,<br/>
잘 뜨면 이어서 작업하면 된다.<br/>
<br/>
먼저 'Terminal'을 누른 뒤 'New Terminal'을 눌러<br/>
터미널 이라는 것을 띄운다.<br/>

![터미널 띄움](https://github.com/user-attachments/assets/82d66235-ff3e-4ad3-abd1-7842ab9b8b6d)


<br/>
VS code에서 터미널은 '현재 작업중인 폴더에서' 명령어를 입력할 수 있는 창이다.<br/>
이 터미널이라는 곳에서 현재 위치를 알 수 있고, 파일이나 폴더를 편집할 수 있다.<br/>
<br/>
우리가 오늘 배울 명령어는 '리눅스'라는 운영체제의 명령어이므로,<br/>
리눅스 명령어를 사용하기 위해선 그에 맞는 '쉘 프로그램'을 써야한다.<br/>

#### 쉘 프로그램 - 명령어를 운영체제에 전달하여,
#### 그에 맞는 언어로 구동되게 하는 프로그램이다.

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

![터미널 띄움](https://github.com/user-attachments/assets/82d66235-ff3e-4ad3-abd1-7842ab9b8b6d)


터미널 오른쪽 위 화살표를 눌러 'Git bash'를 클릭하면,

![깃배시](https://github.com/user-attachments/assets/01f860b3-50c4-4e88-a3fa-11f608bbe2b4)

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

![mkdir명령](https://github.com/user-attachments/assets/d19be92b-1a81-4f4a-b0fb-391cb7266ab5)

터미널에 명령어 입력시,

![폴더생성큰화면](https://github.com/user-attachments/assets/be4d6059-f4bc-4bc8-9860-b1f653829bd3)

school 이라는 폴더가 생성되었다<br/>\
<br/>
우리는 폴더 및 파일생성에 관해 배우므로,<br/>

![폴더생성작은화면](https://github.com/user-attachments/assets/7ec2a47d-4242-4f01-907f-40584c646ed9)

폴더 및 파일 리스트에 포커스를 맞춰 사진을 올려보겠다.

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
touch cs.txt
```
이 명령어는 철수의 생활기록부를 만드는 명령어다.<br/>
<br/>
대충 touch(파일생성 명령어) + cs(철수 영어이름 줄임말).txt<br/>
이렇게 알아들어주면 좋겠다.<br/>
본 글쓴이는 영어가 약한관계로 철수를 영어로 못쓴다.<br/>
<br/>
아무튼<br/>
<br/>
필자는 폴더 및 파일의 관계 컨셉을 학교와 학생으로 할 것이기 때문에,<br/>
시험삼아 철수,영희의 생활기록부를 만들어 볼 것이다.<br/>
<br/>
이 생활기록부도 학교와 관련된 물건이기 때문에,<br/>
컨셉에 충실하기위해 학교폴더안에 넣어볼 것이다.<br/>

하지만 터미널은 '현재 작업중인 위치'에서 폴더,파일을 편집하는 공간이므로,<br/>
아까 만들어놓은 school 이라는 폴더안에 만들고 싶다면,<br/>
cd(change directory) 라는 명령어를 사용하여야 한다.<br/>

```
cd school
```

![cd로 스쿨이동](https://github.com/user-attachments/assets/a5864720-5048-4606-94d7-0ca4210a7908)

이 명령어를 입력 후, 현재 경로에 school이 추가된걸 볼 수 있다.<br/>
change directory, 말 그대로 폴더를 바꾼다라는 뜻.<br/>
상위 폴더에서 하위 폴더나 파일로 내려가게 되는 것 이다.<br/>
반대로 돌아가고 싶을 땐,

```
cd ..
```

을 입력하면 상위 폴더로 이동한다.

아무튼 school 폴더로 이동했으므로 철수,영희 생기부를 만들어 보겠다.

![철수영희생기부GUI](https://github.com/user-attachments/assets/e789c347-f127-475a-ae69-7e2636a80d24)

GUI로 확인해 보았을 때, school폴더안에 두 파일이 잘 만들어진걸 볼 수 있다.<br/>
이 사실을 터미널에서 확인하는 방법이 있다.

<br/>
<br/>
<br/>
<br/>

### 현재 디렉토리의 파일이나 디렉토리 나열 - ls

아까 파일 제작이 잘 반영이 된걸 보기위해,<br/>
터미널에 ls를 입력하여 현재 디렉토리에 있는 내용을 조회해본다.

![스쿨내 ls](https://github.com/user-attachments/assets/70d286ee-2b2d-4369-a878-5f37432f0fa1)

이렇게 cs.txt , yh.txt이 출력된다.


