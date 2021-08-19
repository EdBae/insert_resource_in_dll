# insert_resource_in_dll


리소스 (.res) 데이터 DLL에 집어넣기 DELPHI

(.res) 데이터 DLL에 집어넣기

.bmp / .ico / .cur / .avi / .wmf / .jpg / .gif / .avi / .mp4
BITMAP / ICON / CURSOR / METAFILE / JPEG / 

이런 파일들을 리소스가 아닌 DLL 파일로 만들어서 사용하는 방법의 예제이다.

RESOURCE DLL 파일 생성하기

{$R *.RES}

에서 *에 파일명 RES 확장자의 파일 적어준다.

*.res는 리소스 파일 *.rc 라는 텍스트 파일을 brcc32.exe 로
실행하면 *.res라는 리소스 파일 생성.

MyResource.dpr 를 실행하면 MyResource.dll 파일이 생성되고 이 파일을 이용해서

ResTest2.exe 에서 LoadLibrary와 FreeLibrary 함수 이용하여 
동적으로 라이브러리를 로드하여 사용한다.

출처: https://sbrich.tistory.com/3799?category=152578 [SB리치패밀리]
