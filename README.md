# nsa-codechallenge-2023

## Task 2

Answer
```
P1
P6
P43
P44
```

## Task 3

list all env
```
env print -a
```

and find `key_addr`

use `md` to view the address, `md.b` print the byte value

```
md.b <key_addr>
```

be careful for the endian

## Task 4

`hashcat` to bruteforce `[0-9a-f]`
key: `c44b878c1a623dfb38ba90f9a249260342fc6b38`

## Task 5

use `binwalk` to find secret file in `dropper` binary

## Task 6
```
# ssh tunnel
ssh -L 27017:100.100.250.36:27017 -i jumpbox.key user@external-support.bluehorizonmobile.com

# mongodb
mongodb://maintenance:7324f65b696f30@localhost:27017/?authSource=snapshot-84878f91a215
```
