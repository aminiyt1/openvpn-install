**جدید: [wireguard-install](https://github.com/Nyr/wireguard-install) نیز در دسترس است.**

## نصب OpenVPN
اسکریپت نصب OpenVPN برای سیستم‌عامل‌های اوبونتو، دبیان، آلما‌لینوکس، راکی لینوکس، سنت‌اویس و فدورا.

این اسکریپت به شما اجازه می‌دهد در کمتر از یک دقیقه سرور VPN خود را راه‌اندازی کنید، حتی اگر تا به حال از OpenVPN استفاده نکرده باشید. این اسکریپت به گونه‌ای طراحی شده است که تا حد امکان ساده و همه‌کاره باشد.

### نصب و راه‌اندازی
اسکریپت را دانلود و اجرا کرده و مراحل را دنبال کنید:

#### روش اول (پیشنهادی):
```bash
wget [https://raw.githubusercontent.com/aminiyt1/openvpn-install/master/openvpn-install.sh](https://raw.githubusercontent.com/aminiyt1/openvpn-install/master/openvpn-install.sh) -O openvpn-install.sh && chmod +x openvpn-install.sh && ./openvpn-install.sh
```

#### روش دوم (جایگزین):
```bash
apt update && apt install unzip && unzip -j openvpn-install-master.zip
bash openvpn-install.sh
```

پس از اتمام نصب، می‌توانید دوباره اسکریپت را اجرا کنید تا کاربران جدید اضافه کنید، کانفیگ‌ها را مشاهده یا پاک کنید و یا کلاً OpenVPN را از روی سرور حذف کنید.

---
**رفع مشکل (Troubleshooting):**
در صورتی که پس از نصب، سرویس فعال نشد و کار نکرد، از دو دستور زیر استفاده کنید:
```bash
systemctl enable openvpn@server
reboot
```
---

### من سرور VPN می‌خواهم اما سروری ندارم
می‌توانید یک VPS با هزینه مقرون‌به‌صرفه از ۲ یورو یا ۲ دلار در ماه از [AlphaVPS](https://alphavps.com/clients/aff.php?aff=474&pid=457&currency=1) تهیه کنید.

### حمایت مالی
اگر تمایل به قدردانی و حمایت مالی دارید، می‌توانید از طریق [PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=VBAYDL34Z7J6L) یا [ارز دیجیتال](https://pastebin.com/raw/M2JJpQpC) این کار را انجام دهید. با تشکر!

### حامیان
به دنبال VPN بدون درگیری با ترمینال هستید؟ راه‌اندازی با یک کلیک + VPS رایگان در ۳ دقیقه. [Clever VPN](https://www.clever-vpn.net/en/landing-vpn?wg-referral=01LOULuQoi) را امتحان کنید.
