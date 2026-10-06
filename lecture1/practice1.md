### Lecture 1: Course overview + the shell
pwd
ls -la
cd ..
mkdir lecture1
cd lecture1
touch hello.txt
echo "Hello, Missing Semester!" > hello.txt
cat hello.txt
cp hello.txt hello_copy.txt
mv hello_copy.txt hello_moved.txt
rm hello_moved.txt

### 2.然后练管道和重定向
ls -la | grep hello
echo "another line" >> hello.txt
cat hello.txt | wc -l

再写一个小脚本：

bash
nano hello.sh
写入：

bash
#!/bin/bash
echo "Hello from shell script!"
保存退出（Ctrl+O，回车，Ctrl+X），然后：

bash
chmod +x hello.sh
./hello.sh