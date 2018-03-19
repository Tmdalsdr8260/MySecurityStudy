# 10. Trainer10
<h4> 해킹의 과정과 SetUID에 대하여 알아봅시다<h4>

---

## <해킹의 종류>

`Local` 해킹 : 해킹하고자 하는 서버에 일반계정을 가지고 있을때, `루트 권한`을 얻고자 하는 해킹

`Remote` 해킹 : 자신이 해킹하고자 하는 서버에 아이디를 가지고 있지 않을 때, `아이디`를 얻고자 하는 해킹

- 무작위로 입력하여 접속
- 데몬의 취약점을 공락하여 접속
- 게시판이나 방명록을 이용하여 접속 ... 등 수십가지 존재

중요한 것은 Local 해킹 
- 루트 권한을 얻지 않으면 서버는 그림의 떡!!

---

## <SetUID란?>

`SetUID` : Set(변경하다) + UID(User ID)
           = 일시적으로 자신의 ID를 변경하는 것 

- 파일에 걸리는 것 > 이 파일 실행시 루트권한 획득
- 잠시 루트권한을 얻는 동안 멍청한 파일을 속이는 것 = 해킹

해킹을 하기 위해서는 프로그램에서 에러가 나는 순간, 메모리의 장소등을 계산해야 하긴 때문에 `C언어`가 중요

SetUID 살펴보기>

    Ex)
    -r-s--x--x  1 root    root      22312 Sep 26    1999 /usr/bin/passwd*
       ①

1)  x(실행권한)이 들어갈 자리에 s(SetUID)가 들어감
= s가 x를 포함하고 있기 때문

    [trainer10@ftz traienr10]$ find / -perm -4000

위의 명령은
" / 에서 부터, 적어도 SetUID가 걸린 모든 파일을 찾아라 "

4000앞의 - = 적어도
-perm = 권한을 찾겠다
4 = SetUID
000 = rwx모두 의미

find 명령 옵션>
-perm 권한과 일치하는 파일을 찾는다
-name 이름과 일치하는 파일을 찾는다
-user 유저와 일치하는 파일을 찾는다
-group 그룹과 일치하는 파일을 찾는다




---