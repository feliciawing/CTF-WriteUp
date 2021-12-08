# MetaCTF 2021

## Et tu, Hacker?

>The law firm of William, Ian, Laura, and Lenny (WILL for short) has just been the victim of an attempted cyber attack. Someone tried to brute force the login for one of their employees. They have the event logs of the incident, and were wondering if you could tell them which user was targeted. Flag is in the form of MetaCTF{}.

### Analysis

So we were given a event logs file named `bruteforce.evtx`

Which then after we opened it we could see there is some login attempt

![bruteforce](img/bruteforce.png)

And which after we scrolled down a little bit we see more login attempt which is a bruteforce as it happends in a shorttime and in a row

![bruteforce](img/bruteforce1.png)

So we did some analyzing which we found out that most of account name used for the bruteforce is `ericm`

![](img/flag.png)

So we tried to submit the account name combined with the flag form and it's correct

Flag : `MetaCTF{ericm}`