# 02. Trainer2
<h4>디렉토리에 관한 여러가지 명령들을 알아봅시다<h4>

---

## <디렉토리에 관한 명령어>

`pwd` : 현재 자신이 들어가 있는 디렉토리를 알수 있는 명령어

    Ex) [trainer2@ftz trainer2]$ pwd
    /home/trainer2

현재 경로가 나타나게 됩니다

`cd` : 여러가지 방법을 이용하여 디렉토리 간 이동을 할 수 있게 하는 명령어 입니다.

    Ex) [trainer2@ftz trainer2]$ cd ..
    
cd 명령어 뒤에 `..`를 붙이면 한 단계 위로 이동 할 수 있습니다

    Ex) [trainer2@ftz trainer2]$ cd trainer2

위의 예시에서는 trainer2 디렉토리로 내려갔지만 다른 경우에서도 내려가고 싶은 디렉토리의 이름을 cd 뒤에 작성하면 한 단계 내려갈 수 있습니다.

`최상위 디렉토리(/)` : 리눅스에서는 '/'를 최상위 디렉토리라고 합니다.

    Ex) [trainer2@ftz trainer2]$ cd /

이 최상위 디렉토리에서 다시 원래 있던 곳으로 돌아가기 위해서는 많은 과정이 생기므로 한번에 할 수도 있습니다

    Ex) [trainer2@ftz trainer2]$ cd /home/trainer2

---

## <디렉토리의 생성과 삭제>

`mkdir`(Make DIRectory) : 새로운 디렉토리를 만드는 명령어

    Ex) [trainer2@ftz trainer2]$ mkdir linuxer

- mkdir 명령어 뒤에 만들 디렉토리의 이름을 입력하면 linuxer라는 이름의 디렉토리가 생성됩니다!

`rmdir`(ReMove DIRectory) : 디렉토리를 지우는 명령어

    Ex) [trainer2@ftz trainer2]$ rmdir linuxer

- rmdir 명령어 뒤에 지울 디렉토리의 이름을 입력하면 방금 생성했던 linuxer라는 이름의 디렉토리가 삭제됩니다!

---

## <파일과 과련된 명령어>

`cp`(CoPy) : 파일을 복사하는 명령어

    Ex) [trainer2@ftz trainer2]$ cp 복사원본 복사사본

위의 예시대로 할 시에 복사원본을 복사하여 복사사본이라는 이름으로 파일이 생성됩니다.

`rm`(ReMove) : 파일을 삭제하는 명령어

    Ex) [trainer2@ftz trainer2]$ rm 복사사본

`mv`(MoVe) : 파일을 복사한 후 원본을 지우는 명령어


    Ex) [trianer2@ftz trainer2]$ mv 복사원본 복사사본

- 이러한 특성때문에 주로 파일 이름을 변경할 때 사용

---