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

tempraliry chage enviromental variable by  [variable=value command]
```
[ec2-user@ip-172-31-40-30 tmp]$ LANG=C cal 3 2020
     March 2020
Su Mo Tu We Th Fr Sa
 1  2  3  4  5  6  7
 8  9 10 11 12 13 14
15 16 17 18 19 20 21
22 23 24 25 26 27 28
29 30 31

[ec2-user@ip-172-31-40-30 tmp]$ echo $LANG
en_US.UTF-8
```




