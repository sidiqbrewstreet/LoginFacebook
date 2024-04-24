# Project Description
SecretKeyFacebook Merupakan Perpustakaan Python Untuk Melakukan Login Terhadap Platfrom [Facebook](https://www.facebook.com) Melalui Portal Windows Dan Android. Project ini Dibuat Menggunakan User Agent Yang Bawaan Sesuai Portal Login. Tidak Perlu Khawatir Anda Dapat Menggunakan User Agent Andalan Anda Untuk Melakukan Verifikasi AOUTH Sebagaimana Yang Saya Contohkan Dibawah ini:

```python
# Example User Agent

# for Facebook API  = 'com.facebook.katana'
# for Messenger API = 'com.facebook.orca'

UserAgent_Windows   = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36'
UserAgent_android   = 'Dalvik/2.1.0 (Linux; U; Android 7.1.2; SM-G977N Build/LMY48Z) [FBAN/FB4A;FBAV/417.0.0.33.65;FBPN/com.facebook.katana;FBLC/in_ID;FBBV/480086274;FBCR/Corporation Tbk;FBMF/samsung;FBBD/samsung;FBDV/SM-G977N;FBSV/7.1.2;FBCA/x86:armeabi-v7a;FBDM/{density=1.5,width=720,height=1280};FB_FW/1;FBRV/0;]'
UserAgent_messenger = 'Dalvik/2.1.0 (Linux; U; Android 7.1.2; SM-G977N Build/LMY48Z) [FBAN/Orca-Android;FBAV/417.0.0.33.65;FBPN/com.facebook.orca;FBLC/in_ID;FBBV/480086274;FBCR/Corporation Tbk;FBMF/samsung;FBBD/samsung;FBDV/SM-G977N;FBSV/7.1.2;FBCA/x86:armeabi-v7a;FBDM/{density=1.5,width=720,height=1280};FB_FW/1;FBRV/0;]'
```
<br>
<br>

# Feature
**Login From Website (Windows)**
- Login Reguler
- Login Validate
- Login Async

**Login From API (Android)**
- Login Reguler
- Login Validate
- Login Messenger

<br>
<br>

# Installation
```python
pip install secretkeyfacebook
```
<br>

# How To Use
**From Login Windows**
```python
from secretkeyfacebook import Reguler

def LoginWithReguler(email=email, password=password, UserAgent=UserAgent):
    response = Reguler(email=email, password=password, UserAgent=UserAgent)
```
```python
from secretkeyfacebook import Validate

def LoginWithValidate(email=email, password=password, UserAgent=UserAgent):
    response = Validate(email=email, password=password, UserAgent=UserAgent)
```
```python
from secretkeyfacebook import Validate

def LoginWithAsync(email=email, password=password, UserAgent=UserAgent):
    response = Async(email=email, password=password, UserAgent=UserAgent)
```
<br>

**From Login Android**
```python
from secretkeyfacebook import Reguler_API

def LoginWithReguler_API(email=email, password=password, UserAgent=UserAgent):
    response = Reguler_API(email=email, password=password, UserAgent=UserAgent)
```
```python
from secretkeyfacebook import Validate_API

def LoginWithValidate_API(email=email, password=password, UserAgent=UserAgent):
    response = Validate_API(email=email, password=password, UserAgent=UserAgent)
```
```python
from secretkeyfacebook import Messenger_API

def LoginWithMessenger_API(email=email, password=password, UserAgent=UserAgent):
    response = Messenger_API(email=email, password=password, UserAgent=UserAgent)
```

# Error Message
```python
# Jika Kredensial Tidak Valid/Tidak Terpenuhi
error_user_msg = "{'error':{'status':'400 Bad Request','status_code': 400,'data':{'email':None,'password':None}},'message':'Username and Password dont exist'}"
```
```python
# Jika Kredensial Tidak Valid/Tidak Terpenuhi
error_user_msg = "{'error':{'status':'400 Bad Request','status_code': 400,'data':{'email':None,'password':None}},'message':'Username and Password dont exist'}"
```
