## نصب OpenVPN
اسکریپت نصب OpenVPN برای سیستم‌عامل‌های اوبونتو، دبیان، آلما‌لینوکس، راکی لینوکس، سنت‌اویس و فدورا.

این اسکریپت به شما اجازه می‌دهد در کمتر از یک دقیقه سرور VPN خود را راه‌اندازی کنید، حتی اگر تا به حال از OpenVPN استفاده نکرده باشید. این اسکریپت به گونه‌ای طراحی شده است که تا حد امکان ساده و همه‌کاره باشد.

### نصب و راه‌اندازی
اسکریپت را دانلود و اجرا کرده و مراحل را دنبال کنید:

#### روش اول (پیشنهادی):
```bash
wget https://raw.githubusercontent.com/aminiyt1/openvpn-install/master/openvpn-install.sh -O openvpn-install.sh && chmod +x openvpn-install.sh && ./openvpn-install.sh
```

#### روش دوم (جایگزین):
```bash
apt update&&apt install unzip&&unzip -j openvpn-install-master.zip
```

### دستور بازکردن منو ، ساخت و دریافت کانفیگ :
```bash
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

