## ロボットシステム学　課題１

第７、８回で作成したデバイスドライバーをベースに、オリジナリティのある改造をしてgithibに置く

---

## デバイスドライバーの改良

デバイスドライバーの改良を行い入力した英文のモールス信号を打つことができるようにしました。
改良したプログラムのULR
https://github.com/kanekoNK/RS-GPIO/blob/master/myled/myled.c

---

## 実際に動かす手順

 * git cloan https://github.com/kanekoNK/RS-GPIO.git
 * cd RS-GIIP
 * cd myled
 * sudo rmmod myled  (開いていた場合閉じる)
 * sudo insmod myled.ko
 * sudo chmod 666 /dev/myled0
 * echo モールス信号にしたい英文を入力 > /dev/myled0
 
---
## 実際に動かした動画
https://youtu.be/hMVFuafjlzk
