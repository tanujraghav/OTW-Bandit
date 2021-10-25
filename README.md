# OverTheWire [Bandit](https://overthewire.org/wargames/bandit/) - Solutions

<br>

Server Information

|Host|<span style="font-weight:normal">ssh://bandit.labs.overthewire.org|
|:-|:--|
|<b>Port|2220|

---

**Level 0**

> ```bash
> (127.0.0.1) ssh bandit0@bandit.labs.overthewire.org -p 2220

:pirate_flag: **`bandit0`**

---

**Level 0 &#8680; 1**

> ```bash
> cat readme

:pirate_flag: **`boJ9jbbUNNfktd78OOpsqOltutMc3MY1`**

---

**Level 1 &#8680; 2**

> ```bash
> cat ./-

:pirate_flag: **`CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9`**

---

**Level 2 &#8680; 3**

> ```bash
> cat "spaces in this filename"

:pirate_flag: **`UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK`**

---

**Level 3 &#8680; 4**

> ```bash
> cat inhere/.hidden

:pirate_flag: **`pIwrPrtPN36QITSp3EQaw936yaFoFgAB`**

---

**Level 4 &#8680; 5**

> ```bash
> file ./inhere/*
> cat ./inhere/-file07

:pirate_flag: **`koReBOKuIDDepwhWk7jZC0RTdopnAYKh`**

---

**Level 5 &#8680; 6**

> ```bash
> find inhere/ -type f -readable ! -executable -size 1033c
> cat inhere/maybehere07/.file2

:pirate_flag: **`DXjZPULLxYr17uwoI01bNLQbtFemEgo7`**

---

**Level 6 &#8680; 7**

> ```bash
> find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
> cat /var/lib/dpkg/info/bandit7.password

:pirate_flag: **`HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs`**

---

**Level 7 &#8680; 8**

> ```bash
> cat data.txt | grep millionth

:pirate_flag: **`cvX2JJa4CFALtqS87jk27qwqGhBM9plV`**

---

**Level 8 &#8680; 9**

> ```bash
> cat data.txt | sort | uniq -c | grep -v 10

:pirate_flag: **`UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR`**

---

**Level 9 &#8680; 10**

> ```bash
> strings data.txt | grep -e [=]

:pirate_flag: **`truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk`**

---

**Level 10 &#8680; 11**

> ```bash
> base64 -d data.txt

:pirate_flag: **`IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR`**

---

**Level 11 &#8680; 12**

> ```bash
> cat data.txt | tr [A-Za-z] [N-ZA-Mn-za-m]

:pirate_flag: **`5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu`**

---

**Level 12 &#8680; 13**

> ```bash
> mkdir /tmp/yourname123
> cp ~/data.txt .
> xxd -r data.txt > data.gz
> gzip -d data.gz && mv data data.bz2
> bzip2 -d data.bz2 && mv data data.gz
> gzip -d data.gz
> tar -xf data
> tar -xf data5.bin && mv data6.bin data.bz2
> bzip2 -d data.bz2
> tar -xf data && mv data8.bin data.gz
> gzip -d data.gz
> cat data

:pirate_flag: **`8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL`**

---

**Level 13 &#8680; 14**

> ```bash
> (127.0.0.1) scp -P2220 bandit13@bandit.labs.overthewire.org:~/sshkey.private .
> (127.0.0.1) chmod 400 sshkey.private
> (127.0.0.1) ssh bandit14@bandit.labs.overthewire.org -p 2220 -i sshkey.private
> cat /etc/bandit_pass/bandit14

:pirate_flag: **`4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e`**

---

**Level 14 &#8680; 15**

> ```bash
> echo 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e | nc localhost 30000

:pirate_flag: **`BfMYroe26WYalil77FoDi9qh59eK5xNr`**

---

**Level 15 &#8680; 16**

> ```bash
> echo BfMYroe26WYalil77FoDi9qh59eK5xNr | openssl s_client -connect 127.0.0.1:30001 -quiet

:pirate_flag: **`cluFn7wTiGryunymYOu4RcffSxQluehd`**

---

**Level 16 &#8680; 17**

> ```bash
> nmap -sV --script ssl* localhost -p31000-32000
> echo cluFn7wTiGryunymYOu4RcffSxQluehd | openssl s_client -connect 127.0.0.1:31790 -quiet

:pirate_flag: *SSH Private Key*

---

**Level 17 &#8680; 18**

> ```bash
> (127.0.0.1) chmod 400 sshkey.private
> (127.0.0.1) ssh bandit17@bandit.labs.overthewire.org -p 2220 -i sshkey.private
> diff passwords.old passwords.new

:pirate_flag: **`kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd`**

---

**Level 18 &#8680; 19**

> ```bash
> (127.0.0.1) ssh bandit18@bandit.labs.overthewire.org -p 2220 ls -l
> (127.0.0.1) ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme

:pirate_flag: **`IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x`**

---

**Level 19 &#8680; 20**

> ```bash
> ./bandit20-do cat /etc/bandit_pass/bandit20

:pirate_flag: **`GbKksEFF4yrVs6il55v6gwY5aVje5f0j`**
