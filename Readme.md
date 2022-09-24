#  How to create service account with mobile phone using termux
- First install termux on your phone and You can download Termux here by click below link
- [version 0.118](https://github.com/termux/termux-app/releases/download/v0.118.0/termux-app_v0.118.0+github-debug_universal.apk)

After complete installation process, run below cmd on termux.
```
termux-setup-storage
```
```
pkg update
```
```
pkg upgrade 
```
```
pkg install git
```
```
pkg install python
```
```
pip install --upgrade pip
```
```
mkdir /sdcard/MyTermux/ -p
```
```
cd /sdcard/MyTermux
```
```
git clone https://github.com/luccawill/saaccount
```
```
cd /sdcard/MyTermux/saaccount
```
```
pip3 install -r requirements.txt
```
You can get credentials.json file from [Google Console](https://console.cloud.google.com/?pli=1)

```
python3 gen_sa_accounts.py --quick-setup -1
```
```
python3 gen_sa_accounts.py  --download-keys Your Project ID
```

```
python generate_drive_token.py
```
```
cd accounts
```
```
python3 emails.py
```


