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

## 폴더 생성 - mkdir(make directory)


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

## 파일 생성 - touch

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

## 현재 디렉토리의 파일이나 디렉토리 나열 - ls

아까 파일 제작이 잘 반영이 된걸 보기위해,<br/>
터미널에 ls를 입력하여 현재 디렉토리에 있는 내용을 조회해본다.

![스쿨내 ls](https://github.com/user-attachments/assets/70d286ee-2b2d-4369-a878-5f37432f0fa1)

이렇게 cs.txt , yh.txt이 출력된다.


### 디렉토리,파일 상세히 나열 - ll

ls의 상휘호환이라고 할 수 있는 ll이라는 명령어를 공부해 볼 것이다.<br/>
<br/>
ll은 정식 명령어가 아닌, ( ls -l ) 명령어를 간략히 나타낸 명령어인데,<br/>
다른 터미널에서는 작동되지 않는 경우가 많으니,<br/>
ls -l 을 습관적으로 사용하는 것을 권장한다.<br/>
<br/>

![ll로 철수영희출력](https://github.com/user-attachments/assets/f23462f9-4c48-4341-9c55-a497a3a212e5)

<br/>


- 권한 : -rw-r--r--	파일 유형 및 접근 권한

- 링크 수 : 1	해당 파일이나 디렉토리에 연결된 하드 링크의 수
- 소유자 : min43	파일이나 디렉토리의 소유자 이름
- 그룹	: 197609	파일이나 디렉토리가 속한 그룹 이름
- 크기	: 0	파일의 크기(바이트 단위) 디렉토리의 경우 메타데이터 크기
- 수정 날짜 및 시간	: Mar 16 18:30	마지막으로 파일이나 디렉토리가 수정된 날짜와 시간
- 파일명 : cs.txt	파일이나 디렉토리의 이름
  


### 디렉토리 내 숨김 파일까지 띄우는 명령어 - ls -a

보안상 보여줄 수 없어 띄우지 않는 파일은<br/>
`ls -a` 를 이용해서 볼 수 있다.


<br/>
<br/>
<br/>
<br/>

### cat - 파일 내용 보기

일단, 이 명령어는 파일 내 내용을 출력하는 명령어이므로,<br/>
먼저 철수의 생기부 내용을 간략하게 입력하겠다.


![철수 생기부 작성](https://github.com/user-attachments/assets/64ef559f-b21e-456e-9366-97601fac2996)

현실에서 이런 생기부를 가지게된다면<br/>
상당히 문제가 되지만, 아무튼 이건 필자 상상으로 작성한<br/>
철수의 생기부다.<br/>
<br/>
이제 cs.txt 에 작성한 생기부 내용을 터미널에서 조회해보자.

```
cat cs.txt
```

![캣으로 철수보기](https://github.com/user-attachments/assets/c4ed04bd-d8cc-42ff-bfba-5c714a408521)

이렇게 cs.txt 내부에 있던 생기부 내용을<br/>
터미널에 출력하였다.

## head ,tail - 파일 내용 보기(처음부터 , 끝부터)

cat과 사용법은 똑같지만, 단어 뜻과 똑같이<br/>
head는 처음부터 출력 , tail은 끝부터 출력한다.<br/>
<br/>
하지만 몇줄을 출력하는지를 지정하지 않았다.<br/>
이럴 땐, 기본값인 10줄만큼 출력한다.

```
head cs.txt
```

![헤드로 철수보기](https://github.com/user-attachments/assets/00b030e4-0ec8-4201-8754-20e60384ecbe)

head를 사용하니, 철수 생기부 내용 10줄이 출력되었다.<br/>
이번엔 끝부터 보자.<br/>
<br/>
<br/>

```
tail cs.txt
```

![테일로 철수보기](https://github.com/user-attachments/assets/a3211bfd-6bb4-4e85-839e-502b5722141b)

이번엔 끝부터 10줄만큼 내용이 출력되었다.<br/>

<br/>
<br/>

이젠, 추가 옵션들에관해 알아보자.<br/>

```
head -n 5 cs.txt
```

head 명령어 뒤에 num을 줄인 n 앞에 - 를 붙여 표현한다.<br/>
그리고 몇줄을 출력할지 뒤에 숫자를 붙인다.<br/>
5 줄을 출력할것이므로 -n 5 로 입력하였다.<br/>
<br/>

![헤드5줄철수](https://github.com/user-attachments/assets/a0707cd8-de79-4bd4-abeb-c6d2eb385f78)

```
head cs.txt -n 5
```

이렇게 순서를 바꾸어 작성해도 코드는 잘 작동한다.<br/>

![헤드철수5줄](https://github.com/user-attachments/assets/e52fa870-5ebf-4f44-896f-eaea70b2b36b)

<br/>
<br/>

tail 명령어도 똑같은 원리로 구동된다.

```
tail -n 5 cs.txt
```

![테일5줄철수](https://github.com/user-attachments/assets/a54c13ad-605b-4623-a96f-ecfa870bd400)

이렇게 코드 끝부터 5줄이 출력되었다.<br/>

<br/>
<br/>
<br/>
<br/>

## 파일 이동 , 이름바꾸기 - mv

move의 줄임말은 mv 명령어이다.<br/>
<br/>
파일을 이동시키는 명령어인데,<br/>
파일을 이동시키기 전, 이름변경부터 해보겠다.<br/>
<br/>
생기부 내용대로 철수는 돈이 많으므로<br/>
부자를 의미하는 rich를 붙여보겠다.<br/>

```
mv cs.txt rich_cs.txt
```

![철수이름변경CLI](https://github.com/user-attachments/assets/e7ec6c40-bbef-44bf-b84a-e48088855c61)

이 명령어를 터미널에 입력하니, 생기부 파일 이름이<br/>

![철수이름변경GUI](https://github.com/user-attachments/assets/0847cd6d-5b76-4988-8228-087956ec5a11)

기본 cs.txt 이름에서 rich_cs.txt 로 성공적으로 변경되었다.<br/>
<br/>
mv (기존이름) (바꿀이름) 순으로 입력한다.<br/>
<br/>
<br/>
이제 이 파일을 이동시켜볼것이다.<br/>

```
mv rich_txt ../
```

경로를 설정할 때, 위치를 구별하는 기호는 / 인데,<br/>
school 폴더에서 쫓아내보기위해, 상위 폴더로 이동하는 .. 을 붙여<br/>
school보다 상위 폴더로 이동시켰다.

![부자철수퇴장](https://github.com/user-attachments/assets/1683d822-93a0-4285-81d7-8df3250f0eba)

![부자철수퇴장GUI](https://github.com/user-attachments/assets/df0cd9de-793b-4dff-b27d-438d7dee4182)

이제 쫓겨났던 불쌍한 철수의 생기부파일을 다시 school 폴더에 넣고<br/>
원래 이름으로 복귀시켜보겠다.<br/>
<br/>
그 전에, 현재 필자가 위치하는 폴더에선,<br/>
상위 폴더에 있는 철수를 구할 수 없으므로,

![철수를구하기위한cd](https://github.com/user-attachments/assets/f544b717-250e-4ad1-bf0f-df448d4e1f55)

이렇게 나도 상위폴더로 이동했다.<br/>
이제 철수를 구할 수 있는 위치다.

```
mv rich.txt school/cs.txt
```

![철수구하기CLI](https://github.com/user-attachments/assets/d3534831-f924-40f0-85b1-4156ddbc3c9c)

![철수구하기GUI](https://github.com/user-attachments/assets/346e6f55-c95c-407d-b990-211a906781bc)

이렇게 이름이 원래 cs.txt로 변경되고, school 폴더안으로 이동시켰다.<br/>
하지만 철수를 구하느라 내가 school 폴더안에 없다.<br/>
내 위치를 터미널에서 알기위한 명령어 하나만 배우고 넘어가자.<br/>

<br/>
<br/>
<br/>
<br/>

## 현재 경로 확인 - pwd

![현재경로확인](https://github.com/user-attachments/assets/5a56fc86-d0a1-4c63-9fd6-7a2287be61d9)

이 명령어는 터미널에 pwd만 입력하면 현재 작업중인 위치를 볼 수 있다.<br/>
<br/>
다시 철수 , 영희의 파일을 수정하기위해, school 폴더로 넘어간다.

![cd후school이동후pwd](https://github.com/user-attachments/assets/18816741-ab60-40b8-89eb-c86387a3ef3c)

이제 철수와 영희를 괴롭힐 준비가 완료됐다.<br/>
<br/>
<br/>
<br/>
<br/>

## 파일 편집기 - vi

```
vi cs.txt
```

이 명령어를 입력하면 터미널에 굉장히 무서운 무언가가 실행되는데<br/>
여기서 파일내용을 수정 할 수 있다.<br/>
<br/>

![vi철수에게1](https://github.com/user-attachments/assets/3d27f171-6671-435e-8a06-f5ad7484322a)

이런 터미널형태가 된다면 성공이다.<br/>
이제 편집을 하기 위해 누르는 다양한 단축키들이 있지만,<br/>
필자는 i 를 제일 많이 누르므로 이걸로 실습해보자.

<br/>
<br/>
<br/>

![vi철수에게2(i누름)](https://github.com/user-attachments/assets/609056bf-c3c5-42c7-a9b4-6d74db5d847b)

i 를 누르니, 터미널 맨 밑줄에  'INSERT' 가 뜬다.<br/>
이제 화살표를 이용해 내가 원하는 내용을 수정하면 된다.

<br/>
<br/>
<br/>

![vi철수에게3(i누르고 수정)](https://github.com/user-attachments/assets/398ffe30-d4a8-4035-8ae4-db281debc446)

내용 편집이 완료됐다. 더욱 사악한 생기부가 완성되었다.<br/>
이제 편집기에서 탈출해보자.

<br/>
<br/>
<br/>

![vi철수에게4(esc누름)](https://github.com/user-attachments/assets/2e7b31dd-ae15-4705-9658-34478cbd239a)

esc를 누르면 파일 편집기에서 탈출하게된다.<br/>
그리고 : (콜론) 을 누르면 이렇게 콜론과 무언갈 입력하는 모드로<br/>
바뀌는데, 이제 여기에 단어 몇개를 넣어서 실습해 볼 것이다.
<br/>
<br/>
<br/>
<br/>

![vi철수에게5(저장후종료)](https://github.com/user-attachments/assets/480a5e98-9a5d-4b79-86c9-9da1e5d1de2e)

이제 w와 q의 의미를 알아보자.<br/>
- w : 저장
- q : 닫기

w와 q를 입력하면 저장 , 닫기후 터미널이 다시 원래모습으로 되돌아간다.
<br/>
<br/>
<br/>
<br/>
![vi철수에게6(최종본)](https://github.com/user-attachments/assets/6ac4a84f-eb1b-4415-aa0f-bbaf037485dc)

파일내에 수정한 내용이 그대로 잘 반영되었다.<br/>
<br/>
<br/>
<br/>
이렇게 리눅스 기초 명령어를 VS code에서 실습해보았다.<br/>
다음에는 다른 코딩 정보를 가지고 오겠다.<br/>
