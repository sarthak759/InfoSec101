# Bandit Level 14 to 15 Writeup



Author: [Sarthak Goyal](https://github.com/sarthak759) 

Problem Page: [bandit11](https://overthewire.org/bandit/bandit12) 

## List of Commands Used
```
telnet - remote login protocol, it allows users to connect to other computers
```

## Walkthrough
The first thing I did was using ssh to login to port 30000, and it failed, so I tried to find some command which uses hostname and port only and came across telnet 

## Password
`BfMYroe26WYalil77FoDi9qh59eK5xNr`

## Bash/Python script to automate the process
```
telnet local localhost 30000
```
## Suggested modifications [Optional]
What can you do to make this level more difficult. The inherent idea should be similar.