## Git merge vs. Git rebase
둘의 차이점을 알아 보겠습니다.

![alt text](git-merge-git-rebase.jpeg)

Git에서 한 브랜치의 변경 사항을 다른 브랜치로 병합할 때, git merge 또는 git rebase를 사용할 수 있습니다.
아래 다이어그램은 두 명령어가 어떻게 작동하는지 보여줍니다.

### Git merge
git merge를 실행하면, 메인 브랜치에 새로운 커밋 **G'**가 생성됩니다.
G'는 메인 브랜치와 feature 브랜치의 이력을 연결하는 역할을 합니다.
병합 방식이 비파괴적(non-destructive) 이므로, 메인 브랜치와 feature 브랜치의 기존 커밋은 변경되지 않습니다.

### Git Rebase
git rebase는 기능 브랜치의 커밋을 메인 브랜치의 최신 커밋 이후로 이동시킵니다.

이 과정에서 기능 브랜치의 기존 커밋(E, F, G)이 **새로운 커밋(E', F', G')**으로 다시 작성됩니다.

git rebase의 장점은 선형 커밋으로 유지된다는 것입니다.

git rebase는 'rebase의 황금규칙'을 따르지 않으면 위험할 수있습니다.

rebase의 황금규칙이란?
public에서 사용을 하지말라는 것 입니다.