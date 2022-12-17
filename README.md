# noob programming 
Noob programming is a world-wide developer community platform to share technology and get mentoring.


## Github
### Name of the local git branch is changed to "main" from "master"!!
Related Articles</br>
* https://www.zdnet.com/article/github-to-replace-master-with-alternative-term-to-avoid-slavery-references/ 
* https://jarv.is/notes/github-rename-master/

Must rename your local master git branch!
git branch -m master main

[How to use git (MUST READ)]
1. git clone [remote address] -> 로컬에 복사(git remote -v 쳐보면 git clone때문에 remote 주소가 등록됨)
2. git branch -m master main (master -> main 으로 rename)
3. git pull origin main -> origin의 코드를 로컬 main 브랜치를 up-to-date 시킴
4. git checkout -b inyeobkim-dev -> 새로운 브랜치에서 작업은 필수! (브랜치 명명은 이름 + dev)
5. git push orign inyeobkim-dev -> inyeobkim-dev 브랜치를 remote origin 으로 푸쉬! (main 브랜치로 작업 브랜치를 merge 하지말고 작업 브랜치를 바로 push 해주세요)
6. 협업자들끼리 확인한 뒤 다같이 merge 할 예정

그 외 명령어
1. git branch -d <branch_name> --> deleting local branch
2. git push -d origin <branch_name> --> deleting remote tracking branch
3. git branch -D dev (force delete without considering merge result: --delete --force)
4. git branch -a (list all branches including local and remote tracking)
5. git checkout -b <branch_name> (create a new branch of branch_name and switch to it)

# Development Resources
* https://trello.com/en (Project Management Tool) -> Make sure to add your name and a due date when making a new card
* https://docs.google.com/document/d/134MmpJO3CIvDpNYukts_IlSy3LWm9_-zJSPI-eJ_Myc/edit - Google Doc for the meeting minutes
* https://slack.com/ - for the group project

# [Frontend]

## Articles
* Github Token: https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/

## Meeting Schedule
* Monday 10pm

## Development Considerations
* Tech stack
* Platforms(Web/Mobile)
* Development Team
* Developement Cost
* Timeline(UI/UX, Frontend, Backend, Testing/launching, Finalizing/Maintenance)
* How to use Trello

## Frontend Structure Design
<img width="812" alt="Screen Shot 2021-07-03 at 11 29 42 AM" src="https://user-images.githubusercontent.com/60948817/124340690-02c58600-dbf2-11eb-974c-98036d2546a5.png">

## Frontend Folder Structure
<img width="568" alt="Screen Shot 2021-07-04 at 2 19 37 PM" src="https://user-images.githubusercontent.com/60948817/124374046-e6e5e100-dcd2-11eb-8e24-77a92ee1dba2.png">

## Frontend Resources
* Redux explanation: https://dev.to/codebucks/what-is-redux-simply-explained-2ch7  
* React redux: https://react-redux.js.org/tutorials/connect   
* Emmet: https://medium.com/@eshwaren/enable-emmet-support-for-jsx-in-visual-studio-code-react-f1f5dfe8809c

## How to load React App
Type "npm start" on the terminal inside the frontend directory where package.json is located.

# [Backend]

## Function Requirement
https://www.notion.so/StockChat-8f932b0828b34c9382bb36e43ac51715

## Data Modeling
![image](https://user-images.githubusercontent.com/85722378/126040240-7ee3b6fb-823d-4d8c-b4a8-c603227482a9.png)
