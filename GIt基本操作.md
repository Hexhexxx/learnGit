# Git基本操作

#### 初始化操作

- 创建一个新的Git仓库

  ```
  git init
  ```

  

- 添加一个远程仓库

  > remote指令。 <name>是注册名称，<url>是指定远程数据库的URL。
  >
  > 执行推送或者拉取的时候，如果省略了远程数据库的名称，则默认使用origin为远程数据库的名称，因此一般都会把远程数据库命名为origin。

  ```git
  git remote add <name> <url>
  git remote add origin git@github.com:Hexhexxx/仓库名
  ```

​		

- 克隆一个远程仓库

  > <repository>指定为远程数据库的URL，<directory>指定为复制目标目录的名称。

  ```
  git clone <repository> <directory>
  ```

  

#### 提交文件

1. 将文件添加到缓存区

   ```
   git add . 
   ```

2. 提交文件到本地仓库

   ```
   git commit -m "提交备注"
   ```

3. 将文件推送到远程数据库

   > <repository>是推送的目标地址，<refspec>是指定推送的分支。

   ```
   git push <repository> <refspec>...
   git push -u origin master
   ```



#### 其他命令

- 确认目录的状态

  ```
  git status
  ```

  

- 打开gitk

  ```
  gitk
  ```

  





