# Gituseage

---------------------------------------------------------------------------------------------------------------
create a new repository on the command line  

echo "# Gituseage" >> README.md  
git init  
git add README.md  
git commit -m "first commit"  
git branch -M main  
git remote add origin https://github.com/MambaCtrl/Gituseage.git  
git push -u origin main  

--------------------------------------------------------------------------------------------------------------
//更新内容时（工作区->暂存区->版本库）：    
//直接修改文件即修改工作区  

>cd "路径"              //若想进入某个文件夹下

![](https://imgchr.com/i/DpCKn1)

git add <filename>      //把工作区文件添加到暂存区  

git commit -m <"说明">        //把暂存区文件添加到master版本库  

git push -u origin master    //把本地库的内容推送到远程，即把当前分支master推送到远程第一次推送master分支时，加上了-u参数    

如果在github的remote上已经有了文件，会出现错误。此时应当先pull一下，即：  
git pull origin master  

然后再进行：  
git push origin master  
