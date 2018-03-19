# 09. Trainer9
<h4>리눅스의 권한에 대해서 알아봅시다<h4>

---

## <권한 : Permission>

리눅스는 다른 사람이 서로의 파일에 접근하지 못하도록 막음

권한 밖의 파일을 건드린다면?
- Permission Denied(접근 거부) 에러 발생

---

## <리눅스 사용자>

종류>
1) 유저 : 사용자 자신
2) 그룹 : 하나 이상의 그룹에 속하게 됨(default : 자신의 유저네임과 같은 그룹)
3) 아더 : 유저와 그룹을 제외한 모든 다른 사람
4) 루트 : 절대적 권한을 가진 사용자 <= 이권한을 얻기 위해 `해킹`을 하게 됨

`id` 명령어 : 현재 사용자의 정보를 알 수 있는 명령어

    [trainer9@ftz trainer9]$ id
    uid=2009(trainer9) gid=2009(trainer9) groups=2009(trainer9)
     ①                  ②                   ③

1) uid : User ID (trainer9=2009)
2) gid : Group ID (특별한 일이 없는 한 gid = uid)
3) groups : 현재 자신이 어떤 그룹에 속해 있는지 알려줌 (기본적으로 자신의 uid와 같은 그룹에 속함)

## <파일의 권한 분석>

    Ex) -rwxrwxrwx      1 trainer9 trainer10        5 10dnjf 20 21:35 test1
          ①  ②  ③           유저      그룹                              파일이름

권한의 종류>
r(읽기권한) `cat`명령
w(쓰기권한) 파일의 수정권한
x(실행권한) exe, bat, com 의 확장자를 가진 것

1) 유저의 권한
2) 그룹의 권한
3) 아더의 권한

---