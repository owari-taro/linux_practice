## symbolic-link

```
[ec2-user@ip-172-31-40-30 tmp]$ vi test.txt
[ec2-user@ip-172-31-40-30 tmp]$ dir
test.txt
[ec2-user@ip-172-31-40-30 tmp]$ dir
test.txt
#create symbolic-link which enable access to a designated file with  different name
[ec2-user@ip-172-31-40-30 tmp]$ ln -s test.txt  test2.txt
[ec2-user@ip-172-31-40-30 tmp]$ ls -l
total 4
lrwxrwxrwx 1 ec2-user ec2-user 8 Jan  5 00:39 test2.txt -> test.txt
-rw-rw-r-- 1 ec2-user ec2-user 9 Jan  5 00:37 test.txt
[ec2-user@ip-172-31-40-30 tmp]$
```



```
[ec2-user@ip-172-31-40-30 tmp]$ cat -n test.txt
     1
     2  hellow!
     3  world!
[ec2-user@ip-172-31-40-30 tmp]$ cat -n test.txt >new.txt
[ec2-user@ip-172-31-40-30 tmp]$

```

>& command redirect both std-ouput and standard-error
```
[ec2-user@ip-172-31-40-30 tmp]$ ls tmp hoge >$ out.txt
ls: cannot access hoge: No such file or directory
ls: cannot access out.txt: No such file or directory
[ec2-user@ip-172-31-40-30 tmp]$ dir
$  new.txt  test2.txt  test.txt  tmp
[ec2-user@ip-172-31-40-30 tmp]$ ls tmp hoge >& out.txt
[ec2-user@ip-172-31-40-30 tmp]$ dir
```
