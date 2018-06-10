# CapstoneDesign-smart-AR-platform


# 빠르게 시작하기
본 프로그램을 실행하기 위한 빠른 시작 가이드 입니다. 

※이 프로그램을 시작하기 위해서는 [Unity](https://unity3d.com/kr/get-unity/download)와 [Nodejs](https://nodejs.org/ko/download/)가 우선적으로 설치되어야 합니다.

###  1단계. Unity Project 열기
본 프로그램을 clone하여 Unity라는 이름의 폴더를 Unity 에서 오픈합니다.

### 2단계. Target Marker 확인
프로그램을 실행하면 SampleScene이 자동으로 추가되어 있습니다.<br/>
SampleScene에서 ImageTarget으로 추가되어 있는 객체들을
카메라로 인식 시, AR 콘텐츠가 그 위에 나타납니다.<br/>
**즉, ImageTarget이 marker가 됩니다.**

*ImageTarget의 이미지는 Asset\Editor\Vufoia\ImageTargetTextures\Test 에서 확인할 수 있습니다.<br/><br/>
*Target Marker를 자신이 원하는 객체로 바꾸고 싶다면 [Vuforia](https://www.vuforia.com/)에 가입하여
license key를 생성하고<br/> target database를 만들어 자신의 Unity project에 import합니다. 자세한 내용은 [여기](https://library.vuforia.com/articles/Training/getting-started-with-vuforia-in-unity.html)를 참고 하세요.

### 3단계. Nodejs 서버 실행
cmd를 실행해 본 프로그램을 clone한 폴더로 이동후, Nodejs라는 이름의 폴더에서 **main.js**를 실행합니다.

### 4단계. 서버 지정하기
Unity project에서 Asset\MyScripts\SelectContentType.cs 파일을 오픈합니다.<br/>
`private string url = "http://MYSERVERIP:3000/";`<br/>
MYSERVERIP 부분을 자신의 서버주소로 바꿔줍니다.

### 5단계. 안드로이드 APK 빌드하기
안드로이드 디바이스를 PC에 연결 한 후, Unity 프로젝트에서 **File - Build & Run** 을 통해 실행합니다.
