# [OFFLINE SEED Generator for Tangle](https://acycliclabs.github.io/seedgen/)

## SEED
You must generate a random 81 character seed using only A-Z and the number 9. It is imperative that your seed be an 81 character random assortment of A-Z and 9.

### Create SEED on Linux Terminal
```
cat /dev/urandom |tr -dc A-Z9|head -c${1:-81}
```

### Create SEED on Mac OsX Terminal
```
cat /dev/urandom |LC_ALL=C tr -dc 'A-Z9' | fold -w 81 | head -n 1
```

(based on [knarz seedgen](https://knarz.github.io/seedgen/))

#### [Note: This is an offline seed generator and the entire code is here. However, the IOTA community has strict guidelines as to generate the seed only from wallet apps like trinity due to security concerns. Feel free to explore if you believe this works for you.]
