---
type: posts
title: Blog
date: 2022-6-28
---

# Detecting Price Manipulation Attacks on DeFi Applications

Decentralized Finance (DeFi) is a system of financial products and services built and delivered through smart contracts on various blockchains. In the past year, DeFi has gained popularity and market capitalization. However, it has also been connected to crime, in particular, various types of securities violations. 

Ethereum functions as a distributed virtual machine and is the platform on which
much of the DeFi ecosystem currently runs.

The rapid growth of Decentralized Finance (DeFi) boosts the Ethereum ecosystem. At the same time, attacks towards DeFi apps are increasing. However, existing smart contract vulnerability detection tools cannot be directly used to detect DeFi attacks. That's because they lack the capability to recover and understand high-level DeFi semantics, e.g., a user trades a token pair X and Y in a Decentralized EXchange (DEX). 

In work by Siwei et al (2021), they focus on the detection of two types of new attacks on DeFi apps, including direct and indirect price manipulation attacks. The former one means that an attacker directly manipulates the token price in DEX by performing an unwanted trade in the same DEX by attacking the vulnerable DeFi app. The latter one means that an attacker indirectly manipulates the token price of the vulnerable DeFi app (e.g., a lending app). 

They propose a platform-independent way to recover high-level DeFi semantics by first constructing the cash flow tree from raw Ethereum transactions and then lifting the low-level semantics to high-level ones, including token trade, liquidity mining, and liquidity cancel. And detect price manipulation attacks using the patterns expressed with the recovered DeFi semantics. They have implemented a prototype named \tool{} and applied it to more than 350 million transactions. It successfully detected 432 real-world attacks in the wild. 