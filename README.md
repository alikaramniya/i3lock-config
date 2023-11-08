# i3lock-color

### اگر میخواین که یک i3lock خوشگل مثل پایین داشته باشین با من همراه باشید 

![i3lock-color in action](examples/screenshot.png "Screenshot sample")

## installation
### [arch](#Arch)
### [ubuntu](#Ubuntu)
## Installation

- [Manual](#manual) 👈 **choose this if confused or uncertain**
- [Oh My Zsh](#oh-my-zsh)
- [Prezto](#prezto)
- [Zim](#zim)
- [Antibody](#antibody)
- [Antidote](#antidote)
- [Antigen](#antigen)
- [Zplug](#zplug)
- [Zgen](#zgen)
- [Zplugin](#zplugin)
- [Zinit](#zinit)
- [Zi](#zi)
- [Zap](#zap)
- [Homebrew](#homebrew)
- [Arch Linux](#arch-linux)
- [Alpine Linux](#alpine-linux)
- [Fig](#fig)

### Manual

```zsh
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
```

Users in China can use the official mirror on gitee.com for faster download.<br>
中国用户可以使用 gitee.com 上的官方镜像加速下载.

```zsh
git clone --depth=1 https://gitee.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
```

This is the simplest kind of installation and it works even if you are using a plugin manager. Just
make sure to disable the current theme in your plugin manager. See
[troubleshooting](#cannot-make-powerlevel10k-work-with-my-plugin-manager) for help.

### Oh My Zsh

1. Clone the repository:
    ```zsh
    git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
    ```
    Users in China can use the official mirror on gitee.com for faster download.<br>
    中国用户可以使用 gitee.com 上的官方镜像加速下载.

    ```zsh
    git clone --depth=1 https://gitee.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
    ```
2. Set `ZSH_THEME="powerlevel10k/powerlevel10k"` in `~/.zshrc`.

### Prezto

Add `zstyle :prezto:module:prompt theme powerlevel10k` to `~/.zpreztorc`.


#### Dependencies

# Arch Linux

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

# Ubuntu
