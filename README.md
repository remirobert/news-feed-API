# API

**base_url** : http://remirobert.com:4242

#Authentification

##Signup
create a new user

  - **Method**     : POST
  - **route**      : {{base_url}}/signup
  - **parameters** :
```json
{
  email: "",
  password: ""
}
```
  - **response**   :
 ```json
  {
  "user": {
    "id": "397e1d8b-7cd1-43ae-8bbf-4b8ae5defef0",
    "email": "user1@gmail.com",
    "password": "email"
  },
  "token": {
    "accessToken": "GDRYFXAIATTGEBLP9JX6W03T3IPFX041EA8K8H3KV2898RHO3I0K7Q994C6G64Z0IMPOB2IOE2CZBO1Y6GHD6DD6I0IIHD4GMDOA1XU49LSG99YV48Y5XL7Z92ERB5PSHM7F91OX8BG1YWW0C083SQI929GFVUXMP7HXATNG8AIS5TUPGWRM3J20CGKGM95GFTUY5SORCPYFFKDAKEW4NG43APIQBHZNSSU3ZQX2AMY5JWA2IBJ52AUER858D31X",
    "refreshToken": "TUCOC1X9T9YJSNQZMWPAFG6W79L4YSG5LTXJJV5Q41S011HSTFMBMTVCD80V2Z6S05PIOZ5FCM2OBC4HF0F2929ZMPONT50E399Y2O4WT5AGLEV6EY40JN124A81HBJF2IT167M6W7HJXCP32O7XXXRICRLVHHHNN4L126VLID8NEWCLB5MZYIZ6VYK1W0MQPL61BU7S0PGJ5Z7TZR7L79ENSK8JBV7N0T4ZPM2PXXJE6O2VZZDETBEVXNR109TH",
    "expireDate": "Wed Jan 11 18:30:43 EST 2017"
  }
}
 ```
 
##Login
authentificate user to get access, and refresh token

  - **Method**     : POST
  - **route**      : {{base_url}}/auth
  - **parameters** :
```json
{
  email: "",
  password: ""
}
```
  - **response**  :
 ```json
 {
  "accessToken": "GS6T805VODRVV964OHTIRQKE65GQF2DGFXV13QLDGR6QR3E1J9ZUZSFUTKC2RRFHF92ANGGATI447867NUCYEZYA253HPYSDC4XQZGNHCL6EG1KS7DGG71ANQCM3DAO5FNNE6E1TAQJ15L7SYHA6J17FRF4AQQ50ORU6RGZAL42ZSZ6KRKTSQLERPW0OQ4UC2180HU5RPBZLL8HFWF8KFILTFX454IQMSS22JRNBTNVCJLEH0WZRNOY2JTVWSND3",
  "refreshToken": "RZV1BNCX0O0MUH1YL42HRZIKOHXF0ALRJSJTO4YQR8DUGF6DXZNZCRDHSQDSSF8OF0AEMJSGXKFHJJD7JOWJ3UIGSOUBP4YBW4XDBUZW1EGBCP3VUADP13ITD8PPQ4JZ3KKNH9N7FF1NP60PSD6ME54DHI9B3OLPQCWOYLFHV9UUCOUNCAP9ZFT9E7Y79VDACE93AQM2QF75PRUUOCVB5FX8XEJH1NS57666H0W7D8Q23LQT1MX65UIZ8L4J9G8G",
  "expireDate": "Wed Jan 11 18:31:02 EST 2017"
}
 ```
