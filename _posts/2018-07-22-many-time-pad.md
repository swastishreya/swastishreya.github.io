---
layout: post
title: Many Time Pad Attack
featured-img: cipher
mathjax: true
---

# Crypto is the new cool ?

We hear a lot about cryptography, cryptocurrency and cryptanalysis these days, isn't it ?

I got interested in the crib drag process used to decrypt messages when One Time Pad isn't taken seriously :P.

## What is One Time Pad ?

In cryptography, it is said that a One Time Pad encryption cannot be cracked(or let's say broken). It is referred as a perfectly secure method of encryption. But, this requires a one-time pre-shared key, whose size must be longer than or equal to the size of the message. In order to encrypt the message, each bit or character of the message is combined with the corresponding bit or character of the 'pre-shared' key. For combining the message, we make use of modular arithmetic.
Reference link : [wikipedia](https://en.wikipedia.org/wiki/One-time_pad).

For better understanding you can head to [Khan Academy](https://www.khanacademy.org/computing/computer-science/cryptography#crypt).

## What is a Many Time Pad Attack ?

First of all, in order for a message to be perfectly secure, it requires that the key never be used more than once. We can retrieve the text of two messages, which have been encrypted with the same key, without even knowing the key. So, a many time pad attack is only possible if you re-use a key to encrypt more than one messages. 

The simplest and the most understandable article I've read about many time pad attack is [this](http://travisdazell.blogspot.com/2012/11/many-time-pad-attack-crib-drag.html).

## About my code

I've used the crib drag method to implement the many time pad attack. I've written the code in python. 