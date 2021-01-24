git init                  # 해당 디렉터리에 깃 저장소를 만듦

|||||||||||||||    작업트리 -> 스테이지 -> 저장소     |||||||||||||||

git status                # 현재 깃의 상태를 나타냄

git add                   # 해당 파일을 스테이징

git commit -m             # 커밋 + 메시지 작성
git commit -am            # 한 번 이상 커밋된 파일을 스테이징과 커밋을 동시에 처리
git commit -amend         # 방금 입력한 커밋 메시지를 수정

git log                   # 커밋로그를 확인
git log --stat            # 해당 커밋에 어떤 파일이 관련되었는 지 알 수 있음

git checkout -- filename  # 해당 파일을 수정 전 상태로 되돌림

git reset HEAD filename         # 해당 파일을 스테이지에서 내림
git reset HEAD^                 # 최근에 커밋된 파일을 취소하고 스테이지에서 내림
git reset HEAD~n                # 최근 n개의 커밋을 취소
git reset --hard {커밋 해시}     # 해당 커밋이 가장 최신 커밋으로 됨

git revert {커밋 해시}           # 해당 커밋을 보류 시킴 / 보류 시킨 것이 커밋 됨
