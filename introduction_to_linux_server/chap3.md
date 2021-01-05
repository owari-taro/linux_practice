```
[ec2-user@ip-172-31-40-30 tmp]$ alias|grep ls
alias l.='ls -d .* --color=auto'
alias ll='ls -l --color=auto'
alias ls='ls --color=auto'
[ec2-user@ip-172-31-40-30 tmp]$
```


## difference between shell variable and enviromental variable
```
[ec2-user@ip-172-31-40-30 tmp]$ export MYENV="hoge"
[ec2-user@ip-172-31-40-30 tmp]$ myVal="geho"
[ec2-user@ip-172-31-40-30 tmp]$ bash
[ec2-user@ip-172-31-40-30 tmp]$ echo $MYENV
hoge
[ec2-user@ip-172-31-40-30 tmp]$ echo $myVal

[ec2-user@ip-172-31-40-30 tmp]$
```
