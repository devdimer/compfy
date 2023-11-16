# Compfy
See [What is This](https://github.com/allusive-dev/compfy#what-is-this)

<br>
<br>

# Update

Now that Compfy has publically released I want to make a few things clear.
- Compfy will continue to recieve updates based on `yshui/picom`'s stable releases.
- Compfy is no longer considered a fork of Picom, it is its own compositor based upon Picom.


**There is now a live matrix chat room for Compfy/Picom-Allusive. Join us [here](https://matrix.to/#/#compfy-discussion:matrix.org)**

<br>
<br>


Want to chat or maybe help bug test? Contatct me here:

[![Matrix](https://img.shields.io/badge/MATRIX-012121.svg?style=for-the-badge&logo=Matrix&logoColor=white)](https://matrix.to/#/@allusive_:matrix.org)
[![Discord](https://img.shields.io/badge/DISCORD-5865F2.svg?style=for-the-badge&logo=Discord&logoColor=white)](https://github.com/allusive-dev/allusive-dev#contact-me)
[![Email](https://img.shields.io/badge/EMAIL-160F33.svg?style=for-the-badge&logo=ProtonMail&logoColor=white)](mailto:jasper@allusive.dev)

Thanks very much for the support on this project recently, it really helps me stay motivated to keep working on it.
Can we get to 100 stars on GitHub next?

**If you are feelling really generous I now have GitHub sponsors setup so you can support my work more directly.
Even if you can only give a small amount it goes a long way!**

[![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/allusive-dev)

### Sponsors
Thank you to the following people who make this work possible!

[@SolninjaA](https://github.com/SolninjaA) ($5 One Time) (The First Ever Sponsor!)
[@maclightning2](https://github.com/maclightning2) ($3 A Month) (First Ever Monthly Sponsor)

## Announcements

Please check out the updated documentation.

Current Featueres:

- Includes all fixes and changes from `yshui/picom-v10.2`
- Includes pijulius animation code. (

    **As of `1.2.0` `animation-for-workspace-in`, `animation-for-workspace-out`, `animation-for-transient-window` have been removed because their corrosponding functions caused the issue of the wrong animations playing in all other instances, Aswell as not working as intended**
  
  )
- Includes corners-rule. Allowing you to set the corner-radius on a per window basis.
- Animation open and unmap exclusion lists! Don't want something animating? Now you can fix that.
- Blur rules. Background blurring can now be done on a whitelist basis to reduce hardware consumption.
- Fixes rounded corner issues on AwesomeWM, bspwm and i3.
- A New option, `wm-support` has been added. Applies patches for ("awesome", "dwm", "herb"). "herb" being HerbstluftWM.
- Adds `inactive-exclude` and `active-exclude`. See Wiki or Donument for more information.

## What Is This?

For those who don't know this is a compositor for Linux and the X11 platform. It gives windows transparency, blur, animations and much more!

Compfy provides all the features from `Picom` whilst implementing many more and also receiving frequent bugfixes as issues come up.

This is currently the best actively maintained X11 Compositor adding proper animations and more features as requested by the community!

## Documentation/Wiki.

The Wiki is also avaliable and actively updated on [Donument](https://donument.com/d/Allusive/compfy/-/documents/) an up and coming git versioned database allows for more than just code to be versioned.

The GitHub Wiki is still actively maintained just incase, so don't worry about relying 100% on a external site yet if you don't feel comfortable with that. Thought I highly encourage taking a good look at Donument.

Can't find what you need in the wiki or have an problem? Open an Issue.

## Installation

### Building Manually
```
$ meson setup . build
$ ninja -C build
$ ninja -C build install
```

Dependencies:

```
libconfig
libdbus
libev
libglvnd
libx11
libxcb
libxdg-basedir
pcre2
pixman
uthash
xcb-util-image
xcb-util-renderutil
gcc (make)
git (make)
meson (make)
ninja (make)
```

### Arch Linux or other Arch based distros

```
$ paru -S compfy
```
or
```
$ yay -S compfy
```

### NixOS

Compfy is not yet avaliable on unstable(23.11)

Coming soon though.

Thank you for your patience.
