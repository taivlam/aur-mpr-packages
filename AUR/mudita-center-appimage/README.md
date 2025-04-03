# `mudita-center-appimage`

## Maintainer metadata
* Architecture: `X86_64` only
* Packaging the AppImage
* File integrity: SHA512 checksums in YAML files
* No file authenticity (via GPG)
* [Link](https://github.com/mudita/mudita-center/releases/latest) to latest stable release on GH
* [AUR page](https://aur.archlinux.org/packages/mudita-center-appimage)
* Mudita Center application [page](https://mudita.com/products/software-apps/mudita-center/)

## Description

[Mudita](https://mudita.com/) is a digital minimalism company from Poland that
makes e-ink phones designed to counter the trend of
[problematic smartphone use](https://en.wikipedia.org/wiki/Problematic_smartphone_use).
The Mudita Pure is the company's first product that was successfully crowdfunded
on [Kickstarter](https://www.kickstarter.com/projects/mudita/mudita-pure-your-minimalist-phone/)
in September 2019 and started shipping the phone around 2022.

Mudita Center is a desktop application that manages a Mudita Pure phone and
other products from Mudita.

### Updates only for the latest stable release version of Mudita Center

To only keep updates on the latest stable version of Mudita Center, use the RSS
[feed](https://forum.mudita.com/c/software-updates/22.rss) for the "Software
Updates" tag on the [Mudita Forum](https://forum.mudita.com/) (which is based
on [Discourse](https://en.wikipedia.org/wiki/Discourse_(software))).

A warning about using the tags feed on GitHub: there are several daily automatic
development version of via its [GH tags](https://github.com/mudita/mudita-center/tags)
that are created daily, which are also replicated in the Atom feed for Mudita
Center's GH releases when one tries to use the releases Atom feed.

## Other (older) maintainer metadata/package description

This AUR package uses the [AppImage](https://en.wikipedia.org/wiki/AppImage)
version the application, as this is the only binary file available for Mudita
Center from [GitHub](https://github.com/mudita/mudita-center).

This is the first AUR package I adopted.

### Change these items after every upstream update
* `pkgver`
* `pkgrel` (if needed)
* `sha256sums_x86_64`

Lastly make sure to run:
```
$ makepkg --printsrcinfo > .SRCINFO
```
to keep the `.SRCINFO` up-to-date!

#### Note to self

This is here to help me remember what changes to the `PKGBUILD` I need to make.
I will keep reading the [AUR submission guidelines](https://wiki.archlinux.org/title/AUR_submission_guidelines)
to make sure everything is proper.

Also, no need to upload the `.SRCINFO` files onto GitHub, as these only affect
the AUR web listing on the package.

## Background info

[Mudita](https://mudita.com/) is a Polish technology company that started off
making an e-ink cell phone called the [Mudita Pure](https://mudita.com/products/phones/mudita-pure/).
The Mudita Pure first started via a Kickstarter crowdfunding
[campaign](https://www.kickstarter.com/projects/mudita/mudita-pure-your-minimalist-phone)
in 2019 and continued with an in-demand Indiegogo
[campaign](https://www.indiegogo.com/projects/mudita-pure-your-minimalist-phone#/).

Mudita Pure's operating system is [MuditaOS](https://mudita.com/products/phones/mudita-pure/muditaos/)
and the source code is on [GitHub](https://github.com/mudita/MuditaOS).

[Mudita Center](https://mudita.com/products/software-apps/mudita-center/) is a
desktop application that lets users update Mudita Pure devices via a USB
connection.  This is the only way to update MuditaOS, even when Mudita Pure is
being used as a mobile Wi-Fi hotspot.

## Rant on the insanity of pursuing security for its own sake

As a rather unenthusiastic owner of both the Light Phone II and the Mudita Pure,
I can say that Josh of Side of Burritos is ultimately a crank after watching the
[video](https://www.youtube.com/watch?v=OrZacTUhH0c).  Maybe you only need a
cell phone to make a single call on a SIM network, just like the Protagonist in
[_Tenet_](https://en.wikipedia.org/wiki/Tenet_(film)).  (Both examples are
relatively expensive as physical burner phones, though both lack camera
sensors - an excellent choice for those who would've removed the camera sensors
anyways.)

Maybe you just need a cell phone for a K-8 child to make unencrypted 4G phone
calls and SMS text messages to you when they come back home from school, and
they live within 1-2 miles of their school.  Even the cheapest third-generation
[iPhone SE](https://en.wikipedia.org/wiki/IPhone_SE_(3rd_generation)) is at
least over $500, after adding a case and glass screen protector.  (Not everyone
lives like a consumer electronics royal like MKBHD.)

Maybe you need a phone without the capability of installing any sort of app
store.  Now, don't get me started on that...

<details>

Yes, the only thing of value from Side of Burritos' first [video](https://www.youtube.com/watch?v=IzpVI4zaso0)
is that I use [Droid-ify](https://github.com/Droid-ify/client) and find the UX
of F-Droid proper rather slow.  Otherwise, this means absolutely means nothing
to a user like Louis Rossmann who needs a solution "right now"™.

The second part of the [video](https://www.youtube.com/watch?v=lAbgeJau3eE)
series on updating Android apps "securely".  The one point that helped me was to
simply use GrapheneOS's Owner profile to push apps that I'd use in both the
Owner and secondary user profiles; otherwise, undesirable apps should only be
installed on the secondary user profiles and never on the Owner profile.
However, I still figured this out primarily through direct experience and I only
realized in hindsight.

To top all of this out, this [video](https://www.youtube.com/watch?v=FFz57zNR_M0)
to outline the solution of "just use an RSS feed reader (on your phone), it's
gonna be great (on your phone)" makes me despise the [Read You](https://github.com/Ashinch/ReadYou)
app and having ever even tried it.  I wish I could take back every second of my
life this pathetic app has needlessly wasted.

Effectively the last [video](https://www.youtube.com/watch?v=JiN37bn0OE8) on
[Obtanium](https://github.com/ImranR98/Obtainium) of this "series" is absolutely
insane from a UX perspective. Do you know how hard it is to convince people to
use Signal for messaging, instead of SMS/MMS text messaging?  What makes you
think anyone wants to go through this Kafkaesque process of installing on
GrapheneOS?  Anyone who was willing to try GrapheneOS would probably want to
execute me at this point if I taught them that this is the most "secure" way of
updating Android apps.  So much for "upholding the Android security model" if
everyone following it to the "T" hates the experience.

</details>

#### TL;DR

<details>

Use [Feeder](https://github.com/spacecowboy/Feeder) on GrapheneOS, as it's
[recommended](https://www.privacyguides.org/en/news-aggregators/#feeder) by
Privacy Guides.  Feeder "just works"™.

Don't use Read You, it's absolute garbage when it comes to IRL UX; waiting for
notifications to come in from Nitter has a lower probability than waiting for
cosmic rays to catastrophically [corrupt](https://en.wikipedia.org/wiki/Soft_error)
your post-2018 laptop's SSD.  We need to stop making apps called "`* You`" for
any new app made with Material You (a.k.a. 
[Material Design 3](https://en.wikipedia.org/wiki/Material_Design#Material_Design_3_(Material_You))).

Just like how [Kakashi](https://en.wikipedia.org/wiki/Kakashi_Hatake) from
_Naruto_ says:

> [T]hose who abandon their friends are worse than scum!

I say that those who worship ill-defined security design over creating usable
solutions that are truly private and secure by default and by design to meet
where your users are right now are worse than scum.

Of course Light Phone II running on some closed-source Android 8 fork is not
secure, or Mudita Pure for that matter.  Nothing is going to compare to the
Titan M security chips in Google Pixel devices on Android, which GrapheneOS
fully utilizes.  I'd rather trust my life putting GrapheneOS into lockdown mode
rather than the PIN code on the Light Phone II or Mudita Pure (neither of which
has OS security backed by a dedicated hardware security chip).  Maybe it's not
**your** use case, but I'm sure someone else has been looking for it.

</details>

Become wise enough to be your own master, and decide on what **you** want.  Only
then will you be able to craft your own solutions with the features you need and
the threat model that works best for you.  Don't let others project onto you.

