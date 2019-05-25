# mouseacc

I was bored one night so made a bash script to toggle mouse acceleration for mac.

It works by using the command:

```bash
defaults write .GlobalPreferences com.apple.mouse.scaling $val
```

The only issue with this approach is that your mouse sensitivity will be locked but since [smoothmouse.com](smoothmouse.com) is no longer supported, and I could not find any free solutions without ads or prompts to pay for the full version, I decided created this as any easy way to toggle it on and off.

## Usage

If you don't know how to execute a bash script - you can't go wrong with this [guide](https://www.taniarascia.com/how-to-create-and-use-bash-scripts/).

```bash
mouseacc [-r | -w [-1|1] | -d]

options:
-r, --read                read the current value (-1 = off, 1 = on)
-w, --write               set value (-1 = off, 1 = on)
-d, --remove-setting      remove the mouseacc setting and use system default
```

Also a reboot/loginlogout is required for a change to take place.


Enjoy!
