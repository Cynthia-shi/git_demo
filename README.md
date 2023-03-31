# git_demo

## Git介绍  
* Git是分布式版本控制工具，用来管理本地的代码工程，它可以记录代码内容的变更。  

## Git常见操作  
* 初始化本地仓库  
git init  # 方法一：cd到想要创建本地仓库的目录后，使用以下命令,此时目录中会生成一个.git文件夹 git clone https:github.com/xxx/xxx.git           # 方法二：从远程仓库克隆一个仓库
* 设置用户名  邮箱   
git config --global user.name "FELaoL"    
git config --global user.email felaol@sina.com    
* 将已修改文件添加至暂存区      
git add filename       # 添加指定的文件到暂存区      
git add .             # 添加所有已修改的文件到暂存区     
* 查看本地库状态    
git status     
* 将暂存区的文件提交到git本地仓库     
git commit -m "第一次修改"        # ""中是本次修改的简要信息说明注释     
* 查看日志    
git reflog                     # 查看版本信息   
Git log                        # 查看详细版本信息  
* 版本穿梭 
git reset --hard 版本号         # 回到（版本号）版本     
* 查看用户名 邮箱
git config user.name git config user.email      
* 查看其他配置信息    
git config --list    
* 查看git版本   
git --version    

## Git分支    
* 查看分支（初始时git中只有一个master分支）     
git branch -v    
* 新建一个分支   
git branch 分支名                 # 创建一个新分支    
git checkout -b 分支名            # 创建一个新分支并切换到该分支     
* 切换分支     
git checkout 分支名                  # 切换到（分支名）分支     
* 合并分支     
git merge 分支名                     # 将分支合并到master上     
* 合并分支冲突      
git merge 分支名 -> 两个分支都有修改则合并冲突报错 -> 手动修改文件删掉指针和字符 -> git add .  -> git commit -m “备注”                                                  # 将分支合并到master上
