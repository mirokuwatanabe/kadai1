# driver for LED 3minutes timer

## 概要

2021年度ロボットシステム学講義内にて __上田隆一先生__ のデバイスマネージャを改造し、Raspberry Pi 3 Model Bを使用し課題1用に3分タイマーを製作したものです。

## 動作環境
```
- Raspberry Pi 3 Model B
- Ubuntu 15.0.4
```
## インストール
```
1. make
2. sudo insmod myled.ko
3. sudo chmod 666 /dev/myled0
```
## アンインストール
```
1. sudo rmmod myled
2. make clean
```
## 実行方法

### demomode(30秒)
```
echo 0 > /dev/myled0
```

### mainmode(3分)
```
echo 1 > /dev/myled0
```

## 実行結果

youtubeにアップ済み

[LED timer](https://youtu.be/1AHgrck_Brk)

## ライセンス

[GNU General Public License](https://github.com/mirokuwatanabe/kadai1/blob/553b6a600fd91a45b983abfa87a5f41cab04e293/LICENSE)

