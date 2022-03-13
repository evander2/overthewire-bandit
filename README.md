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


## Level 14→ Level 15

## Level 15→ Level 16

## Level 16→ Level 17

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




