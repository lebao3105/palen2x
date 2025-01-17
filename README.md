<p align="center">
    <img src="https://cdn.discordapp.com/attachments/1017854329887129611/1068174531048513596/Palen1x.png" alt="logo" width="250">
</p>
<br>
<p align="center">
<strong>Linux distro that lets you install <a href="https://github.com/palera1n/palera1n">palera2n</a>.</strong><br>
    It aims to be easy to use, have a nice interface and support 32 and 64 bit CPUs.
</p>
<p align="center">
    <a href="#Information">Information</a> •
    <a href="#contributing">Contributing</a> •
    <a href="#credits">Credits</a> •
    <a href="https://github.com/palera1n/palen1x/blob/main/CHANGELOG.md">Changelog</a> • 
    <a href="https://dsc.gg/palera1n">Support Discord</a> 
</p>

<p align="center">
    <img src="https://cdn.discordapp.com/attachments/1017854329887129611/1068153144305008730/IMG_0807.png" alt="screenshot" width="950">
</p>

-------
## Warnings
- Use `-f -c` or `-f -B` for Rootful when creating fakeFS/bindFS, you also must use *only* `-f` to boot fakeFS/bindFS, otherwise it'll spit out an error saying that you already created the fakeFS/bindFS or it'll freeze without fakeFS/bindFS.
    - (`-f -B` won't work on 16.x). 

- This distro's purpose is to make [palera1n](https://github.com/palera1n/palera1n) easier and more intuitive(with TUI) to use within a stripped down distribution. Each option in `palera1n_options` correlates to what can be found in palera1n documentation. I am not including flags that the user will most likely never need, for example, `-i`. Further documentation on [palera1n](https://github.com/palera1n/palera1n) can be found [here](https://cdn.nickchan.lol/palera1n/artifacts/c-rewrite/palera1n.1.html).

- `A9 and below` devices may need to rerun the jailbreak if it gets stuck on PongoOS booting. If palera1n is stuck, press `CTRL + C` and type `exit` to go back into palen1x_menu, and rerun palera1n (make sure you don't force reboot, if you do you may need to rerun this process).

- On `A11`, **you must disable your passcode while in the jailbroken state** (on iOS 16, you need to reset your device before proceeding with palera1n on `A11`).

## Information
**Make an [iCloud/iTunes backup](https://support.apple.com/en-us/HT203977) before using, so that you can go back if something goes wrong**.

- Downloads for palen2x can be found [here](https://github.com/infinite989/palen2x/releases). 

- Guide for palen2x can be found [here](https://ios.cfw.guide/using-palen1x/).

###### Older downloads can be found [here](https://cdn.nickchan.lol/palera1n/artifacts/palen1x/)

## Building palen2x
To change the version of palen1x, either change `version` file, or manually specify it with `./build.sh`.

```sh
git clone https://github.com/infinite989/palen2x.git
cd palen2x
sudo ./build.sh RELEASE
```

The iso will be placed in work/.

## Run palen2x locally

Only for palera1n supported OSes (and probably Windows doesnot get invited, sorry)

Get whiptail first.

Get this repo cloned (if you haven't before), "cd" to it, then run these as root:

```bash
# find ./scripts -type f -not -iname 'inetcat' -exec cp -p '{}' '/usr/bin' ';'
# echo "Rootless" > /usr/bin/.jbtype
# echo "" > /usr/bin/.args
```

Start by running palen2x_menu.

## Important Notes
**make sure to flash with dd flashing with iso mode will cause issues
i recommend to use rufus to flash it**

Ventoy works too, but booting with GRUB mode may required.

## Credits
- Asineth for [checkn1x](https://github.com/asineth0/checkn1x)
- raspberryenvoie for [odysseyn1x](https://github.com/raspberryenvoie/odysseyn1x)
- [Everyone else who contributed to palen1x](https://github.com/palera1n/palen1x/graphs/contributors)
- ImmortalShad0w for adding and improving palen1x [palen2x](https://github.com/infinite989/palen2x)
