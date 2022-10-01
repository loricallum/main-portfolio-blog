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



# What if React's API and Svelte's compiler had a baby

Million makes creating user interfaces as easy as React, but with faster performance and smaller bundle size for the end user. By computing the user interface beforehand with a compiler, Million reduces the overhead of traditional Virtual DOM.

Okay cool… but why should I use Million if I can just use Preact if I need something a bit more lightweight?

While alternative libraries like Preact reduce bundle sizes by efficient code design, Million takes it a step further by leveraging compilation to make a quantum leap in improving bundle size and render speed.


# InAppBrowser tool reveals hidden JavaScript injections

A tool created by developer Felix Krause reveals hidden JavaScript injections through in-app browsers.

In-app browsers offer a convenient way for developers to let users browse specific websites without leaving their apps. However, they can be used to invade users’ privacy.

A JavaScript injection can be used via an in-app browser to collect data about users including their taps on a webpage, keyboard inputs, and more.

Armed with this data, a “digital fingerprint” can be created of a specific individual which can be used for targeted advertising.

Krause created a tool called InAppBrowser that can generate a report about the JavaScript commands that a developer is running through an in-app browser.

To use the tool, you only have to open the app you wish to analyse and use the in-app browser to open the URL “https://InAppBrowser.com”.

Krause has already tested some popular apps using his tool, including TikTok and Instagram.

TikTok was found to monitor all keyboard inputs and screen taps when using its in-app browser. Instagram, meanwhile, was able to detect all text selections on websites.