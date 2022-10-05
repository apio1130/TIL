# Git Merge
- 일반적으로 feature 브랜치를 Main 브랜치로 Merge 할 때 기본적으로 3가지 Merge 방식이 있음
- 종류 
  - Merge
  - Rebase
  - Squash + Merge

## Merge
- feature 브랜치에서 Main 브랜치로 결함하는 병합 커밋을 생성

## Rebase
- Main 브랜치에 커밋 내역을 다시 작성함
- Merge와 다르게 병합 커밋을 생성하는게 아닌 feature 의 커밋 내역을 그대로 Main 브랜치에 생성

## Squash + Merge
- feature 의 커밋 내역을 모두 포함한 새 스쿼시 커밋을 만들어 Main 브랜치에 생성
- Rebase와 다르게 커밋 내역들이 스쿼시 되어 있어 롤백에 있어 어려움이 있음(feature의 일부 커밋에 대한 롤백 불가)

## 참고
- https://matt-rickard.com/squash-merge-or-rebase
