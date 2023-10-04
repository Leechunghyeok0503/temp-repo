# Lecture 5

### Standard Output
**>**: 어떤 명령에 대한 출력 결과를 screen해서 보는게 아니라 file로 저장할 때 사용한다. 중복해서 수행하면 기존의 내용을 덮어쓰고 완전히 새로운 내용으로 file이 만들어진다.
**>>**: 예전에 기록했던 내용에 새로운 내용을 추가할 수 있다.
### Standard Input
**<**: 파일로부터 입력을 리디렉션할 수 있다.( '<' 와 '>' 같이 쓸 수 있음)

 |: command1|commad2 -> command1의 Output을 받아 그대로 command2에 대한 Input으로 넣어줌
 ls | wc -l: 현재 directory 안에 있는 file의 개수 확인 가능

 echo:echo 뒤에 오는 내용을 그대로 출력한다.
 echo *: 모두 출력한다
 echo ~: 현재 사용자의 홈 directory를 출력한다.
 echo ~name: 특정 유저의 홈 directory를 출력한다.
 Backslash(\\): Enter와 같은 기능

### Permissions
Linux: 서로의 file을 건드리거나 권한이 없는 사람이 어떤 권한을 가지고 실행하는 문제를 방지하고자 리눅스에서는 file과 directory에다가 3단계로 구분되는 명확한 권한을 부여한다.
-: file을 의미
d: directory를 의미
Files와 Directoies는 owner/group/others라는 3단계 권한을 가지고 있다.
rwx: 읽고 쓰고 실행 가는하다는 말
chmod 600 some_file: 600은 권한, 그 뒤엔 권한을 변경할 file, directory 이름임.
6=110: 읽고 쓸 수 있음음
0=000: do nothing
0=000: do nothing


---
Superuser라면 컴멘드 전에 'sudo' 넣을 것

Shell script
$ nano myscript.sh

hostory: 전에 사용한 커멘드 볼 수 있음

Superuser라면 컴멘드 전에 'sudo' 넣을 것

Shell script
$ nano myscript.sh

hostory: 전에 사용한 커멘드 볼 수 있음
