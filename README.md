# secret
A project to easily generate passwords or passphrases.

# how does it work?
```
A tool to generate secrets. By default it uses numbers, lower case letters and upper case letters (-naA)

Usage: secret [OPTIONS] [LENGTH]

Arguments:
  [LENGTH]
          

Options:
  -n, --numbers
          Wether to use numbers

  -v, --verbose
          Wether to be verbose

  -a, --lower-letters
          Wether to use lower case letters

  -A, --upper-letters
          Wether to use upper case letters

  -s, --symbols
          Wether to use symbols

  -w, --words
          Wether to use words instead of characters

  -l, --language <LANGUAGE>
          [default: ger]

  -h, --help
          Print help (see a summary with '-h')

  -V, --version
          Print version
```
# Password Examples
### without anything
```bash
./secret
qraxmsQGLBcRvUTcHEdT
```
### length of 20
```bash
./secret 20
iia2Glay6tmvT556hYXd
```
### only numbers
```bash
./secret 10 -n
6613472999
```
### only letters upper and lower case
```bash
./secret 10 -aA
RpNPkfRKLF
```
### length of 42 with numbers (-n), symbols (-s) and upper (-A) and lower (-a) case letters
```
./secret 42 -naAs
O__$=$vvI+xat-q*S+q%r=6gg++Ibm6HpoL@UWhk@x
```

# Passphrase Examples
#### Passphares work the same, but `-w | --word` as option is needed
### without anything
```
./secret -w
neunzehn-Wolkenlos-Holzhammer-Quelle-Ritzel
```
### 2 words
```
./secret 2 -w
Süße-Benzin
```
### why the hell are they german?
```
./secret 2 -w --language eng
strawberry-date
```
because german is default
### with leetspeak
```
./secret 2 -wn --language eng
4ppl3-n3ct4r1n3
```
### with leetspeak and uppercase letters
```
./secret 10 -wAn -l eng
R4spB3rRY-Eggpl4nt-nutm3G-kumqu4T-h0n3yd3w-v4N1ll4-x4NthAN-4ppl3-vIn3g4r-w4tErm3l0N
```
