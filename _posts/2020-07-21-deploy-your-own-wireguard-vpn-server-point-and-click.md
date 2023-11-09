---
layout: post
title: Deploy Your Own WireGuard VPN Server, Point and Click
categories: []
tags: []
status: publish
type: post
published: true
meta: {}
---
**TL;DR: While stuck at home during quarantine I built a point and click interface to deploy a WireGuard VPN Server to DigitalOcean. Bypass navigating VPN providers and run your own in about 15 minutes located in Amsterdam, Bangalore, Frankfurt, London, New York, San Francisco, Singapore, or Toronto.**

**Try it today, would love your feedback:** [https://vpn.democratize.cloud](https://vpn.democratize.cloud)

**See how it works, only pre-requisite is a** [**DigitalOcean**](https://m.do.co/c/293013c2f99a) **account:**

![Video](https://www.youtube.com/embed/Hh8m3vZJ6-0)

# Background

A basic tool in digital hygiene is the use of a VPN. For years I was a customer of Cloak VPN which then became Encrypt.me in 2017, who was then acquired by J2 Global. The service was (and probably still is) great, but with all those acquisitions and changes, I started to look around at options. There are tons of VPN providers and packages. As I researched, I came upon an [open source](https://github.com/trailofbits/algo) tool, [AlgoVPN](https://blog.trailofbits.com/2016/12/12/meet-algo-the-vpn-that-works/).

> “Algo VPN is a set of Ansible scripts that simplify the setup of a personal WireGuard and IPsec VPN. It uses the most secure defaults available and works with common cloud providers.”

The first thing that caught my eye were the [endorsements](https://github.com/trailofbits/algo#endorsements) so I gave it a shot. After installing dependencies, setting up a DigitalOcean account, and running some commands, I had a working VPN that I could set up on all of my devices. Further, the VPN was running on a server in my DigitalOcean account. The total cost was about $5 a month.

# Then Came Stay At Home

I had some time on my hands and I started thinking about all of these solutions I had access to being a software engineer. Tools like Algo VPN are limited to use by those that understand leveraging the cloud, installing programming languages, supporting packages, using secure shells, etc… Could you democratize their use? This thinking led to two things:

1. A mission statement: “Allowing everyone to leverage open source tools on their cloud.” [https://democratize.cloud](https://democratize.cloud)
2. The development of [https://vpn.democratize.cloud](https://vpn.democratize.cloud)

This first version was beta-tested by a small group with rounds of feedback simplifying the interface. In future iterations, I plan to support more advanced options as well as offer customization such as naming servers and devices in a paid plan.

I’m also starting to explore if the solution may work for Managed Service Providers, if that is you please do get in [touch](https://benr.eu/about).
