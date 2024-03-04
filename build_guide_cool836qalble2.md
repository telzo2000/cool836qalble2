## Build guide


## Firmware


###  QMK_FIRMWARE

[Here](https://github.com/telzo2000/cool836qalble/tree/main/firmware/cool836qalble)

<br>

[remap](https://remap-keys.app/catalog/FEmXx8GyuKYuJ5JSfcQG)

<br>

## Build 1

### 1 Diode soldering


Solder the diodes to the back of PCB.
<br>
PCBの裏面にダイオードのハンダ付けをします。
<br>

There are lead type and SMD diodes.
<br>
ダイオードはリードタイプか、SMDがあります。
<br>
Here, we will explain the lead type soldering.
<br>
ここでは、リードタイプのハンダ付けの説明をします。
<br>


Use a lead bender to bend the legs of the diode.
<br>
リードベンダーを使い、ダイオードの足を曲げます。
<br>

Insert the diode into the board.
<br>
ダイオードを基板に挿しこみます。
<br>

Please pay attention to the orientation of the diode.
<br>
ダイオードの向きに注意してください。
<br>


Secure the diode with masking tape, then face up.
<br>
マスキングテープでダイオードを固定してから、表面を上にします。
<br>
Solder the protruding legs.
<br>
はみ出ている足部分に、ハンダ付けをします。
<br>
After soldering, use nippers to cut off the protruding legs.
<br>
はんだ付けが終わったら、はみ出ている足をニッパーで切り取ってください。
<br>


[８倍速　Diodeハンダ付け動画](https://youtu.be/Yaodh2-XxV4)

<br>
<br>

### 2 Soldering switch sockets


Solder the switch sockets on the back side.
<br>
裏面にスイッチソケットのハンダ付けをします。
<br>

[８倍速　Switch socketハンダ付け動画](https://youtu.be/E__mHvmIXQo)

<br><br>

### 3 Mounting the Ble Micro Pro

Conthrough specifications are recommended.
<br>
コンスルーの仕様を推奨します。
<br>
<br>
A 12-pin or 13-pin connector is required. Even with 12 pins, there is no problem in use by inserting it closer to the USB-C terminal side as shown in the image.
<br>
コンスルーは12ピンまたは13ピンが必要です。12ピンでも画像のようにUSB-C端子側に寄せて差し込むことで、使用上、問題ありません。
<br>
![](img/img00015.jpg)
![](img/img00016.jpg)

Please take a look at the image below and pay attention to the orientation of the Ble Micro Pro.
<br>
下の画像を見て、Ble Micro Proの向きに気を付けて装着してください。
<br>
![](img/img00017.jpg)
![](img/img00018.jpg)


### 4 Soldering the battery board

Assemble the battery board according to the supplier's instructions.
<br>
購入先の説明に沿って、電池基板を組み立ててください。
<br>
<br>
Prepare two pin sockets with one pin.
<br>
ピンソケットを１ピン分にしたものを２つ用意してください。
<br>
<br>
Solder the pin sockets to the PCB as shown in the image below.
<br>
下の画像のように、ピンソケットをPCBにはんだ付けしてください。
<br>
![](img/img00019.jpg)

Place the battery board and solder it. Leave some space between it and the PCB, referring to the image below.
<br>
電池基板を載せて、はんだ付けをしてください。下の画像を参考にして、PCBとの間をやや空けておいてください。
<br>

![](img/img00021.jpg)

![](img/img00022.jpg)

![](img/img00023.jpg)

<br>
Keep the switch on the battery board ON. It's fragile, so be careful.
<br>
電池基板のスイッチをONにしておいてください。壊れやすいので、注意が必要です。
<br>
<br>

### 5 Soldering the power switch

Solder the horizontal slide switch as shown in the image below.
<br>
下の画像のように、水平スライドスイッチをはんだ付けしてください。
<br>
![](img/img00024.jpg)

![](img/img00025.jpg)

![](img/img00026.jpg)

<br>

### 6 Instorlling QMK＿Firmware on Ble Micro pro

Connect Ble Micro pro and PC with cable.
<br>
Ble Micro proとPCをケーブルで繋ぎます。
<br>
<br>
Access [here](https://sekigon-gonnoc.github.io/BLE-Micro-Pro-WebConfigurator/#/home).
<br>
[ここ](https://sekigon-gonnoc.github.io/BLE-Micro-Pro-WebConfigurator/#/home)にアクセスします。
<br>

![](img/img00003.png)
![](img/img00004.png)
![](img/img00005.png)
![](img/img00006.png)
Click NEXT at the bottom.
<br>
下段のNEXTをクリックします。
<br>
You will be asked for the bootloader version, but if you choose the latest version, you should be fine.
<br>
bootloaderのバージョンを聞かれますが、最新版で選んでおけば、大丈夫と思います。
<br>
<br>
Click Update.
<br>
Updateをクリックします。
<br>
<br>
It will ask for a serial port connection, so choose the one with the connected cable.
<br>
シリアルポートの接続を要求しますので、繋がっているケーブルのものを選んでください。
<br>
You will be asked the same question again, but don't worry, just repeat it again. One of these days, you can update. After that, click Next.
<br>
同じようなことをもう一度尋ねられますが、気にせず、もう一回繰り返してください。そのうち、Updateができます。そのあとは、Nextをクリックしてください。
<br>

![](img/img00007.png)

You will be asked for the application version, but if you choose the latest version, I think it's great. Then click Update. Then, when you get a connection request, do the same as before.
<br>
application versionを尋ねられますが、最新版を選べば、大乗と思います。そして、Updateをクリックしてください。その後、接続要求が出たら、先ほどと同じようにしてください。
<br>
![](img/img00008.png)
We recommend setting Debounce to 3. Chattering occurred in the author's environment. After 3 it's stable.
<br>
Debounceを３にしておくことを勧めます。作者の環境では、チャタリングが発生しました。３にしてからは安定しています。
<br>
![](img/img00009.png)

Click Update and you will be prompted to connect, just do the same as before.
<br>
Updateをクリックすると、接続要求が出ますので、前と同じようにしてください。
<br>
![](img/img00010.png)
congratulations. The first stage is finished.
<br>
おめでとうございます。第一段階が終了しました。
<br><br>
Click on QMK Confiurator for Ble Micro Pro.
<br>
次にQMK Confiurator for Ble Micro Proの方をクリックしてください。
<br>
![](img/img00011.png)
You will be asked to connect, so do the same as before.
<br>
接続要求がきますので、前と同じようにしてください。
<br>
![](img/img00012.png)

config.json is requested. Download the config.json [here](https://github.com/telzo2000/cool836qalble/tree/main/firmware/cool836qalble) and use it.
<br>
config.jsonが要求されます。[ここ](https://github.com/telzo2000/cool836qalble/tree/main/firmware/cool836qalble)にあるconfig.jsonをダウンロードして、使用してください。
<br>
<br>
Congratulations. The second stage is over.
<br>
おめでとうざいます。第二段階が終わりました。
<br>

![](img/img00010.png)

Select Remap from here.
<br>
ここからRemapを選択してください。
<br>
![](img/img00013.png)

![](img/img00014.png)
Edit your favorite keymap.
<br>
自分好みのキーマップを編集してください。
<br>
<br>
congratulations. The third stage is finished. Firmware is complete.
<br>
おめでとうございます。第三段階が終了しました。ファームウェアが完成です。


### Build 2(case)

### 1 Case


I will explain using a case printed by stereolithography of black resin ordered from JLCPCB. The procedure is basically the same for cases printed with Ankemake M5 for home use.
<br>
JLCPCBに発注したブラックレジンの光造形で印刷されたケースを使って説明します。家庭用AnkemakeM5で印刷したケースでも作業の手順は、基本的に同じです。
<br>
<br>
Fix the magnets to the five dents inside the case with an adhesive or the like. There are 5 in the top case and 5 in the bottom case for a total of 10.Please pay attention to the polarity of the magnet. Make sure the top case and bottom case are magnetically attached.
<br>
ケースの内側にある５つの凹みに磁石を接着剤などで固定します。トップケースに５箇所、ボトムケースに５箇所の合計10箇所です。
極性に注意してください。トップケースとボトムケースが磁力で着くようにしてください。
<br>
![](img/img00027.jpg)

As shown in the image below, attach rubber O-rings to the four protrusions on the bottom case. This makes it a gasket mount. You can do without the O-ring, but the PCB may move up and down inside the case.
<br>
下の画像のように、ボトムケースに4箇所の凸部にゴムのO-ringを装着します。これによりガスケットマウントとなります。O-ringはなくても大丈夫ですが、ケース内で、PCBが上下に動く可能性があります。
<br>
![](img/img00028.jpg)

The O-ring in the image is [this product](https://www.amazon.co.jp/gp/product/B07G4SM5SM/ref=ppx_yo_dt_b_asin_title_o03_s00?ie=UTF8&psc=1).
<br>
画像のO-ringは[この商品](https://www.amazon.co.jp/gp/product/B07G4SM5SM/ref=ppx_yo_dt_b_asin_title_o03_s00?ie=UTF8&psc=1)です。
<br>
Pay attention to the orientation of the Switch Parts and attach them to the bottom case.
<br>
Switch Partsの向きに注意して、ボトムケースに取り付けてください。
<br>
![](img/img00029.jpg)
<br>
Place the hole in the switch plate on the O-ring. And it is completed by covering the top case.
<br>
スイッチプレートの穴をO-ringに載せます。このとき、水平スライドスイッチのつまみがSwitch Pasrtsの窪みに入るようにしてください。そして、トップケースを被せて完成です。
<br>
![](img/img00030.jpg)
![](img/img00031.jpg)
![](img/img00032.jpg)

Welcome to the world of 36 keys.
<br>
36キーの世界へようこそ。
<br>