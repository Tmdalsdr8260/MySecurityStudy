# 1일차 - 3교시
- 2018-03-06 (화)

---

## <파이썬 설치>

1) `python.org`에 접속합니다.
2) 상단 메뉴의 `Downloads`를 클릭하여 다운로드 페이지에 들어갑니다.
3) 상단의 낙하산 그림 좌측의 `Download Python 3.6.4`를 클릭하여 다운을 시작합니다.
4) 다운이 완료 되면 `python-3.6.4.exe` 를 실행하여 설치를 진행합니다
5) 첫화면에서 하단의 `Add Python 3.6 to PATH`를 체크한 뒤 Install Now 버튼을 클릭하여 설치를 시작합니다.
체크하지 않을 경우 파이썬을 환경 변수에 직접 지정해주어야 하는 불편함이 있습니다.
6) 설치가 완료 되면 `close`버튼을 클릭하여 설치를 완료합니다.

---

## <Sublime Text 설치>
-window 기준입니다

1) `sublimetext.com`에 접속합니다.
2) 상단에 바로 보이는 `DOWNLOAD FOR WINDOWS`버튼을 클릭합니다.
3) 다운받은`Sublime Text Build 3143 x64 Setup.exe` 파일을 실행합니다.
4) Next를 눌러 다음으로 넘어간 뒤 Sublime Text를 설치할 경로를 지정한 후 다시 Next를 눌러줍니다.
5) 파일을 열때 오른쪽 마우스 클릭시에 Sublime Text를 나타나도록 하기 위해서는 `Add to explorer context menu`를 체크해줍니다.
6) 그 뒤 Install 버튼을 눌러 설치를 시작합니다.
7) Finish 버튼을 눌러 설치를 완료합니다.

---

## <파이썬 맛보기>
이제 설치해놓은 파이썬과 sublime text로 잠시 맛보기를 해봅시다

우선 sublime text를 실행하여 아래 코드를 작성해줍니다.

    print("hello world")

ctrl+s 를 눌러 저장한 뒤 그 파일이 있는 경로의 파일 탐색기를 들어갑니다. 예시를 위해 text.py 로 저장을 해보겠습니다.

이때 shift키와 오른쪽 마우스를 같이 클릭하면 여기에서 powershell 열기라는 버튼이 나옵니다. 그걸 눌러주세요!

그 후 아래 보이는 명령을 powershell에 입력해줍니다.

    python text.py

그렇다면 hello world가 화면에 출력됩니다!!

윈도우 cmd 환경에서는 경로로의 이동만 해준 후에는 위와 같습니다.

---

## <sublime text 단축키>

현재 줄을 다음 줄에 복사, 붙여넣기 하기 : ctrl + shift + D

현재 줄 주석 처리 : ctrl + /


---
## <파이썬의 주석 처리>

한 줄 주석처리 : `#`
여러 줄 주석처리 : `'''`

---