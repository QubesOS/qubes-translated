---
lang: de
layout: doc
permalink: /de/doc/releases/3.1/release-notes/
ref: 16
title: Qubes R3.1 release notes
---

# Qubes R3.1 release notes
<a id="qubes-r31-release-notes"></a>

## New features since 3.0
<a id="new-features-since-30"></a>

* Management Stack based of Salt Stack in dom0 - [documentation][salt-doc]
* Out of the box Whonix setup
* UEFI support
* LIVE edition (still alpha, not part of R3.1-rc1)
* Updated GPU drivers in dom0
* Colorful window application icons (instead of just colorful lock icon)
* PV Grub support ([documentation][pvgrub-doc])
* Out of the box USB VM setup, including [handling USB mouse][input-proxy]
* Xen upgraded to 4.6, for better hardware support (especially Skylake platform)
* Improve updates proxy flexibility - especially repositories served over HTTPS

You can get detailed description in [completed github issues][github-release-notes]

## Known issues
<a id="known-issues"></a>

* Installation image does not fit on DVD, requires either DVD DL, or USB stick (5GB or more)

* Windows Tools: `qvm-block` does not work

* Some icons in the Qubes Manager application might not be drawn correctly when using the Xfce4 environment in Dom0. If this bothers you, please use the KDE environment instead.

* USB mouse (in the case of USB VM) does not work at first system startup (just after completing firstboot). Workaround: restart the system.

* For other known issues take a look at [our tickets](https://github.com/QubesOS/qubes-issues/issues?q=is%3Aopen+is%3Aissue+milestone%3A%22Release+3.1%22+label%3Abug)

It is advised to install updates just after system installation to apply bug fixes for (some of) the above problems.

## Downloads
<a id="downloads"></a>

See [Qubes Downloads](/de/downloads/).

## Installation instructions
<a id="installation-instructions"></a>

See [Installation Guide](/de/doc/installation-guide/).

## Upgrading
<a id="upgrading"></a>

### From R3.0
<a id="from-r30"></a>

The easiest and safest way to upgrade to Qubes R3.1 is to install it from
scratch and use [qubes backup and restore tools](/de/doc/backup-restore/) for
migrating of all of the user VMs.

Users of Qubes R3.0 can upgrade using [experimental
procedure](/de/doc/upgrade-to-r3.1/).

### From R2 or earlier
<a id="from-r2-or-earlier"></a>

When upgrading from earlier versions the easiest and safest way is to install
it from scratch and use [qubes backup and restore tools](/de/doc/backup-restore/)
for migrating of all of the user VMs.

Alternatively you can [upgrade to R3.0
using](/de/doc/releases/3.0/release-notes/#upgrading) first, then follow the
instructions above. This will be time consuming process.

[salt-doc]: /de/doc/salt/
[pvgrub-doc]: /de/doc/managing-vm-kernel/
[input-proxy]: https://github.com/QubesOS/qubes-app-linux-input-proxy/blob/master/README.md
[github-release-notes]: https://github.com/QubesOS/qubes-issues/issues?q=is%3Aissue+sort%3Aupdated-desc+milestone%3A%22Release+3.1%22+label%3Arelease-notes+is%3Aclosed