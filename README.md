# LED_Device_driver

ロボットシステム学の第7，8回の授業において作成したデバイスドライバーを改良したものになります。

# 動作環境

Raspberry Pi 3 Model B

OS:ubuntu 20.04 server

# 使用したもの

Raspberry PI 3 Model B

LED　×1

抵抗（220Ω）×2

電子ブザー ×1

ブレットボード ×1

ジャンパー線 ×4

# 配線図
![image](https://user-images.githubusercontent.com/95861309/146193888-ae945a6c-af1d-40bd-85cd-33030c5dcf5a.png)

# 使い方

次のようなコマンドを実行する。

$ sudo rmmod

$ sudo insmod myled.ko

$ chmod 666 /dev/myled0

$ sudo chmod 666 /dev/myled0

$ echo 1 > /dev/myled0

（ブザーがサイレンにのように音を出すのに合わせて、LED1が5回点滅する）

$ echo 0 > /dev/myled0

（停止）




