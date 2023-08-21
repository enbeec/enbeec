# 💛 Val Currie 💫

## ❤️ New Website Coming Soon!! 💥

I've been on a bit of a journey with my website. I picked Hugo because hopefully I can get `ox-hugo` working since I use `org-mode` but for now I whipped up a quick blog with a couple articles.

Figuring out where to host it was weirdly difficult. I initially wanted to go with object storage with an easy "run this command" workflow for deployment and updating the certificate. I do not, however, keep a credit card attached to my AWS account -- it's there for career development and testing but I don't love their billing model on my budget.

To keep a long story short I've come back around on something that's always been in my back pocket -- just running a containerized webserver and integrating a CDN. I've been hearing about Cloudflare alternatives lately so decided to give it a go.

You can track my progress here:

- [x] fail (after solving multiple problems) to use Linode Object Storage to host a Hugo site
- [x] contemplate running a webserver on a VPS using Docker
- [x] realize you're more comfortable with FreeBSD jails and set up a server on a hosting provider
- [x] find [a CDN with a free tier](https://gcore.com/cdn) to make self hosting the site a sane option
- [ ] server setup
  - [x] find a hosting provider with FreeBSD and decent prices
  - [x] set up an instance (root on UFS) with a ZFS pool on object storage
  - [x] firewall, packages, config, Bastille (for jail management)
  - [x] bootstrap an `nginx` thickjail
  - [ ] configure domain
  - [ ] import SSL cert *(I grabbed one I got with a bundle from my registrar before I thought I'd be using a server -- I'll ACME things eventually)*
  - [ ] push site
- [ ] add server to CDN sources

## 💙 Art Projects 🌊

[Lissajous Harmonics (Teensy OLED)](https://github.com/enbeec/lissajous-demo)

## 💜 OS Tomfoolery 🌌

- [BastilleBSD](https://bastillebsd.org/) template to null mount my homedir in a jail --> [[here]](https://github.com/enbeec/bastille-templates)
  - I have a few other templates on a home server I may publish if I can work out a few bugs *(or publish to get the bugs worked out?)*
  - Until something like [`runj`](https://github.com/samuelkarp/runj) is ready for use by someone with limited free time like me, Bastille is the closest I can get to the config-as-code ease of Docker

<!--
## 💚 🏔️
-->


