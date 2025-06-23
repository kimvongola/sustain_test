# List of Command Line
***
## Server Command

- เปิด Git ใน Server: ```ssh [Username]@[Server IP]```
- สร้าง Repository: ```mkdir [PATH]```
- สร้าง Bare Repository(Repo ที่่ไม่สามารถแก้ไฟล์ใน git ได้ต้อง clone ละค่อย Push): ```git init --bare [PATH]```
- ลบ Repository folder: ```rm -rf [Reponame].git```
- ลบ Tracking: ```Remove-Item -Recurse -Force .\[Reponame]\```
- ลบแค่ .git: ```rm -rf .git```
  ***
 ## Client Command
 - เชื่อม Repository ของ Server: ```git remote add origin ssh://[Username]@[Server IP]/[PATH to repo]```
 - Clone Repository: ```git clone ssh://[uesrname]@[Server IP]:/[PATH to Repo]```
 - สร้าง Project ใน Repository ```mkdir [Project Name]```
 - สร้าง Readme: ```echo [Content] > [Filename.type]```
 - สั้งให้ Git ดูการเปลี่ยนแปลงของไฟล์นั้นๆ: ```git add [Filename]```
 - สั้งให้ Git ดูการเปลี่ยนแปลงของไฟล์ทั้งหมด(Tracking): ```git add .```
 - Commit/Update File(Local Update): ```git commit -m [Update Name]```
 - Push Code(Public Update): ```git push -u origin main```
 - สร้าง & เปลี่ยน Branch: ```git checkout -b [Branch name]```
 - Push Branch ตัวเองไป Main(รอบแรก): ``` git push -u origin [Branch name]```
 - Push Branch ตัวเองไป Main(รอบถัดไป): ``` git push```
 - ลบ Branch: ```git push origin --delete [Branch name]```
 - ดูว่ามี Branch อะไรบ้าง: ```git ls -remote origin```
 - ดูประวัติ Branch: ```git log --oneline```
 - หา PATH ของ Repository: ```realpath ~/[Repository Name]```
 - ลิสต์ไฟล์ในแต่ละ Repository: ```git --git -dir = [PATH] ts -tree -r [Branch name] --nameonly```
 - ดูเนื้อหาใน File: ```git show branch:[Path to file]```

***
# Process
1. Install Git Bash https://git-scm.com/downloads
2. Login to Server with your account ```ssh [Username]@[Server IP]```
3. Create your own repo ```mkdir [PATH]```
4. Go to your created repo ```cd [PATH]```
5. Make it a bare repo ```git init --bare [PATH]```
6. Clone repo(main branch) to your laptop ```git clone ssh://[username]@[Server IP]:/[PATH to Repo]```
   2. Clone repo(specific branch) to your laptop ```git clone -b [Branch main] ssh://git@[Server IP]:/[PATH to Repo]```
8. Cretae/Edit your script
9. Track the chabge of the scripts ```git add .```
10. Commit to the local cloned repo ```git commit -m [Update Name]```
11. [OPTIONAL] : Pull repo to check changes ```git pull origin main```
11.2. Pull specific branch ```git checkout [Branch name]``` -> ```git pull origin [Branch name]```
13. Push to the main repo ```git push -u origin main```
14. Check content in file ```git --git-dir=[Path to repo] show [Branch name]:[File name]```
