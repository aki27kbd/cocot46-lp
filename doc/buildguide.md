# Build Guide

![cocot46_lp_02](https://user-images.githubusercontent.com/88039287/149662909-3fa049e6-ae18-43c0-b3b9-cd5fc75c6064.jpg)

cocot46-lpのビルドガイドになります。
cocot46-lpは、cocot46をベースとしつつ携帯性に特化してより小型化・薄型化したキーボードです。
以下のような特徴を備えています。
・カラムスタッガードの一体型キーボード
・中央にミニトラックボールとロータリーエンコーダを搭載
・Choc v1スイッチ専用とすることで薄型化
・キーピッチを通常の19.05mmより小さい18mm×17mmとすることで小型化
・ロータリーエンコーダは水平タイプとロープロファイルタイプの選択が可能
・標準でミドルプレートが付属することで剛性と防塵性能アップ
・BLE Micro Proと単四電池2本を搭載することで無線化にも対応（別途専用の電池基板が必要）
・Remap対応による容易なキーマップ変更

## 部品
### キット付属品（PCBセット）

|名前|数|備考|
|---|---|---|
|PCB|1枚||
|ボトムプレート（FR4）|1枚||
|ミドルプレート（アクリル）|1枚||
|トラックボールカバープレート（FR4）|1枚||
|M2 スペーサー 4.5mm（メス―メス）|8本||
|M2 スペーサー 7mm（メス―メス）|4本||
|M2 ねじ 4mm|20本||
|M2 ねじ 8mm|4本||
|SMDダイオード|47個||
|タクトスイッチ|1個||
|トラックボール用L型ピンソケット|1個||
|トラックボール用L型ピンヘッダ|1個||
|水平ロータリーエンコーダ|1個||
|スライドスイッチ|2個||
|コンデンサ|1個||
|ショットキーバリアダイオード|2個||
|ゴム足|6個||

### キット付属品（アクリルトッププレート）

boothにて販売されているアクリルを購入するか、[こちら](https://github.com/aki27kbd/cocot46-lp/blob/master/doc/cocot46_lp_top_plate.zip?raw=true)のデータからご自身でアクリルを発注していただくことも可能です。  
発注の際には厚さ2mmのアクリルを選択するようお願いします。

|名前|数|備考|
|---|---|---|
|トッププレート（アクリル）|1枚||

### キット以外に必要なもの

全てのパーツは[遊舎工房](https://shop.yushakobo.jp/)で揃えることが可能です。

|名前|数|備考|
|---|---|---|
|MicroUSBケーブルもしくはUSB-Type Cケーブル|1本||
|ProMicroもしくはBLE Micro Pro|1個||
|コンスル―（12ピン・高さ2.5mm）|2本||
|キースイッチ|46個|Kailh Choc v1|
|キーキャップ（1U）|46個|Kailh Choc v1|
|ロータリーエンコーダ（ロープロファイル）＋ノブ|1個|水平ロータリーエンコーダを用いない場合|
|7mmオプティカルトラックボールモジュール１uタイプ|1個||
|トラックボールモジュール用レベル変換基板|1個||

7㎜オプティカルトラックボールモジュール1uタイプに関しては[Amazon](https://www.amazon.co.jp/BitTradeOne-ADTB7M-7mm%E3%82%AA%E3%83%97%E3%83%86%E3%82%A3%E3%82%AB%E3%83%AB%E3%83%88%E3%83%A9%E3%83%83%E3%82%AF%E3%83%9C%E3%83%BC%E3%83%AB%E3%83%A2%E3%82%B8%E3%83%A5%E3%83%BC%E3%83%AB%EF%BC%91u%E3%82%BF%E3%82%A4%E3%83%97/dp/B087BVNWYS)、[モノタロウ](https://www.monotaro.com/p/6295/7835/)でも購入可能です。

トラックボールモジュール用レベル変換基板に関しては[のぎけす屋様](https://nogikes.booth.pm/items/2008258)でも購入可能です。

各ショップの在庫状況に応じて検討ください。

### 無線化オプションパーツ

|名前|数|備考|
|---|---|---|
|電池基板|2枚||
|電池カバープレート|2枚||
|単四電池ホルダー|2個||
|電池用ピンソケット（3ピン）|2個||
|電池用L型ピンヘッダ（3ピン）|2個||
|M2 スペーサー 6mm（メス―メス）|4本||
|M2 ねじ 4mm|8本||

BLE Micro Proを用いて無線接続するためには[こちら](https://github.com/aki27kbd/cocot46-lp/blob/main/doc/bmp_setup.md)の手順を参照してください。

## 組み立て
### 0. 部品確認

  まずはパーツが揃っているか確認ください。

  ![cocot46_lp_bg_00](https://user-images.githubusercontent.com/88039287/150814688-0e7eba8d-c149-4315-a729-e102b3b68193.jpg)

  その他上述の「キット以外に必要なもの」および「オプション部品」を揃えた上で組み立てに取り掛かってください。

### 1. ダイオード

  PCB裏面に、写真の向きでダイオードをはんだ付けします。ダイオードの表面の線と、PCBのシルクの線の向きが揃うように配置してください。
  **ダイオードの向きは基板の左右で異なります。必ずシルクをよく確認した上ではんだ付けを行ってください。**
  予め片側にはんだを盛っておき、溶かしながらピンセットでダイオードを押さえつけると固定しやすくなります。  
  **全47箇所**はんだ付けを行ってください。

  ![cocot46_lp_bg_01](https://user-images.githubusercontent.com/88039287/150814850-325ac945-e81b-4534-97aa-56cb185fc64b.JPG)

### 2. トラックボール用ピンソケット

  PCB裏面に、トラックボール用L型ピンソケットを差し込み、マスキングテープなどで固定した後表面からはんだ付けします。

  ![cocot46_lp_bg_02](https://user-images.githubusercontent.com/88039287/150815025-e3b71e0f-2dff-4ea2-bf0d-873b16cc7acd.jpg)

### 3. タクトスイッチ

  PCB表面に、タクトスイッチ（リセットスイッチ）をはんだ付けします。1箇所のみです。

  ![cocot46_lp_bg_03](https://user-images.githubusercontent.com/88039287/150815428-c562403e-48b8-4569-94d3-d77dcb016370.jpg)

### 4. ProMicro

  ProMicroの準備をします。写真の向きでコンスル―をはんだ付けします。
  コンスル―には向きがあるので注意してください。コンスル―の向きについては[こちら](https://yushakobo.zendesk.com/hc/ja/articles/360044233974-%E3%82%B3%E3%83%B3%E3%82%B9%E3%83%AB%E3%83%BC-%E3%82%B9%E3%83%97%E3%83%AA%E3%83%B3%E3%82%B0%E3%83%94%E3%83%B3%E3%83%98%E3%83%83%E3%83%80-%E3%81%AE%E5%8F%96%E3%82%8A%E4%BB%98%E3%81%91%E6%96%B9%E3%82%92%E6%95%99%E3%81%88%E3%81%A6%E4%B8%8B%E3%81%95%E3%81%84)を参照ださい。マイクロUSBソケットはもげやすいので、適宜補強をしてからはんだ付けを行ってください。

  ![bg_04_promicro](https://user-images.githubusercontent.com/88039287/127672558-b29795b9-0192-4cca-91e0-c8eb80710140.jpg)

### 5. ロータリーエンコーダ

  中央部分に水平ロータリーエンコーダをはんだ付けします。ロータリーエンコーダの脚を通し、裏側からはんだ付けをしてください。

  ※必ず6本の足が全て裏面に出ていることを確認してからはんだ付けを行ってください。

  ![cocot46_lp_bg_05_1](https://user-images.githubusercontent.com/88039287/150815755-7f5e540b-ae37-4a48-977f-94998ce229ac.jpg)

  ![cocot46_lp_bg_05_2](https://user-images.githubusercontent.com/88039287/150815830-112ec73a-da94-49f2-a506-28143c883865.jpg)


### 6. キースイッチ

  トッププレートの保護紙をはがし、PCBの上に重ねます。キースイッチの足を折らないように確認しながら差し込み、トッププレートを固定します。

  ![cocot46_lp_bg_06_1](https://user-images.githubusercontent.com/88039287/150825546-226b246a-a076-4093-8aff-21106f3e3e2f.jpg)

  ![cocot46_lp_bg_06_2](https://user-images.githubusercontent.com/88039287/150825919-d1599336-7182-472d-b319-dff4bf262778.jpg)

  全てのキースイッチを差し込んだら、PCB裏面からはんだ付けを行います。2本×46キー分、スイッチの足が出ていることを確認しながらはんだ付けを行ってください。

  ![cocot46_lp_bg_06_3](https://user-images.githubusercontent.com/88039287/150825965-35e1c0ef-025b-4d2d-b0c8-0d708077f0ff.jpg)

### 7. スライドスイッチ

  スライドスイッチ2箇所を表面からマスキングテープなどで固定し、裏面からはんだ付けを行います。

  ![cocot46_lp_bg_07](https://user-images.githubusercontent.com/88039287/150827936-089ae2f4-6b21-448b-bc4f-293376e5d506.jpg)

### 8. トラックボール

  トラックボールユニットの準備を行います。  
  トラックボール用L型ピンヘッダ、トラックボールモジュール、レベル変換基板を写真のようにはんだ付けします。  
  特にトラックボールモジュールとレベル変換基板をつなぐケーブル部分は間隔が狭いので、隣り合うパッドとショートしないよう気を付けてください。

  ![cocot46_lp_bg_08_1](https://user-images.githubusercontent.com/88039287/150828212-6652a026-4537-42af-8737-63267b598785.jpg)

  ![cocot46_lp_bg_08_2](https://user-images.githubusercontent.com/88039287/150828290-7258974b-93e3-4ee7-b965-424afe280523.jpg)

### 9. その他パーツ

  その他パーツをPCB裏面にはんだ付けします。  
  ショットキーバリアダイオード×2、コンデンサを写真の位置にはんだ付けしてください。  
  ショットキーバリアダイオードは向きがあるので、PCBのシルクを良く確認してからはんだ付けを行ってください。  
  コンデンサはどちらの向きにつけても問題ありません。

  ![cocot46_lp_bg_09_1](https://user-images.githubusercontent.com/88039287/150940996-8d033138-99c8-46dd-b015-dc02d45a265b.jpg)

  同じくPCB裏面の1箇所をジャンパーさせます。
  ![cocot46_lp_bg_09_2](https://user-images.githubusercontent.com/88039287/150941276-67185f1d-d8dd-47bb-a375-e8291e64f91b.jpg)


### 10. 組み立て

  4.5mmスペーサーと4mmネジでトッププレート表面から8箇所ねじ止めを行います。

  ![cocot46_lp_bg_10_1](https://user-images.githubusercontent.com/88039287/150941990-f7f6c764-6c1a-4761-b42a-d4e13f381c5b.jpg)

  8で組み立てたトラックボールユニットをPCBのL型ピンソケットに差し込みます。ケーブルがPCBの溝部分におさまるように折りたたみます。

  ![cocot46_lp_bg_10_2](https://user-images.githubusercontent.com/88039287/150942217-2cb88b5a-e8d3-4587-9f7a-430a67433ebf.jpg)

  ProMicroもしくはBLE Micro ProをPCBに差し込みます。コンスル―を用いている場合ははんだ付け不要です。

  ![cocot46_lp_bg_10_3](https://user-images.githubusercontent.com/88039287/150942398-e0f602d1-51c0-4585-954a-79349a622c04.jpg)

  ミドルプレートの保護紙をはがし、PCB裏面に重ねます。  
  リセットスイッチの足やコンデンサの位置が干渉しないように向きに注意してください。

  ![cocot46_lp_bg_10_4](https://user-images.githubusercontent.com/88039287/150942763-995c6a78-cce3-4301-9974-b792d05e7a83.jpg)

  ミドルプレートにボトムプレートを重ね、4mmネジで8箇所ねじ止めをします。

  ![cocot46_lp_bg_10_5](https://user-images.githubusercontent.com/88039287/150942956-4837d751-f395-4bdd-bbda-583e2b99c17b.jpg)

  トラックボールカバープレートの固定のため、PCB上に7mmスペーサーを立て、ボトムプレート側から8mmネジで固定します。

  ![cocot46_lp_bg_10_6](https://user-images.githubusercontent.com/88039287/150943154-ad37ad85-0dc8-4efe-ba9f-9b5006692d90.jpg)

  トラックボールカバープレートを4㎜ネジで固定します。

  ![cocot46_lp_bg_10_7](https://user-images.githubusercontent.com/88039287/150943464-e09c6d30-1074-456a-b5e0-aee56a30bd53.jpg)

  ボトムプレートにゴム足を6箇所貼り付けます。

  ![cocot46_lp_bg_10_8](https://user-images.githubusercontent.com/88039287/150943562-b9298f73-7e93-4f6a-aecd-9b969f3ade3b.jpg)

  お好みのキーキャップを付けて完成です！

  ![cocot46_lp_bg_10_9](https://user-images.githubusercontent.com/88039287/150943634-fee76eb2-479d-44df-a9be-66271fd34549.jpg)


## ファームウェア

***ファームウェアはcocot46と共通です。***
トラックボールを操作する手によって、2種類ファームウェアを用意しております。

[右手用](https://github.com/aki27kbd/cocot46/blob/main/firmware/cocot46_trackball_right.zip?raw=true)  
[左手用](https://github.com/aki27kbd/cocot46/blob/main/firmware/cocot46_trackball_left.zip?raw=true)  
[右手用v2](https://github.com/aki27kbd/cocot46/blob/main/firmware/cocot46_trackball_v2.zip?raw=true)

[REMAP](https://remap-keys.app/catalog/rZnKrpVyZLRcMqKgEM7Z/firmware)からファームウェアのダウンロードおよびProMicroへの書き込みを行うことができます。キーマップは[こちら](https://remap-keys.app/configure)から更新可能です。  
トラックボール、LED含めて上記.hexファイルで確認いただけます。

（.hexファイルをQMK ToolboxなどでProMicroに書き込む従来の方法でも問題ありません。）


![remap](https://user-images.githubusercontent.com/88039287/130786498-4202abef-06bf-4c86-a5e6-c8a95990caf2.jpg)

組み立て段階で動作確認をする際も、REMAPのTest Matrix Modeを使うと便利です。

ソースコードは[こちら](https://github.com/aki27kbd/qmk_firmware/tree/master/keyboards/cocot46)を参照ください。

また、VIA用のjsonファイルは[こちら](https://github.com/aki27kbd/cocot46/blob/main/firmware/cocot46_via.json)を参照ください。

## 無線化

BLE Micro Proを用いて無線接続するためには[こちら](https://github.com/aki27kbd/cocot46/blob/main/doc/bmp_setup.md)の手順を参照してください。

## 終わりに
何かトラブルがあれば[Twitterアカウント](https://twitter.com/aki27kbd)までご連絡ください。

また、完成写真をSNSにアップいただけるととても励みになります。（アップするのがはばかられる方はDMで直接送りつけていただいても構いません。）

ハッシュタグは #cocot46 です。
