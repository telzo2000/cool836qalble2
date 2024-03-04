## Build guide


## Firmware


###  QMK_FIRMWARE

[Here](https://github.com/telzo2000/cool836qalble/tree/main/firmware/cool836qalble2)


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

![](img/img00004.jpg)

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

### 3 Soldering the capacitor



Solder the [capacitor](https://akizukidenshi.com/catalog/g/gP-02151/).
<br>
[コンデンサー](https://akizukidenshi.com/catalog/g/gP-02151/)をハンダ付けします。
<br>

First, apply solder to the terminal on one side. Then, place the capacitor, melt the solder, and fix it.
<br>
最初に、片側の端子にハンダを盛ります。そして、コンデサーを置き、ハンダを溶かして、固定します。
<br>

Next, melt and pour solder into the other terminal and attach the capacitor. Please fix it.
<br>
次に、もう片側の端子にハンダを溶かして、流し込んで、コンデンサーを。固定してください。
<br>
<br>


### 4 Soldering the slide switch

![](img/img00003.jpg)

Insert the [slide switch](https://shop.yushakobo.jp/products/5624?variant=45044666007783) from the back side of the PCB and solder the front side. Please remove the protruding legs.
<br>
[スライドスイッチ](https://shop.yushakobo.jp/products/5624?variant=45044666007783)はPCBの裏面から挿入して、表面をハンダ付けします。はみ出た足は、切り取ってください。
<br>


### 5 Mounting the Ble Micro Pro

Conthrough specifications are recommended.
<br>
コンスルーの仕様を推奨します。
<br>
<br>
A 13-pin connector is required.
<br>
コンスルーは13ピンが必要です。
<br>


Please take a look at the image below and pay attention to the orientation of the [Ble Micro Pro](https://shop.yushakobo.jp/products/ble-micro-pro/).
<br>

下の画像を見て、[Ble Micro Pro](https://shop.yushakobo.jp/products/ble-micro-pro/)の向きに気を付けて装着してください。
<br>

![](img/img00001.jpg)



### 6 Soldering the battery board

<br>

Solder [the battery holder](https://www.monotaro.com/p/8835/2765/) to the PCB as shown in the image below.
<br>

下の画像のように、[電池ホルダー](https://www.monotaro.com/p/8835/2765/)をPCBにはんだ付けしてください。
<br>

![](img/img00002.jpg)
z
<br>
<br>





### 7 (Option) Solering the reset switch


Actually, it's not necessary. If you are an cool836qalble2 and are trying to install a PRO micro without buying a Ble Micro Pro, you will need a reset switch.
<br>

実は必要ありません。もし、あなたがcool836qalble2なのに、Ble Micro Proをおごることをせずに、ただのpro micro取り付けようとするならば、リセットスイッチは必要でしょうね。

### 8 Soldering the joystick

Solder the [joystick](https://akizukidenshi.com/catalog/g/g115233/) as shown in the image below.
<br>

下の画像のように、[ジョイスティック](https://akizukidenshi.com/catalog/g/g115233/)をはんだ付けしてください。
<br>

![](img/img00007.jpg)

<br>




### 9 Instorlling QMK＿Firmware on Ble Micro pro

The following is from cool836qalble. It is basically the same for cool836qalble2, so please refer to it.
<br>
以下は、cool836qalbleのものです。cool836qalble２でも、基本的に同じですので、参考にしてください。
<br>
<br>

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

config.json is requested. Download the config.json [here](https://github.com/telzo2000/cool836qalble2/tree/main/firmware/cool836qalble2) and use it.
<br>
config.jsonが要求されます。[ここ](https://github.com/telzo2000/cool836qalble2/tree/main/firmware/cool836qalble2)にあるconfig.jsonをダウンロードして、使用してください。
<br>
<br>
Congratulations. The second stage is over.
<br>
おめでとうざいます。第二段階が終わりました。
<br>

![](img/img00010.png)

Select [Remap](https://qmk018.remap-keys.app/configure) from here.
<br>

ここから[Remap](https://qmk018.remap-keys.app/configure)を選択してください。
<br>
![](img/img00013.png)


![](img/img00014.png)

json file is requested, so select via.json located [here](https://github.com/telzo2000/cool836qalble2/tree/main/firmware/cool836qalble2).
<br>

jsonファイルが要求されますので、[ここ](https://github.com/telzo2000/cool836qalble2/tree/main/firmware/cool836qalble2)にある、via.jsonを選択してください。

<br>
Edit your favorite keymap.
<br>
自分好みのキーマップを編集してください。
<br>

![](img/img00020.png)

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
Place the hole in the switch plate on the O-ring. 
<br>
スイッチプレートの穴をO-ringに載せます。このとき、水平スライドスイッチのつまみがSwitch Pasrtsの窪みに入るようにしてください。
<br>
<br>
Place the knob on the joystick.
<br>
ジョイスティックにノブを載せてください。

![](img/img00015.jpg)

![](img/img00016.jpg)

<br>
Please cover with the top case.
<br>
トップケースを被せてください。

![](img/img00017.jpg)




Welcome to the world of 36 keys.
<br>
36キーの世界へようこそ。
<br>
![](img/img00018.jpg)