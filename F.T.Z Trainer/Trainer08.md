# 08. Trainer8
<h4>리눅스에서 새로운 파일을 만든 뒤 컴파일하는 방법을 알아봅시다.<h4>

---

## <텍스트 파일의 생성과 수정>

파일의 종류> 
- 일반 텍스트 파일 : cat명령 사용하여 내용출력

- 프로그램 소스 파일 : 컴파일을 거쳐 실행 가능하게 만듬


텍스트 파일 생성법>
1) 명령어 입력창에서 아래와 같이 입력

    cat > 파일이름.txt

2) 내용 입력
3) ctrl+D 입력

`>` 문자(리다이렉션) : (=방향을 전환한다)
                     cat명령 = 출력
                     cat + > = 입력

- 원래 파일이 있을때 리다이렉션을 한 번 사용하면 기존 내용은 모두 삭제됨

해결책 : 리다이렉션을 두번 사용하기 (`>>`)

    [trianer8@ftz traienr8]$ cat >> test.txt

---

## <프로그램 소스 파일 생성법>
1) 명령어 입력창에서 아래와 같이 입력

    cat > program.c

2) 소스 코드 입력
3) ctrl+D 입력

소스 파일은 `컴파일`이라는 과정을 거쳐야 실행 가능!!

컴파일 방법>

    gcc -o program.exe program.c
           프로그램_이름 소스파일

위와 같이 프롬프트에 명령어 입력

---

## <파일의 실행>

파일의 실행은 `절대경로`를 이용하여 실행할 수 있다.

    [trainer8@ftz trainer8]$ 절대경로/프로그림 이름

현재경로가 실행시킬 파일의 절대경로와 같다면 `./`을 사용해도 무관!

---