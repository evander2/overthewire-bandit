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





