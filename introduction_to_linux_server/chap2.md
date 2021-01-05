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


## pipe
```
[ec2-user@ip-172-31-40-30 tmp]$ cat -n /etc/services |head -n 100|tail -n 10
    91  http            80/sctp                         # HyperText Transfer Protocol
    92  kerberos        88/tcp          kerberos5 krb5  # Kerberos v5
    93  kerberos        88/udp          kerberos5 krb5  # Kerberos v5
    94  supdup          95/tcp
    95  supdup          95/udp
    96  hostname        101/tcp         hostnames       # usually from sri-nic
    97  hostname        101/udp         hostnames       # usually from sri-nic
    98  iso-tsap        102/tcp         tsap            # part of ISODE.
    99  csnet-ns        105/tcp         cso             # also used by CSO name server
   100  csnet-ns        105/udp         cso
```
