## git flow
- git clone [forked url]
- git flow init -d
- git remote add upstream [url]
- git fetch upstream
- git fetch origin
- git checkout feature/~
  - 안될 시 아래로 실행
  - git checkout -t upstream/feature/~ 

- 강제
  - git reset --hard upstream/[branch name]
  - git check out
  - git fetch upstream
  - git checkout upstream/[branch name]

- 원격 저장소 삭제
  - git push origin :feature/~

- 브랜치 저장소 확인
  - git branch -vv

- 브랜치 저장소 변경
  - git branch --set-upstream-to origin/feature/~~

- 원격 저장소 URL 변경
  - git remote -v (url 상태 확인)
  - git remote set-url origin [url]

- feature --
  - git flow feature start '피처명'
  - git flow feature finish '피처명'

- 덮어쓰기
  git fetch --all
  git reset --hard origin/master
  git pull origin master

- git global 사용자 삭제
  git config --global --unset-all user.name
  git config --global --unset-all user.email

- git 초기화
  git config --global --unset credential.helper
  git config --system --unset credential.helper


## 정규식
- 태그제외 str 만 : 문자열.replace(/\<.*?\>/g, '');
- 특정문자 있는지 : /문자\b/.test(문자열);
- 숫자만 추출 : 문자열.replace(/[^0-9]/g, '');

## etc
https://jsfiddle.net/2tygpe4f/4/

