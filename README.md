# overthewire-bandit

## Level 0

`ssh -p 2220 bandit0@bandit.labs.overthewire.org`

`bandit0`

## Level 0 → Level 1

```
ls -al
cat readme
```
`boJ9jbbUNNfktd78OOpsqOltutMc3MY1`

## Level 1 → Level 2

```
ls -al
cat ./-
```
`CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9`

## Level 2→ Level 3

```
ls -al
cat spaces\ in\ this\ filename
```
`UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK`

## Level 3→ Level 4

```
cd inhere
ls -al
cat .hidden
```
`pIwrPrtPN36QITSp3EQaw936yaFoFgAB`

## Level 4→ Level 5

```
cd inhere
ls -al
head ./*
```
./-file07 :

`koReBOKuIDDepwhWk7jZC0RTdopnAYKh`

## Level 5→ Level 6

```
cd inhere
find -size 1033c
cat ./maybehere07/.file2
```
`DXjZPULLxYr17uwoI01bNLQbtFemEgo7`


## Level 6→ Level 7

```
find / -user bandit7 -group bandit6 -size 33c
```
/var/lib/dpkg/info/bandit7.password

```
cat /var/lib/dpkg/info/bandit7.password
```
`HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs`


## Level 7→ Level 8

```
cat data.txt | grep millionth
```
`cvX2JJa4CFALtqS87jk27qwqGhBM9plV`


## Level 8→ Level 9

```
cat data.txt | sort | uniq -u
```
`UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR`


## Level 9→ Level 10

```
strings data.txt | grep '='
```
`truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk`



## Level 10→ Level 11

```
base64 -d data.txt
```
`IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR`


## Level 11→ Level 12

```
cat data.txt | tr "A-Za-z" "N-ZA-Mn-za-m"
```
`5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu`


## Level 12→ Level 13

```
mkdir /tmp/evan
cp data.txt /tmp/evan
cd tmp/evan
xxd -r data.txt > bata.txt
file bata.txt
```
bata.txt: gzip compressed data, was "data2.bin", last modified: Thu May  7 18:14:30 2020, max compression, from Unix

```
mv bata.txt data2.bin.gz
gzip -d data2.bin.gz
file data2.bin
```
data2.bin: bzip2 compressed data, block size = 900k

```
mv data2.bin data2.bz2
bzip2 -d data2.bz2
file data2
```
data2: gzip compressed data, was "data4.bin", last modified: Thu May  7 18:14:30 2020, max compression, from Unix

```
mv data2 data4.bin.gz
gzip -d data4.bin.gz
file data4.bin
```
data4.bin: POSIX tar archive (GNU)

```
mv data4.bin data4.bin.tar
tar -xvf data4.bin.tar
file data5.bin
```
data5.bin: POSIX tar archive (GNU)

```
mv data5.bin data6.bin.tar
tar -xvf data6.bin.tar
file data6.bin
```
data6.bin: bzip2 compressed data, block size = 900k

```
mv data6.bin data7.bz2
bzip2 -d data7.bz2
file data7
``` 
data7: POSIX tar archive (GNU)

```
mv data7 data8.tar.gz
tar -xvf data8.tar.gz
file data8.bin
```
data8.bin: gzip compressed data, was "data9.bin", last modified: Thu May  7 18:14:30 2020, max compression, from Unix

```
mv data8.bin data9.bin.gz
gzip -d data9.bin.gz
file data9.bin
```
data9.bin: ASCII text

`8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL`


## Level 13→ Level 14

```
ssh -i sshkey.private bandit14@localhost
cat /etc/bandit_pass/bandit14
```
`4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e`


## Level 14→ Level 15

```
echo "4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e" | nc localhost 30000
```
`BfMYroe26WYalil77FoDi9qh59eK5xNr`


## Level 15→ Level 16

```
openssl s_client -connect localhost:30001
BfMYroe26WYalil77FoDi9qh59eK5xNr
```
`cluFn7wTiGryunymYOu4RcffSxQluehd`


## Level 16→ Level 17

```
nmap -p 31000-32000 localhost
```
Not shown: 996 closed ports
PORT      STATE SERVICE

31046/tcp open  unknown

31518/tcp open  unknown

31691/tcp open  unknown

31790/tcp open  unknown

31960/tcp open  unknown

```
openssl s_client -connect localhost:31790
cluFn7wTiGryunymYOu4RcffSxQluehd
-----BEGIN RSA PRIVATE KEY-----
MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34YkYWqUH57SUdyJ
imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObArnxd9Y7YT2bRPQ
Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5iCd5TbtJzEkQTu
DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3OekePQAzL0VUYbW
JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDLrjg0LWN6sK7wNX
x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBABagpxpM1aoLWfvD
KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5RlLwD1NhPx3iBl
J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4+UESzH22P29ovd
d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9AlbssgTcCXkMQnPw9nC
YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uNtJom+asvlpmS8A
vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxcUp1DGL51sOmama
+TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqYdsx0NxHgRRhORT
8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKLxrLgtT+qDpfZnx
SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGRNtMSkCgYEAypHd
HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0iE7KaszX+Exdvt
SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvGCSx+X3l5SiWg0A
R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4hyP5tJi93V5HDi
Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFMLy9FL2m9oQWCg
R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqIZFHxD6MjEGOiu
L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O6CdTkmJOmL8Ni
blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4ZxEnabvXnvWkU
YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfLF2MIAEwyzRqaM
77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1gvtGCWW+9Cq0b
dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9JPsX8MBTakzh3
vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY=
-----END RSA PRIVATE KEY-----
`





## Level 17→ Level 18

## Level 18→ Level 19

## Level 19→ Level 20

## Level 20→ Level 21

## Level 21→ Level 22


## Level 22→ Level 23

## Level 23→ Level 24

## Level 24→ Level 25


## Level 25→ Level 26


## Level 26→ Level 27




