# Connection with SSH
## command
> host : bandit.labs.overthewire.org , port : 2220

```sh
ssh bandit.labs.overthewire.org -p 2220
```
&nbsp;
# Level 0 -> level 1
## command
```sh
cat readme 
```

> password : 'NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL'
&nbsp;
# Level 1 -> level 2
## command 
```sh
cat <-
```
> password : 'rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi'
&nbsp;
# Level 2 -> level 3
## command 
```sh
cat spaces\ in\ this\ filename
```
> password : 'aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG'
# Level 3 -> level 4
## command
```sh
cd inhere
ls -a -> .hidden
cat .hidden
```
> password : '2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe'
&nbsp;
# Level 4 -> level 5 
## command
```sh
ls -a
cd inhere
find -type f | xargs file | grep text
cat ./-file07
```
> password : 'lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR'
&nbsp;
# Level 5 -> 6
## command
```sh
find . -type f -size 1033c ! -executable -exec file {} + | grep -w text
cd maybehere07
cat .file2
```
> password : 'P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU'
&nbsp;
# Level 6 -> 7
## command
```sh
find / -type f -size 33c -user bandit7 -group bandit6
```
> password : 'z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S'
&nbsp;
# Level 7 -> 8
## command
```sh
grep 'millionth' data.txt
```
> password : 'TESKZC0XvTetK0S9xNwm25STk5iWrBvP'
&nbsp;
# Level 8 -> level 9
## command
```sh
sort data.txt | uniq -u
```
> password : 'EN632PlfYiZbn3PhVK3XOGSlNInNE00t'
&nbsp;
# Level 9 -> 10
## command
```sh
strings data.txt | grep '='
```
> password : 'G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s'
&nbsp;
# Level 10 -> level 11
## command
```sh
base64 -d data.txt
```
> password : '6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM'
&nbsp;
# Level 11 -> level 12
## command
```sh
cat data.txt | tr A-Za-z N-ZA-Mn-za-m
```
> password : 'JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv'
&nbsp;
# Level 12 -> level 13
## command
```sh
mkdir /tmp/data2/
cp /home/bandit12/ /tmp/data2/
cd /tmp/data2
xxd -r data.txt > data2
mv data2 data2.gz
gzip -d data2.gz
mv data2 data3.bz2
bzip2 -d data3.bz2
mv data3 data4.gz
gzip -d data4.gz
mv data4 data4.tar
tar xf data4.tar
mv data5.bin data6.tar
tar xf data6.tar
mv data6.bin data6.bz2
bzip2 -d data6.bz2
mv data6 data7.tar
tar xf data7.tar
mv data8.bin data8.gz
gzip -d data8.gz
cat data8

```
> password : 'wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw'
