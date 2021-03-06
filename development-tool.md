# Backend Interview Question - (3) Development Tool

## Keywords

Git flow
GitHub flow
rebase

## Git

### 1. 版本管理系統是什麼？為什麼要用？

### 2. 為什麼 Git 稱作「分散式」版本管理系統？

### 3. 請寫下從 Github 上複製一個專案下來，做一次遞交，然後推上去會用到的所有 git 指令。

### 4. 在上述過程中，如果碰到 push rejected 的錯誤，是什麼原因？如何處理？

### 5. 什麼是 staging area？

### 6. 當多人協作時你要開發個功能，但不影響主程式，該怎麼作呢？要下什麼指令？開發好功能後需要下什麼指令合併回主程式？如果衝突了要如何處理？

> [name=Ivy Hung]

In order to develop a new feature and not pollute the main code, I would create a new branch and switch to it using `git switch -c <feature-branch-name>`.
After finishing developing, I would first switch back to the main branch and check if there is any update on it using `git switch main` > `git pull origin main` , then use `git merge <feature-branch-name>` to merge the feature branch back to the main branch. If there are conflicts, I would resolve them in the code editor, then commit the change.

### 7. 空的資料夾無法被加入 Git 進行版本控制，但這個資料夾如果又是很重要的資料夾，你會怎麼處理？

### 8. 在 Rails 專案中，config/database.yml 這個檔案裡有資料庫的設定、帳號密碼等資訊，在使用 Git 時，你通常會怎麼處理這類型內容比較敏感的檔案？

> [name=Sherry Liao]

I would store these sensitive/confidential information in process.env variables in an .env(dotenv) file, and include this .env file in our .gitignore file before commiting and pushing to the git repo.

### 9. 兩個 branch 各有五十個 commit 要接起來時，極有可能會出現大量的 conflict ，這時你會選擇用 merge 還是 rebase 處理它？哪個可能比較方便（或比較少的衝突）？為什麼？

> [name=Ivy Hung]

I would choose merge. Because a rebase involves repeated merges. If you have to copy fifty commits, you are doing fifty merges. On the other hand, if you use merge, you only need to resolve the possible conflicts one time.

<br>

###### :books: References

[it merge vs git rebase for merge conflict scenarios - stack overflow](https://stackoverflow.com/questions/59622140/git-merge-vs-git-rebase-for-merge-conflict-scenarios)
