---
title: "Nodejs Honeypot"
date: 2022-11-17T8:41:13+08:00
draft: false
hideLastModified: true
summaryImage: "honeypot-logo.png"
keepImageRatio: yes
tags: ["security", "Programming", "Nodejs"]
summary: "CES is a solution that help fine turn your k8s pods egress policy"
showInMenu: false
---

# Nodejs Honeypot

Nodejs Honeypot contains programming scripts, code that can be addon BIG-IP to provide low-interaction and high-interraction Honeypot.

More details refer to https://github.com/cloudadc/nodejs-honeypot.

## What's Nodejs Honeypot?

VS with iRule/iRuleLX as Honeypot, implemented by programming Scripts adapted with F5 HW/SW flexibly Adjustable at any time. Low Interaction Honeypot build by iRule, which can provide TCP Honeypot, HTTP Honeypot, Web Honeypot, etc; High Interaction Honeypot build by iRuleLX(Nodejs), which can provide high mutiple interaction web Honeypot.

## Key Advantages of Programming Honeypot

* The number of Honeypots: Base on ADC platform and its VS Programming interface(iRules/iRulesLX ), One Platform can create large number of Honeypots(600 - 1000) 
* Time to provision: Compare with commercial honeypot two devices architecture, F5 Honeypot only one device, easy to deploy, easy to provision, easy to maintaining
* More security:  F5 Honeypot is network honeypot, no dummy application exist, more security.(防逃逸)
* Low Interaction Honeypot: With F5 programming abilities, easy to create TCP honeypot, UDP Honeypot, HTTP Honeypot
* Invest Cost: Due to single device architecture, Low Investment can get more benefits
* Easy to adapted with different network: F5 is a L4 device, but has L3/L2 Capabilities
* Easy to integrate with Security Products: Can create VS Honeypot on F5 AWAF



