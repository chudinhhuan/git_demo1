# CÁC LỆNH CƠ BẢN KHI THAO TÁC VỚI GIT
### 1.CREAT email, username , password
>check : git config --list
>creat name : git config --global user.usernam name
>creat email: git config --global user.email your_email
>check email : git config user.email
>creat password : git config --global user.password you_pass
### 2.Delete username , email,password 
>delete email: git config --global --unset user.email
>delete password : git config --global --unset user.password
>delete username : git config --global --unset user.username
### 3.clone một source nào đó trên git và rename file
>- clone no rename : git clone link
>- clone and rename : git clone link new_name
>- pull : tải source , map với các file đang có trong project
### 4.Creat track a repository  
>input file you  can follow , type : git init

### 5.Lệnh git status
>- check status files changes 
>- command : git status
>- if changes  , you could comand : git add .  

### 6.Lệnh git add
>  - git add .  : đưa file vào trạng thái chờ
>	- git add -u : thêm những thay đổi của files cũ , ko quan tâm file mới
>	- git add -A : thêm vào all file mới cũ để chuẩn bị commit 
>	- commit : xác nhận thực hiện hành động lưu lại lịch sử một cách hoàn chỉnh

### 7.Lệnh git commit  : đưa file vào vùng sẵn sàng push
>- git commit -m "messager we are changed" : xác nhận thay đổi  trước đó cần add -A
>-  lệnh kết hợp : git commit -a -m "thông điệp"

### 8.Creat repository and push up remote repository
>	- git init  : creat follow
>	- git add namefile.tail   ( * - n )
>	- git commit -m "thôg điệp change" ( * - n )
>	- git branch -M main  
>	- git remote add origin  link.git  
>	- git push -u origin main  ( * - n )

## Lab note 
```
lab:
creat:   ssh-keygen
 
step1: - git init -> khởi tạo repo dưới local
       - git status  -> check now status git

step2: git checkout -b develop_name 
	-> tạo nhánh mới 

step3: commit code gồm: 
	- git add fileName -> add từng file 
	- git add . -> add all file
	- git commit -m "Mesage"

step4: thêm remote:
	- git remote add name_remote linkremote(git@github.com.....)

step5: Push code lên git
	- git push name_remote
---> finish task

******************* Các câu lệnh git cơ bản *****************

- git branch -d name_branch -> xóa 1 nhánh
- git checkout -b name_branch -> creat a new branch
- git branch -> xem danh sách nhánh
- git checkout name_branch -> chuyển nhánh
- git add . 
- git commit -m "Message" -> commit code( cần add trước khi commit)
- git remote add name_remote link_remote -> thêm mới 1 remote
- git remote -v -> kiểm tra remote
- git push name_remote name_branch -> đẩy code lên nhánh trên git 
- git pull name_remote name_branch -> kéo code mới nhất trên nhánh về local 	
```
