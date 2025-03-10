Em breve melhorias aguarde

# TL:DR

- Download and build
- Run against puzzle 66 (address mode)

```
./keyhunt -m address -f tests/66.txt -b 66 -l compress -R -q -s 10

```

You need to add `-t numberThreads` to get better speed

- Run against Puzzle 125 (bsgs mode)

```
./keyhunt -m bsgs -f tests/125.txt -b 125 -q -s 10 -R
```

You need to add `-t numberThreads` and `-k factor` to get better speed


# Disclaimer

I made this tool as a generic tool for the Puzzles.
I recommend to everyone to stay in puzzles

Several of users request me to add support for ethereum and minikeys, I did it.
But again i recommend only use this program for puzzles.

## For regular users

Please read the CHANGELOG.md to see the new changes

# Download and build

This program was made in a linux environment.
if you are windows user i strongly recommend to use WSL enviroment on Windows.
it is available in the Microsoft store

Please install on your system

- git
- build-essential

for legacy version also you are going to need:

- libssl-dev
- libgmp-dev

On Debian based systems, run this commands to update your current enviroment
and install the tools needed to compile it

```
apt update && apt upgrade
apt install git -y
apt install build-essential -y
apt install libssl-dev -y
apt install libgmp-dev -y
```

To clone the repository

```
git clone https://github.com/albertobsd/keyhunt.git
```

don't forget change to the keyhunt directory (But i'm not here to teach you linux commands)

```
cd keyhunt
```

First compile:

```
make
```

if you have problems compiling the `main` version you can compile the `legacy` version

```
make legacy
```


and then execute with `-h` to see the help

```
./keyhunt -h
```
