# i3lock-color

### اگر میخواین که یک i3lock خوشگل مثل پایین داشته باشین با من همراه باشید 

![i3lock-color in action](examples/screenshot.png "Screenshot sample")

## Installation

- [Arch Linux](#arch-linux) 👈 **choose this if confused or uncertain**
- [Ubuntu Linux](#ubuntu-linux)


### Arch Linux

#### برای نصب کردن توی محیط arch اول از همه با کامند پایین i3lock رو نصب کنید

```
sudo pacman -S i3lock
```

### بعد از نصب کردن دستور زیر رو به ترتیب وارد کنید توی ترمینال

```
git clone https://aur.archlinux.org/i3lock-color.git
cd i3lock-color
makepkg -Acs
sudo pacman -U i3lock-color-2.13.c.5-1-x86_64.pkg.tar.zst
```

## اجرا کردن i3lock زیبا

### بعد از نصب اتمام مراحل بالا و انجام نصب به ادرس پایین میریم و یک پوشه به اسم scripts میسازیم و بعد فایل lockرو داخل این پوشه قرار بدین

```
mkdir -p .config/scripts
```


### بعد از انجام این کارا برین داخل مسیر زیر

```
vim .config/i3/config
```

### متن زیر رو داخل اون قرار بدین

```
bindsym $mod+x exec /home/ali/.config/scripts/lock
```

### الان شما یک بار i3 خود را refresh کنید و کلد mod+x$  را بزنید (دکمه پنجره بعلاوه x)

### Ubuntu Linux

#### توی قدم اول دستور پایین رو اجرا میکنیم که نیازمندی هاش نصب بشه
```
sudo apt install autoconf gcc make pkg-config libpam0g-dev libcairo2-dev libfontconfig1-dev libxcb-composite0-dev libev-dev libx11-xcb-dev libxcb-xkb-dev libxcb-xinerama0-dev libxcb-randr0-dev libxcb-image0-dev libxcb-util-dev libxcb-xrm-dev libxkbcommon-dev libxkbcommon-x11-dev libjpeg-dev
```

#### بعد از اجرا کردن این دستور میریم سراغ مخزن و اونو clone میکنیم
```
git clone https://github.com/Raymo111/i3lock-color.git
cd i3lock-color
```

#### بعد یکی از دو دستور پایین رو اجرا میکنیم
##### To build without installing, run:
```
./build.sh
```

##### To build AND install, run:
```
./install-i3lock-color.sh
```

#### بعد از انجام این کارها میریم توی پوشه examples و فایل lock.sh رو میبریم به ادرس پایین و توی فایل config هم برای اون یک کلید میان بر میسازیم
‍‍‍‍
```
cp lock.sh ~/.config/scripts/
```

```
bindsym $mod+x exec /home/ali/.config/scripts/lock.sh
```
