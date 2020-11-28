## ロボットシステム学　課題１

第７、８回で作成したデバイスドライバーをベースに、オリジナリティのある改造をしてGITHUBに置く

---

## デバイスドライバーの改良

デバイスドライバーの改良を行い入力した英文のモールス信号を打つことができるようにしました。声が出せない状況になっても、ラズベリーパイがあれば、モールス信号で助けを呼べます。

改良したプログラムのURL
https://github.com/kanekoNK/RS-GPIO/blob/master/myled/myled.c

---

## 使用道具
 * ラズベリーパイ４/1台
 * 電子ブザー/1個
 * LED/1個
 * ブレットボード/1枚
 * ジャンパー線/8本

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

 * 実家で使用した場合親が心配して部屋に入ってきたので注意が必要
