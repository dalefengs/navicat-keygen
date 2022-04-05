**请支持正版！ 该项目不是本人开发，备份已被删除的 navicat-keygen， 仅用于个人学习！不要用于非法用途！**
# 提取 AppImage 文件

**cp的时候可能比较久请耐心等待  尽量目录一致**

```
mkdir navicat15-premium-cs
sudo mount -o loop navicat15-premium-cs.AppImage navicat15-premium-cs
sudo cp -r navicat15-premium-cs navicat
sudo umount navicat15-premium-cs
rm -rf navicat15-premium-cs
```

## 编译 Navicat Keygen

## 前提条件

**你的gcc支持C++17特性**

请确保你安装了下面几个库：

- `capstone`
- `keystone`
- `rapidjson`
- `openssl`

## 安装 capstone

```
yay -S capstone
```

## 安装 keystone

1. aur仓库（推荐）

   ```
   yay -S keystone
   ```

2. 编译安装

> 编译安装（这里时间比较久，耐心等待会...）

```
git clone https://github.com/keystone-engine/keystone.git
cd keystone
mkdir build
cd build
../make-share.sh
sudo make install
sudo ldconfig
```

## 安装 rapidjson

```
yay -S rapidjson
```

## 安装 openssl

```
yay -S openssl
```

## 编译安装

```
git clone -b linux --single-branch https://github.com/Orginly/navicat-keygen.git
cd navicat-keygen
make all
```

**生成完成后，你会在 `./bin` 文件夹下看到编译后的keygen/patcher。**

# navicat-patcher 替换官方公钥



```
sudo ./bin/navicat-patcher ../navicat
```

## 样例输出

```
**********************************************************
*       Navicat Patcher (Linux) by @DoubleLabyrinth      *
*                  Version: 1.0                          *
**********************************************************

Press ENTER to continue or Ctrl + C to abort.

[+] Try to open libcc.so ... Ok!

[+] PatchSolution0 ...... Ready to apply
    RefSegment      =  1
    MachineCodeRva  =  0x0000000001377200
    PatchMarkOffset = +0x000000000292c840

[*] Generating new RSA private key, it may take a long time...
[*] Your RSA private key:
    -----BEGIN RSA PRIVATE KEY-----
    MIIEowIBAAKCAQEAta5uHinxzLei/iSOBu/Nf8y3X/BuGpmFcxacQIKb60amSHL4
    vg0RaoWs3f04PapKSX+uGeWjhOzWX9UxRXj2xi1FeNgIKDa9+1cLKIvrOVlTlrpx
    irXbOvGkF+uOd2mbEd11LgLwbnTKNoqWZuPHPh3hgUWF+fZ6/7rLuWrh+8K/OlHU
    hOjgKZWoGxO7dXQhDav+iDxW7ab/s5B5/OJcwv+IvI3ZakL12C2fNKYcLtkonCTl
    TyTvq/Q/bBLxoTxzgvkkanv+H99Sd4WuANA6Sk0Tu9vfC2jByVpWlp7OAwOmWVCf
    k7YDoLNQtjONBMEE9+sKr3lxyaJ3+SAC2ity+QIDAQABAoIBAHPi1lShNp35SJtJ
    H9rm3TK2lwU4LFMFN+0oL/SqGuBhCTHPPEClv0UuDQzwNw6Gb6ogKiJUqw/frgIk
    z6/br7TLLbQeQF2+RUJrzC9JyHmlM79CH6h1xWf8uEmVtCMRFpu3ocX+k/QwxMcz
    cSoiAnXpw2yctw+xG9XBBa+4sHrQMkY4VT+gx3W5kvrOEc24HDeiRvFUMSc+TtRd
    SMg69vkMtx2OjjWW/jIXI8XY6evhCHFqXL+1+eG9RMT73Y6LfFyb/EoXzszkHcNs
    WbS/5zwu3ZcHiaUfxp3HldW71A7UfPRLPpGT0y1IWXvCH5aL1u3JIvWUm4HDsLGo
    CRCamH0CgYEA8DNGOPnjQTsREuE/Tfuq6xLNPEj+UoL8l+c9Lu/nW8DpCYSvm65h
    1HUQYLy/IhRTA5m7EO/jaO0qmlgldccUadF4FaNdRyqfmOfcMw3mI9YeQXduS0eU
    EE4J0m2H/Q7X45huDUTKKPOTfOFyA0cqdhicCsh5ll6yjyx8Cw2gZEcCgYEAwaHB
    5Y64fS3xjfRVs2TwxzYXivGmnJBX87VMbvVeN43gFzUKdrXaKaRKHXj4QQt73EdM
    AtDWuhivv+Y1We9mcQ2TZk0Oew+2CSnLm7rW9OAo9LvNOSaYdBXoFjDIayUfX5Ci
    FLaJTYMcWCgw97E1fxr65psh4AuPtIqepd/1Tr8CgYB+/RyrErGq0ud768nkGKGM
    FiybKpwKU2XniUE3h23xfFO3zIZq8A6YnCtEeYUzJzucM7JKigjYeEqFvwRO+Ck6
    qJusFOpDra0i0bIA6+A4IgNs6Q9OjVEiLZ/TuESk7SwGD5hfO3cFn4DiDO6R/RXd
    ybT1nndpoDcWqpYJ4fJiEQKBgQCb6UWZM7w1f2L67Hx9QI/nuBRo2n9PnaJUJ+1t
    gsDkdqazyQ+t2mvaD+Flrdwnc7m9+uKnecUMf4g0OodG7U9NRKMlQnKggFwRMMgz
    ktQ2xK/1r6pllEA5aNJB2/Hk5DVI28rGZtxTv3h5O5OCPfxXZkAUo2E5Z9XEh8GK
    yrRZPQKBgHpl9YRClcX8mL72gXzYc7m+vLsMZZrdqbhFZ9xYdvVmRdqp48lKbkTL
    sMAvHk8ACDXaPCfocbJ2Uq4XrZKk3+PA2709DAUa4lMkCxYAe71qXLv0AGfnG255
    4p4TEE4lmUFqp5C+7rzX97e/a72eXKnmjQ3RpeWs23C2UHmKOMuw
    -----END RSA PRIVATE KEY-----
[*] Your RSA public key:
    -----BEGIN PUBLIC KEY-----
    MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAta5uHinxzLei/iSOBu/N
    f8y3X/BuGpmFcxacQIKb60amSHL4vg0RaoWs3f04PapKSX+uGeWjhOzWX9UxRXj2
    xi1FeNgIKDa9+1cLKIvrOVlTlrpxirXbOvGkF+uOd2mbEd11LgLwbnTKNoqWZuPH
    Ph3hgUWF+fZ6/7rLuWrh+8K/OlHUhOjgKZWoGxO7dXQhDav+iDxW7ab/s5B5/OJc
    wv+IvI3ZakL12C2fNKYcLtkonCTlTyTvq/Q/bBLxoTxzgvkkanv+H99Sd4WuANA6
    Sk0Tu9vfC2jByVpWlp7OAwOmWVCfk7YDoLNQtjONBMEE9+sKr3lxyaJ3+SAC2ity
    +QIDAQAB
    -----END PUBLIC KEY-----

*******************************************************
*                   PatchSolution0                    *
*******************************************************
[*] Previous:
+0x0000000000000070                          01 00 00 00 05 00 00 00          ........
+0x0000000000000080  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x0000000000000090  00 00 00 00 00 00 00 00 40 c8 92 02 00 00 00 00  ........@.......
+0x00000000000000a0  40 c8 92 02 00 00 00 00 00 10 00 00 00 00 00 00  @...............
[*] After:
+0x0000000000000070                          01 00 00 00 05 00 00 00          ........
+0x0000000000000080  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x0000000000000090  00 00 00 00 00 00 00 00 d0 c9 92 02 00 00 00 00  ................
+0x00000000000000a0  d0 c9 92 02 00 00 00 00 00 10 00 00 00 00 00 00  ................

[*] Previous:
+0x000000000292c840  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c850  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c860  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c870  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c880  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c890  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c8a0  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c8b0  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c8c0  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c8d0  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c8e0  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c8f0  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c900  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c910  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c920  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c930  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c940  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c950  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c960  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c970  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c980  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c990  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c9a0  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c9b0  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
+0x000000000292c9c0  00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
[*] After:
+0x000000000292c840  ef be ad de 4d 49 49 42 49 6a 41 4e 42 67 6b 71  ....MIIBIjANBgkq
+0x000000000292c850  68 6b 69 47 39 77 30 42 41 51 45 46 41 41 4f 43  hkiG9w0BAQEFAAOC
+0x000000000292c860  41 51 38 41 4d 49 49 42 43 67 4b 43 41 51 45 41  AQ8AMIIBCgKCAQEA
+0x000000000292c870  74 61 35 75 48 69 6e 78 7a 4c 65 69 2f 69 53 4f  ta5uHinxzLei/iSO
+0x000000000292c880  42 75 2f 4e 66 38 79 33 58 2f 42 75 47 70 6d 46  Bu/Nf8y3X/BuGpmF
+0x000000000292c890  63 78 61 63 51 49 4b 62 36 30 61 6d 53 48 4c 34  cxacQIKb60amSHL4
+0x000000000292c8a0  76 67 30 52 61 6f 57 73 33 66 30 34 50 61 70 4b  vg0RaoWs3f04PapK
+0x000000000292c8b0  53 58 2b 75 47 65 57 6a 68 4f 7a 57 58 39 55 78  SX+uGeWjhOzWX9Ux
+0x000000000292c8c0  52 58 6a 32 78 69 31 46 65 4e 67 49 4b 44 61 39  RXj2xi1FeNgIKDa9
+0x000000000292c8d0  2b 31 63 4c 4b 49 76 72 4f 56 6c 54 6c 72 70 78  +1cLKIvrOVlTlrpx
+0x000000000292c8e0  69 72 58 62 4f 76 47 6b 46 2b 75 4f 64 32 6d 62  irXbOvGkF+uOd2mb
+0x000000000292c8f0  45 64 31 31 4c 67 4c 77 62 6e 54 4b 4e 6f 71 57  Ed11LgLwbnTKNoqW
+0x000000000292c900  5a 75 50 48 50 68 33 68 67 55 57 46 2b 66 5a 36  ZuPHPh3hgUWF+fZ6
+0x000000000292c910  2f 37 72 4c 75 57 72 68 2b 38 4b 2f 4f 6c 48 55  /7rLuWrh+8K/OlHU
+0x000000000292c920  68 4f 6a 67 4b 5a 57 6f 47 78 4f 37 64 58 51 68  hOjgKZWoGxO7dXQh
+0x000000000292c930  44 61 76 2b 69 44 78 57 37 61 62 2f 73 35 42 35  Dav+iDxW7ab/s5B5
+0x000000000292c940  2f 4f 4a 63 77 76 2b 49 76 49 33 5a 61 6b 4c 31  /OJcwv+IvI3ZakL1
+0x000000000292c950  32 43 32 66 4e 4b 59 63 4c 74 6b 6f 6e 43 54 6c  2C2fNKYcLtkonCTl
+0x000000000292c960  54 79 54 76 71 2f 51 2f 62 42 4c 78 6f 54 78 7a  TyTvq/Q/bBLxoTxz
+0x000000000292c970  67 76 6b 6b 61 6e 76 2b 48 39 39 53 64 34 57 75  gvkkanv+H99Sd4Wu
+0x000000000292c980  41 4e 41 36 53 6b 30 54 75 39 76 66 43 32 6a 42  ANA6Sk0Tu9vfC2jB
+0x000000000292c990  79 56 70 57 6c 70 37 4f 41 77 4f 6d 57 56 43 66  yVpWlp7OAwOmWVCf
+0x000000000292c9a0  6b 37 59 44 6f 4c 4e 51 74 6a 4f 4e 42 4d 45 45  k7YDoLNQtjONBMEE
+0x000000000292c9b0  39 2b 73 4b 72 33 6c 78 79 61 4a 33 2b 53 41 43  9+sKr3lxyaJ3+SAC
+0x000000000292c9c0  32 69 74 79 2b 51 49 44 41 51 41 42 ad de ef be  2ity+QIDAQAB....

[*] Previous:
+0x0000000001377200  44 0f b6 24 18 48 8b 44 24 28 8b 50 f8 85 d2 79  D..$.H.D$(.P...y
+0x0000000001377210  6f                                               o               
[*] After:
+0x0000000001377200  45 31 e4 48 8d 05 3a 56 5b 01 90 90 90 90 90 90  E1.H..:V[.......
+0x0000000001377210  90                                               .               

[*] New RSA-2048 private key has been saved to
    /home/orginly/Downloads/navicat-keygen/RegPrivateKey.pem

*******************************************************
*           PATCH HAS BEEN DONE SUCCESSFULLY!         *
*                  HAVE FUN AND ENJOY~                *
*******************************************************

```

# 重新打包成 AppImage

## 安装 appimagetool

> 可能需要网络代理

```
yay -S appimagetool
```

## 打包

```
appimagetool navicat navicat15.AppImage
```

# 运行 Navcat 15

```
sudo chmod +x navicat15.AppImage
./navicat15.AppImage
```

# Navicat-keygen 生成序列号和激活码

```
pwd
/home/orginly/Downloads/navicat-keygen
./bin/navicat-keygen --text ./RegPrivateKey.pem
```

你会被要求选择Navicat产品类别、Navicat语言版本和填写主版本号。之后一个随机生成的 序列号 将会给出。
![image](https://img2020.cnblogs.com/blog/2354934/202104/2354934-20210412220911599-2045499242.png)

```
/bin/navicat-keygen --text ./RegPrivateKey.pem
**********************************************************
*       Navicat Keygen (Linux) by @DoubleLabyrinth       *
*                   Version: 1.0                         *
**********************************************************

[*] Select Navicat product:
0. DataModeler
1. Premium
2. MySQL
3. PostgreSQL
4. Oracle
5. SQLServer
6. SQLite
7. MariaDB
8. MongoDB
9. ReportViewer

(Input index)> 1

[*] Select product language:
0. English
1. Simplified Chinese
2. Traditional Chinese
3. Japanese
4. Polish
5. Spanish
6. French
7. German
8. Korean
9. Russian
10. Portuguese

(Input index)> 1

/**** 版本号 ****/
[*] Input major version number:
(range: 0 ~ 15, default: 12)> 15

[*] Serial number:
NAVM-RTVJ-EO42-IODD

[*] Your name:
```

你可以使用这个 **序列号** 来暂时激活Navicat。

之后你会被要求填写 **用户名** 和 **组织名**。你可以随意填写，但别太长。

```
[*] Your name: DoubleLabyrinth
[*] Your organization: DoubleLabyrinth

[*] Input request code in Base64: (Double press ENTER to end)
```

之后你会被要求填写请求码。**注意不要关闭keygen。**

**断开网络**. 找到注册窗口，填写keygen给你的 **序列号**，然后点击 `激活`

通常在线激活会失败，所以在弹出的提示中选择 `手动激活`。


复制 **请求码** 到keygen，连按两次回车结束。

```
[*] Request Info:
{"K":"NAVHDM6JYBZW6BTG", "DI":"8AACDE2CC4372938A390", "P":"linux"}

[*] Response Info:
{"K":"NAVHDM6JYBZW6BTG","DI":"8AACDE2CC4372938A390","N":"orginly","O":"orginly","T":1618264222}

[*] Activation Code:
aokwdgERal7ycavHbohKxyiHS4m+oI3yCV+N6/q10QUJgA57YwtawE1HKbTO+6WqfOv8piR7o3cNNuK0MCH2hbTdSERIckKYq2x1iWemZi7r7PNINLoPcztNgq6WRWQK62EvDZhggl2BcCPNaR5FqGdC+Ff5H1Qp3qatK9yJTvmeW9U8GOuU/CJ0cN+BMbVvP4LZZh6ejTC/hLEaQQvkDd0pT8cVVjPXMsXNboUdljo4wWg5wWVBS8oYs6I0C8jVdaDIlzlkPMZUfMhtIQMTFPgfMOkm3Zp48EQ0rWdmE1lf8XCRMqCIOrmv4vi+jR90fot8Z+yutX4+MBTyiq6ZOQ==
```

最终你会得到一个base64编码的 激活码。


# 清理

```
pwd
/home/orginly/Downloads

sudo rm -rf navicat15-premium-cs
sudo rm -rf navicat15-premium-cs.AppImage
sudo rm -rf navicat
```
