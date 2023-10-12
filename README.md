# Lecture 6

### Changes VS Snnapshots  
Version control: 시간이 지남에 따라 어떤 version들에 대한 기록을 하는 것  
**CHanges**: 각각의 Version에서 시점을 복구할 때 Base version에 change들을 누적시켜 가면서 복구하는 방식  
**Snapshots**: GIT에서 많이 쓰이는 방식으로 각각의 version에서 file 전체에 대한 정보를 그대로 전환한다.  
### Local, Centralized, and Distributes Version Control
**Centralized**: 중앙에서 version central system을 관리하는 서버가 있다. 이 서버에서 여러 version들을 기록하고 있다가 local computer에서 중앙 서버로 부터 요청하고 기록된 version 중 하나를 가져와 local computer에 저장한다.
**Distributed**: Server Computer가 있다는 점에서 Centralized와 동일하지만 각각의 local computer가 중앙 computer가 가지고 있는 데이터 베이스를 통채로 그대로 복사본을 가지고 있음.

### Permissions
Linux: 서로의 file을 건드리거나 권한이 없는 사람이 어떤 권한을 가지고 실행하는 문제를 방지하고자 리눅스에서는 file과 directory에다가 3단계로 구분되는 명확한 권한을 부여한다.  
-: file을 의미  
d: directory를 의미  
Files와 Directoies는 owner/group/others라는 3단계 권한을 가지고 있다.  
rwx: 읽고 쓰고 실행 가는하다는 말  
chmod 600 some_file: 600은 권한, 그 뒤엔 권한을 변경할 file, directory 이름임.  
6=110: 읽고 쓸 수 있음  
0=000: do nothing  
0=000: do nothing  

Superuser라면 컴멘드 전에 'sudo' 넣을 것  
Shell script  
$ nano myscript.sh  
hostory: 전에 사용한 커멘드 볼 수 있음  
