```bash
rm -rf pixo
git clone https://github.com/PleaseCompile/CTFd-theme-pixo.git pixo
chown -R ctfd:www-data pixo
chmod -R 755 pixo
```

**คำอธิบายสั้นๆ**

* `rm -rf pixo` → ลบโฟลเดอร์เดิมออก (ถ้ามี)
* `git clone ... pixo` → clone แล้วตั้งชื่อโฟลเดอร์เป็น `pixo`
* `chown -R ctfd:www-data` → ตั้ง owner/group ให้เหมือน theme อื่น
* `chmod -R 755` → ให้สิทธิ์อ่าน-รัน / เขียนเฉพาะ owner

💡 หลังจากนั้น restart CTFd:

```bash
sudo systemctl restart ctfd
```

หรือถ้าใช้ `gunicorn` manual:

```bash
sudo systemctl restart ctfd.service
```

ถ้าต้องการ version ultra-short แบบยิงทีเดียว:

```bash
rm -rf pixo && git clone https://github.com/PleaseCompile/CTFd-theme-pixo.git pixo && chown -R ctfd:www-data pixo && chmod -R 755 pixo && systemctl restart ctfd
```



# Pixo Theme
Pixo is a Retro Styled Theme for CTFd which consists of numerous features like OLD CRT like flicker, Old school fonts and notification sound which gives the theme a 90s look.

Compatible with CTFd **Version 3.3.0**

Few Screenshots:
  
  ![Index Page](https://i.imgur.com/lL7zYrg.gif "Index Page")
  
  ![Challenge Page](https://i.imgur.com/o1XHK2t.png "Challenge Page")
  
  ![Challenge Popup](https://i.imgur.com/7YAQFs5.png "Challenge Popup")
  
  ![Score Board](https://i.imgur.com/COI4yAo.png "Score Board")
  
  ![Login Page](https://i.imgur.com/206O99m.png "Login Page")


### Installation Steps:
Open your Docker container's terminal then insert the following Command:
```
git clone https://github.com/hmrserver/CTFd-theme-pixo.git /opt/CTFd/CTFd/themes/pixo
```
Then Login as Admin and go to: ```Admin Panel > Config > Themes``` and switch the Theme to pixo and Click on Update.

That's it! Now you are good to goo..

## Custom License
1. User may edit the item, but can't replace My Theme Copyright & CTFd Copyright.
1. User need confirmation with us before removing copyright mark (footer).


## Credits
- [Freepik](https://www.freepik.com "Freepik") For their awesome images (Arrow & Coin).
- [CTFd](https://github.com/CTFd "CTFd") For Creating such an Awesome Platform.
