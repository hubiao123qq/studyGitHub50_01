本地git工作流程

1.新建文件夹

2.进到文件夹

3.右键点击git bash here 

4.git init 新建仓库(也就是隐藏的.git文件夹)

```
实际上5和6才是用到最多的
5.编码

6.git add .

git commit -m"描述信息"
```



```
刚刚打开的终端`Git Bash`无法使用`ctrl+c和ctrl+v`,需要通过右键进行操作copy paste
```

```
新建一个文件夹命名最好是英文,双击进入文件夹,右键Git Bash 输入git init 出现了一个.git文件夹(一开始是隐藏的)，看不到这个.git文件夹可能是查看---详细信息--隐藏的项目没勾上
```



### 二.设置用户名和邮箱配置

**2.1  设置的第一种方式**

git  config --global user.email ''邮箱''

it config --global user.name ''用户名'' 

**2.2  设置的第二种方式**

先取消设置的邮箱和用户名

git config --global --unset user.email

git config --global --unset user.name

执行完上述命令之后,就再次用上面的命令来设置用户名和邮箱了

### 三.  查看设置好的用户名和邮箱

git  config --global user.email

git config --global user.name

### 四.  git提交

**4.1 添加此次修改的文件**

a.  单个文件

git add 文件名

b.  多个文件

git add 文件名1 文件名2 ....

c.  所有文件

git add .

**4.2 提交**  

git commit -m"提交的内容(文字)"

### 五.  状态信息查看

git status 

刚刚的操作修改了哪些文件呀,是否执行了添加命令呀这些都可以通过如下命令查看:



### 六.  查看完整信息

git log

git log --oneline 查看简略信息(一行内查看)

### 七. git版本回滚

命令：git  reset  --hard 版本号   //版本回滚的命令

命令： git  log --oneline   //查看一行类型的日志,包括版本号

命令： git reflog 查看所有的日志,包括回滚的日志(比如你不小心关掉了git想重新回滚到之前的版本就可用这个命令来查看之前的版本号)

commit 后面的**黄色部分**就是版本号

![image-20200813165337701](C:\Users\hubia\AppData\Roaming\Typora\typora-user-images\image-20200813165337701.png)