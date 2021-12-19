# LEDを光らせ,ブザーを鳴らすデバイスドライバー

ロボットシステム学の第7，8回の授業において作成したデバイスドライバーを改良したものになります。

# OS環境

Raspberry Pi 3 Model B

OS:ubuntu 20.04 server

# 今回使用したもの

Raspberry PI 3 Model B

LED　×1

抵抗（220Ω）×1

電子ブザー ×1

ブレットボード ×1

ジャンパー線 ×4

# 配線図

![S__76259332](https://user-images.githubusercontent.com/95861309/146644332-5ac3030c-0af5-49c4-9a3a-f2b1eec3edff.jpg)


# how to use

#### install
```bash
$ git clone https://github.com/RyosukeIkeji/kadai1.git

$ cd kadai1

$ make

$ sudo insmod myled.ko

$ sudo chmod 666 /dev/myled0
```
#### uninstall
```bash
$ sudo rmmod myled

$ make clean
```
#### run
```bash
$ sudo rmmod myled

$ sudo insmod myled.ko

$ chmod 666 /dev/myled0

$ sudo chmod 666 /dev/myled0

$ echo 1 > /dev/myled0

（ブザーが鳴りだし、LEDも光る）

$ echo 0 > /dev/myled0

（停止）
```
# Clip

https://youtu.be/j82XY6i7Mb4

# Author

Ryuichi Ueda  

Ryosuke Ikeji


# License

GNU General Public License v3.0

https://github.com/RyosukeIkeji/kadai1/blob/b0cea3c5ca9e54edc36f4d4ca4c267676700e539/COPYING










