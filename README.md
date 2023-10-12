# Lecture 6

### Changes VS Snnapshots  
Version control: 시간이 지남에 따라 어떤 version들에 대한 기록을 하는 것  
**CHanges**: 각각의 Version에서 시점을 복구할 때 Base version에 change들을 누적시켜 가면서 복구하는 방식  
**Snapshots**: GIT에서 많이 쓰이는 방식으로 각각의 version에서 file 전체에 대한 정보를 그대로 전환한다.  
### Local, Centralized, and Distributes Version Control
**Centralized**: 중앙에서 version central system을 관리하는 서버가 있다. 이 서버에서 여러 version들을 기록하고 있다가 local computer에서 중앙 서버로 부터 요청하고 기록된 version 중 하나를 가져와 local computer에 저장한다.  
**Distributed**: Server Computer가 있다는 점에서 Centralized와 동일하지만 각각의 local computer가 중앙 computer가 가지고 있는 데이터 베이스를 통채로 그대로 복사본을 가지고 있음.  

### Three stages in Git
Modified 단계의 working directory를 commit 단계로 가기 위한 준비 단계인 Staging area로 옮긴다.  
commit된다는 것은 snapshots을 찍었다. 혹은 특정 version을 기록했다는 걸 의미한다.  

### Git config: First-time setup      
**System level**: 모든 유저와 repository들에 영향을 줌
**Global(User) level**: 현재 사용자의 모든 repository에 영향을 줌
**Local level**: version control 위에서 만든 repositorty 안에서만 적용된다는 내용임
system->global->local: 뒤에 가는 것들이 앞의 것을 덮어쓴다.

---

$ git init: 작업한 directory 안쪽에 .git이라는 서버 directory가 만들어짐  
$ git status: 현재 repository가 어떤 status에 있는지를 확인하기 위해 사용한다.  
$ git add [file_name]: 특정한 file을 stage area로 올리고 싶을 때 사용 ($ git add 다음에 올리고 싶은 file 이름 적기)  
더 변화가 필요할 때 $ nano words.txt 사용한다. 변경된 상태에서 commit하면 원래 stage area에 올라왔던 내용 commit됨  
-> $ git add 사용해서 수정했던 내용을 staging area로 올림  
$ git add. : 전부 올림 
$ git rm -cached[file_name]: file system에서 실제로 file을 지우지 않고 staging 되어있던 file중에 staging area에서 빼내고 싶을 때 사용한다.  
$ nano .gitignore: 특정 file나 directory를 특정 file들만 골라서 무시하게 만들 수 있음




