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
