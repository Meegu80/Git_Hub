# Git_Hub Upload 업로드 푸쉬
깃허브 관리툴인 소스트리를 통해 자료를 관리하고 있습니다.
테스트로 진행중입니다.

![image](https://github.com/Meegu80/Git_SourceTree/assets/79518297/b3bb1c7e-588b-470d-bde5-9a7ab1061bd1)

깃허브 프로그램 사용법
출처 : https://soda-dev.tistory.com/12

1. Git을 설치한다.
https://git-scm.com/downloads

2. GitHub에 새 저장소를 생성한다.
3. 
4. 생성된 저장소의 주소를 기억해두자.
   - 주소는 반드시 HTTPS 주소를 복사한다.
     
5. 파일탐색기로 업로드해야할 폴더로 이동한 후, 마우스 오른쪽 버튼 눌러서 "Git Bash Here"를 누른다.
   
6. 초기 설정을 해준다.<br>
   
git config --global user.name "유저이름"
git config --global user.email "유저 이메일"
잘못이해하면 앞에 'user.name'에 깃허브 이름을 쓰고 마는 경우가 있는데 있는 그대로 user.name이라고 타자치고 " " 이 안에 본인 깃허브 이름을 넣는다, 유저 이메일도 마찬가지.
![image](https://github.com/Meegu80/Git_Hub/assets/79518297/9f519646-1d7f-41d0-86b6-1fe72cf2b93b)

7. 파일 준비
git init      #.git 파일 생성하는 것으로 그냥 똑같이 타자친다, 아무 변화 없이 줄바꿈만 되었다면 실행 완료.
git add .     #선택한 프로젝트 폴더 내의 모든 파일 관리, add치고 스페이스바한번치고 .(콤마) 엔터.
		-> 특정파일만 하고 싶다면  git add 파일이름.파일형식  ex) git add a.txt
git status    #상태확인 (이건 안해도 된다)
git commit -m "주석"     #커밋 복붙이 Shift+Ins키다, 실행되면 대상파일들 목록이 주루룩 화면에 올라간다.
8. 업로드하기
git remote add origin (위 3번에서 저장한 깃허브 저장소 주소)-HTTPS주소다. origin타자치고 공백 바로 주소. origin이 기존에 만들어졌다며 안되는 경우에는 main이나 master로 만들어라.
아래는 main으로 만든 경우이다.
![image](https://github.com/Meegu80/Git_Hub/assets/79518297/9eaf5b4a-77dd-42e6-89bc-c083c71fabc8)

git push -u origin master      왼쪽과 같이 코드치고 엔터누르면 업로드(푸쉬)가 마무리된다. 오리진이 만들어졌으면 master에 푸시하면 된다. 근데 나의 경우 main으로 만들었기때문에 푸시가 main에서 master로 푸시되었다.
그래서 main에 자료가 있지않고, 브랜치 master가 만들어져서 브랜치에서 자료를 확인해야하는 불편함이 생겼다. -끝-
![image](https://github.com/Meegu80/Git_Hub/assets/79518297/460ab184-03da-4f0b-81e8-689302d690dc)


