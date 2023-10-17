# i3lock-color

### اگر میخواین که یک i3lock خوشگل مثل پایین داشته باشین با من همراه باشید 

![i3lock-color in action](examples/screenshot.png "Screenshot sample")


## Dependencies
The following dependencies will need to be installed for a successful build, depending on your OS/distro.

### Arch Linux

#### برای نصب کردن توی محسط arch اول از همه با کامند پایین i3lock رو نصب کنید

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

### بعد از نصب اتمام مراحل بالا و انجام نصب به ادرس پایین میریم و یک پوشه به اسم scripts میسازیم

```
mkidr .config/scripts
touch .config/scripts/lock
```

### بعد فایلتون رو با یک ویرایشگرم متن باز کنید که من از vim استفاده میکنم و بعد محتویات فایل lock رو داخل اون کپی کن

### بعد از انجام این کارا برین داخل مسیر زیر و خط کد زیر رو اضافه کنید و دقت کنید که از قبل وجود نداشته باشه که خطا نگیرین

```
vim .config/i3/config
```

### متن زیر رو کپی کنید

```
bindsym $mod+x exec /home/ali/.config/scripts/lock
```

### الان شما یک بار i3 خود را رفرش کنید و کلد $mod+x را بزنید
