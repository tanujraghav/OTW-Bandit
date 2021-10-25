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

---

**Level 20 &#8680; 21**

> ```bash
> nmap localhost
> (session-1) echo "GbKksEFF4yrVs6il55v6gwY5aVje5f0j" | nc -lp 2021
> (session-2) ./suconnect 2021

:pirate_flag: **`gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr`**

---

**Level 21 &#8680; 22**

> ```bash
> cat /etc/cron.d/cronjob_bandit22
> bash /usr/bin/cronjob_bandit22.sh
> cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv

:pirate_flag: **`Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI`**

---

**Level 22 &#8680; 23**

> ```bash
> cat /etc/cron.d/cronjob_bandit23
> cat /usr/bin/cronjob_bandit23.sh
> echo I am user bandit23 | md5sum | cut -d' ' -f1
> cat /tmp/8ca319486bfbbc3663ea0fbe81326349

:pirate_flag: **`jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n`**

---

**Level 23 &#8680; 24**

> ```bash
> cat /etc/cron.d/cronjob_bandit24
> cat /usr/bin/cronjob_bandit24.sh
> mkdir /tmp/yourname123
> chmod 777 /tmp/yourname123
> cd /tmp/yourname123
> touch script password
> chmod 777 *
> echo "#!/usr/bin/env bash \n cat /etc/bandit_pass/bandit24 > /tmp/yourname123/password" > script
> cp script /var/spool/bandit24/
> cat password

:pirate_flag: **`UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ`**

---

**Level 24 &#8680; 25**

> ```bash
> mkdir /tmp/yourname123
> cd /tmp/yourname123
> echo "#!/usr/bin/env bash
> for i in 0 1 2 3 4 5 6 7 8 9; do
>   for j in 0 1 2 3 4 5 6 7 8 9; do
>     for k in 0 1 2 3 4 5 6 7 8 9; do
>       for l in 0 1 2 3 4 5 6 7 8 9; do
>         echo "UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ $i$j$k$l" >> keys
>       done
>     done
>   done
> done" > script
> bash script
> cat keys | nc localhost 30002

:pirate_flag: **`uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG`**

---

**Level 25 &#8680; 26**

> ```bash
> (127.0.0.1) scp -P 2220 bandit25@bandit.labs.overthewire.org:~/bandit26.sshkey .

:pirate_flag: *SSH Private Key*

---

**Level 26 &#8680; 27**

> ```bash
> (127.0.0.1) ssh bandit25@bandit.labs.overthewire.org -p 2220 bandit26.sshkey
> (minimize the terminal and press `v`)
> :set shell=/bin/bash
> :!shell
> ./bandit27-do cat /etc/bandit_pass/bandit27

:pirate_flag: **`3ba3118a22e93127a4ed485be72ef5ea`**

---

**Level 27 &#8680; 28**

> ```bash
> cd /tmp/yourname
> git clone ssh://bandit27-git@localhost/home/bandit27-git/repo
> cat repo/README

:pirate_flag: **`0ef186ac70e04ea33b4c1853d2526fa2`**

---

**Level 28 &#8680; 29**

> ```bash
> cd /tmp/yourname
> git clone ssh://bandit28-git@localhost/home/bandit28-git/repo
> cd repo
> git checkout c086
> cat README.md

:pirate_flag: **`bbc96594b4e001778eee9975372716b2`**

---

**Level 29 &#8680; 30**

> ```bash
> cd /tmp/yourname
> git clone ssh://bandit29-git@localhost/home/bandit29-git/repo
> cd repo
> git fetch origin dev:dev
> git checkout dev
> cat README.md

:pirate_flag: **`5b90576bedb2cc04c86a9e924ce42faf`**

---

**Level 30 &#8680; 31**

> ```bash
> cd /tmp/yourname
> git clone ssh://bandit30-git@localhost/home/bandit30-git/repo
> cd repo
> git tag
> git show secret

:pirate_flag: **`47e603bb428404d265f59c42920d81e5`**

---

**Level 31 &#8680; 32**

> ```bash
> cd /tmp/yourname
> git clone ssh://bandit31-git@localhost/home/bandit31-git/repo
> cd repo
> echo "May I come in?" > key.txt
> rm .gitignore
> git add .
> git commit -m "request for Level 32 password"
> git push origin master

:pirate_flag: **`56a9bf19c63d650ce78e6ec0354ee45e`**
