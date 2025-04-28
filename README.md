# Built with QMK

# Links
ZMK Repo - https://github.com/zmkfirmware/zmk/
ZMK OLED - https://github.com/mctechnology17/zmk-nice-oled
Pipeline ref - https://www.youtube.com/watch?v=O_urj-rF3bQ&ab_channel=JoeScotto

NOTE: Do this before cloning the repo locally. Running below is like running `git clone`.

REPO init - `bash -c "$(curl -fsSL https://zmk.dev/setup.sh)"`

```
❯ bash -c "$(curl -fsSL https://zmk.dev/setup.sh)"

Keyboard Selection:
 1) 2% Milk		       43) Leeloo-Micro
 2) A. Dux		       44) Lily58
 3) Advantage 360 Pro	       45) Lotus58
 4) BAT43		       46) MakerDiary m60
 5) BDN9 Rev2		       47) Microdox
 6) BFO-9000		       48) Microdox V2
 7) Boardsource 3x4 Macropad   49) MurphPad
 8) Boardsource 5x12	       50) Naked60
 9) BT60 V1 Hotswap	       51) Nibble
10) BT60 V1 Soldered	       52) nice!60
11) BT60 V2		       53) nice!view
12) BT65		       54) nice!view adapter
13) BT75 V1		       55) Osprette
14) Chalice		       56) Pancake
15) Clog		       57) Planck Rev6
16) Contra		       58) Preonic Rev3
17) Corne		       59) QAZ
18) Corneish Zen v1	       60) Quefrency Rev. 1
19) Corneish Zen v2	       61) Redox
20) Cradio/Sweep	       62) REVIUNG34
21) CRBN Featherlight	       63) REVIUNG41
22) eek!		       64) REVIUNG5
23) Elephant42		       65) REVIUNG53
24) Ergodash		       66) Romac Macropad
25) Eternal Keypad	       67) Romac+ Macropad
26) Eternal Keypad Lefty       68) S40NC
27) Ferris 0.2		       69) SNAP
28) Fourier Rev. 1	       70) Sofle
29) Glove80		       71) splitkb.com Aurora Corne
30) Helix		       72) splitkb.com Aurora Helix
31) Hummingbird		       73) splitkb.com Aurora Lily58
32) Iris		       74) splitkb.com Aurora Sofle
33) Jian		       75) splitkb.com Aurora Sweep
34) Jiran		       76) Splitreus62
35) Jorne		       77) TesterProMicro
36) KBDfans Tofu65 2.0	       78) TesterXiao
37) Knob Goblin		       79) TG4x
38) Kyria		       80) Tidbit Numpad
39) Kyria Rev2		       81) Waterfowl
40) Kyria Rev3		       82) ZMK Uno
41) Leeloo		       83) Zodiark
42) Leeloo v2		       84) Quit
❯ Pick a keyboard: 17

MCU Board Selection:
 1) Adafruit KB2040		 14) nRFMicro 1.1 (flipped)
 2) Adafruit QT Py RP2040	 15) nRFMicro 1.1/1.2
 3) BlackPill F401CC		 16) nRFMicro 1.3/1.4
 4) BlackPill F401CE		 17) nRFMicro 1.3/1.4 (nRF52833)
 5) BlackPill F411CE		 18) PillBug
 6) BlueMicro840 v1		 19) Puchi-BLE V1
 7) BoardSource blok		 20) QMK Proton-C
 8) Mikoto			 21) Seeed Studio XIAO nRF52840
 9) nice!nano v1		 22) Seeed Studio XIAO RP2040
10) nice!nano v2		 23) Seeed Studio XIAO SAMD21
11) Nordic nRF52840 DK		 24) SparkFun Pro Micro RP2040
12) Nordic nRF5340 DK		 25) Quit
13) nRF52840 M.2 Module
❯ Pick an MCU board: 10
❯ Copy in the stock keymap for customization? [Yn]: y
❯ GitHub Username (leave empty to skip GitHub repo ❯ creation): andrewknoesen
❯ GitHub Repo Name [zmk-config]: corne
❯ GitHub Repo [https://github.com/andrewknoesen/corne.git]: git@github.com:andrewknoesen/corne.git

Preparing a user config for:
* MCU Board: nice_nano_v2
* Shield(s): corne_left corne_right
* Copy Keymap?: ✓
* GitHub Repo To Push (please create this in GH first!): git@github.com:andrewknoesen/corne.git

❯ Continue? [Yn]: y
Cloning into 'corne'...
remote: Enumerating objects: 60, done.
remote: Counting objects: 100% (17/17), done.
remote: Compressing objects: 100% (10/10), done.
remote: Total 60 (delta 8), reused 7 (delta 7), pack-reused 43 (from 2)
Receiving objects: 100% (60/60), 9.43 KiB | 9.43 MiB/s, done.
Resolving deltas: 100% (13/13), done.
~/Documents/Projects/Personal/corne/corne/config ~/Documents/Projects/Personal/corne/corne
Downloading config file (https://raw.githubusercontent.com/zmkfirmware/zmk/main/app/boards/shields/corne/corne.conf)
Downloading keymap file (https://raw.githubusercontent.com/zmkfirmware/zmk/main/app/boards/shields/corne/corne.keymap)
~/Documents/Projects/Personal/corne/corne
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint:
hint: 	git config --global init.defaultBranch <name>
hint:
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint:
hint: 	git branch -m <name>
Initialized empty Git repository in /Users/andrew/Documents/Projects/Personal/corne/corne/.git/
[master (root-commit) a874ce6] Initial User Config.
 7 files changed, 109 insertions(+)
 create mode 100644 .github/workflows/build.yml
 create mode 100644 boards/shields/.gitkeep
 create mode 100644 build.yaml
 create mode 100644 config/corne.conf
 create mode 100644 config/corne.keymap
 create mode 100644 config/west.yml
 create mode 100644 zephyr/module.yml
Enter passphrase for key '/Users/andrew/.ssh/id_rsa':
Enumerating objects: 15, done.
Counting objects: 100% (15/15), done.
Delta compression using up to 8 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (15/15), 2.50 KiB | 2.50 MiB/s, done.
Total 15 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:andrewknoesen/corne.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.
```