### Github Commit & Push 된 Message 변경하는 법
1. CMD에서 수정하려는 커밋이 포함 된 저장소로 이동합니다.
1. `git commit --amend`를 입력 후 Enter 키를 누릅니다.
1. 텍스트 편집기에서 커밋 메시지를 편집하고 커밋을 저장합니다.
    1. a 키를 눌러 편집 모드로 변경 후, 메시지를 수정합니다.
    1. 수정 완료 후 ESC 키를 눌러서 편집 모드를 종료하고 `wq!`를 입력해 저장합니다.
1. `git push --force example-branch` 명령을 사용하여 이전 커밋을 강제로 푸시합니다.

### 참고 URL
- https://stackoverflow.com/questions/10728420/editing-the-git-commit-message-in-github
- https://docs.github.com/en/github/committing-changes-to-your-project/creating-and-editing-commits/changing-a-commit-message
