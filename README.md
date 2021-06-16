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

![avater](https://imgchr.com/i/DpCKn1)

git add <filename>      //把工作区文件添加到暂存区  

git commit -m <"说明">        //把暂存区文件添加到master版本库  

git push -u origin master    //把本地库的内容推送到远程，即把当前分支master推送到远程第一次推送master分支时，加上了-u参数    

如果在github的remote上已经有了文件，会出现错误。此时应当先pull一下，即：  
git pull origin master  

然后再进行：  
git push origin master  
  
---------------------------------------------------------------------------------------------------------------
//将本地代码推送到分支  
  git init                 //创建本地仓库  
  git remote add origin 仓库地址        //  本地代码连接到远程仓库  
  git checkout -b 分支名               //  新建分支    
  git add ...  
  git commit -m "说明"  
  git push --set-upstream origin 分支名   // 推送分支  
  git push -u origin 分支名 -f            // 不行就强推分支 
  
  删除远程分支：git push origin --delete 分支名称         
  删除本地分支：git branch -d 分支名称                    
  
  -------------------------------------------------------------------------------------------------------------
  //分支合并同步  
  git checkout 主分支   
  git pull origin 主分支  
  git checkout 分支名  
  git merge 主分支     //  合并分支  
  
  --------------------------------------------------------------------------------------------------------------
  
  
