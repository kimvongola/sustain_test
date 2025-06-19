# List of Command Line
***
## Git Creation

- เปิด Git ใน Server: ```[Username]@[Server IP]```
- สร้าง Repository: ```mkdir [PATH]```
- สร้าง Bare Repository(Repo ที่่ไม่สามารถแก้ไฟล์ใน git ได้ต้อง clone ละค่อย Push): ```git init --bare [PATH]```
  ***
 ## Client Command
 - เชื่อม Repository ของ Server: ```git remote add origin ssh://[Username]@[Server IP]/[PATH to repo]```
 - Clone Repository: ```ssh://git@[Server IP]:/[PATH to Repo]```
 - สร้าง Project ใน Repository ```mkdir [Project Name]```
 - สร้าง Readme: ```echo [Content] > [Filename.type]```
 - สั้งให้ Git ดูการเปลี่ยนแปลงของไฟล์นั้นๆ: ```git add [Filename]```
 - สั้งให้ Git ดูการเปลี่ยนแปลงของไฟล์ทั้งหมด: ```git add .```
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

