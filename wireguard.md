---
canonicalUrl: https://www.wireguard.com/
date: 2023-04-23
draft: true
tags:
- inbox
- definition
sr-due: 2023-05-21
sr-interval: 4
sr-ease: 275
---

# WireGuard

> WireGuard is an extremely simple yet fast and modern
> [[virtual private network (vpn)|vpn]] that utilizes state-of-the-art
> cryptography. It aims to be faster, simpler, leaner, and more useful than
> IPsec, while avoiding the massive headache. It intends to be considerably more
> performant than OpenVPN. WireGuard is designed as a general purpose VPN for
> running on embedded interfaces and super computers alike, fit for many
> different circumstances. Initially released for the Linux kernel, it is now
> cross-platform (Windows, macOS, BSD, iOS, Android) and widely deployable. It
> is currently under heavy development, but already it might be regarded as the
> most secure, easiest to use, and simplest VPN solution in the industry.
>
> A combination of extremely high-speed cryptographic primitives and the fact
> that WireGuard lives inside the [[Linux|linux]] kernel means that secure
> networking can be very high-speed. It is suitable for both small embedded
> devices like [[smartphone|smartphones]] and fully loaded backbone routers.
>
> -- [WireGuard](https://www.wireguard.com/)

## Connecting to WireGuard

I wrote special [script](file:///home/inom/.local/bin/wg-toggle.sh):
`wg-toggle.sh` which allows me quickly toggle between WireGuard configuration
(up/down).
