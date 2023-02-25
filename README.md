# C-linux
우분투 리눅스에서 C 프로그래밍 하기


## gcc 컴파일러 설치

sudo apt-get install gcc 

## vim editor 설치

sudo apt-get install vim

## vim editor

파일 작성    
vim hello.c
```c
#include <stdio.h>

int main() {
        printf("Hello World\n");
        return 0;
}

```

i : insert

저장 : ESC :w

종료 : ESC :q

## gcc로 컴파일    
gcc hello.c

## a.out를 실행
./a.out

## 파일내용 16진수로 출력

hexdump hello.c

## 파일내용 ASCII형태로 각 바이트의 값

xxd hello.c     
```c
00000000: 2369 6e63 6c75 6465 203c 7374 6469 6f2e  #include <stdio.
00000010: 683e 0a0a 696e 7420 6d61 696e 2829 207b  h>..int main() {
00000020: 0a09 7072 696e 7466 2822 4865 6c6c 6f20  ..printf("Hello
00000030: 576f 726c 645c 6e22 293b 0a09 7265 7475  World\n");..retu
00000040: 726e 2030 3b0a 7d0a 0a                   rn 0;.}..
```

-b: bit로 표시
xxd -b hello.c     

```c
00000000: 2369 6e63 6c75 6465 203c 7374 6469 6f2e  #include <stdio.
00000010: 683e 0a0a 696e 7420 6d61 696e 2829 207b  h>..int main() {
00000020: 0a09 7072 696e 7466 2822 4865 6c6c 6f20  ..printf("Hello
00000030: 576f 726c 645c 6e22 293b 0a09 7265 7475  World\n");..retu
00000040: 726e 2030 3b0a 7d0a 0a                   rn 0;.}..
```


