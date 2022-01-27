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
参考までに、[Anymany](https://anymany.net/speed-order/)で上記データを発注すると約4,000円となります。

|名前|数|備考|
|---|---|---|
|トッププレート（アクリル）|1枚|2mm|

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

## 組み立て
### 0. 部品確認

  まずはパーツが揃っているか確認ください。

  ![cocot46_lp_bg_00_rev](https://user-images.githubusercontent.com/88039287/151126937-358621aa-b336-4be2-b7d4-50d404a94e23.jpg)

  その他上述の「キット以外に必要なもの」および「オプション部品」を揃えた上で組み立てに取り掛かってください。

### 1. ダイオード

  PCB裏面に、写真の向きでダイオードをはんだ付けします。ダイオードの表面の線と、PCBのシルクの線の向きが揃うように配置してください。
  **ダイオードの向きは基板の左右で異なります。必ずシルクをよく確認した上ではんだ付けを行ってください。**
  予め片側にはんだを盛っておき、溶かしながらピンセットでダイオードを押さえつけると固定しやすくなります。  
  **全47箇所**はんだ付けを行ってください。

  ![cocot46_lp_bg_01_rev](https://user-images.githubusercontent.com/88039287/151127201-75220375-0112-4793-bb07-84063347af75.JPG)

### 2. トラックボール用ピンソケット

  PCB裏面に、トラックボール用L型ピンソケットを差し込み、マスキングテープなどで固定した後表面からはんだ付けします。

  ![cocot46_lp_bg_02](https://user-images.githubusercontent.com/88039287/150815025-e3b71e0f-2dff-4ea2-bf0d-873b16cc7acd.jpg)

### 3. タクトスイッチ

  PCB表面に、タクトスイッチ（リセットスイッチ）をはんだ付けします。

  ![cocot46_lp_bg_03](https://user-images.githubusercontent.com/88039287/150815428-c562403e-48b8-4569-94d3-d77dcb016370.jpg)

### 4. ProMicro / BLE Micro Pro

  ProMicroの準備をします。写真の向きでコンスル―をはんだ付けします。
  コンスル―には向きがあるので注意してください。コンスル―の向きについては[こちら](https://yushakobo.zendesk.com/hc/ja/articles/360044233974-%E3%82%B3%E3%83%B3%E3%82%B9%E3%83%AB%E3%83%BC-%E3%82%B9%E3%83%97%E3%83%AA%E3%83%B3%E3%82%B0%E3%83%94%E3%83%B3%E3%83%98%E3%83%83%E3%83%80-%E3%81%AE%E5%8F%96%E3%82%8A%E4%BB%98%E3%81%91%E6%96%B9%E3%82%92%E6%95%99%E3%81%88%E3%81%A6%E4%B8%8B%E3%81%95%E3%81%84)を参照ださい。マイクロUSBソケットはもげやすいので、適宜補強をしてからはんだ付けを行ってください。

  ![bg_04_promicro](https://user-images.githubusercontent.com/88039287/127672558-b29795b9-0192-4cca-91e0-c8eb80710140.jpg)

  BLE Micro Proを用いる場合、コンスル―のはんだ付けは不要です。

### 5. ロータリーエンコーダ

  中央部分に水平ロータリーエンコーダをはんだ付けします。ロータリーエンコーダの脚を通し、裏側からはんだ付けをしてください。

  ※必ず6本の足が全て裏面に出ていることを確認してからはんだ付けを行ってください。

  ![cocot46_lp_bg_05_1](https://user-images.githubusercontent.com/88039287/150815755-7f5e540b-ae37-4a48-977f-94998ce229ac.jpg)

  ![cocot46_lp_bg_05_2](https://user-images.githubusercontent.com/88039287/150815830-112ec73a-da94-49f2-a506-28143c883865.jpg)

  ロープロファイルロータリーエンコーダを用いる場合は裏面から見るとしたの写真のようになります。（プッシュスイッチ付きのロータリーエンコーダを用いることも可能ですが、高さが出るため推奨されません。）

  ![cocot46_lp_bg_05_3](https://user-images.githubusercontent.com/88039287/151128220-2a6ba572-0184-4a7a-8435-c23c07a71242.JPG)

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

  ![cocot46_lp_bg_09_1_rev](https://user-images.githubusercontent.com/88039287/151132868-40ce0d01-8016-4bde-86aa-1cbefa7bc85b.jpg)

  同じくPCB裏面の1箇所をジャンパーさせます。
  ![cocot46_lp_bg_09_2_rev](https://user-images.githubusercontent.com/88039287/151132919-1b2efc9c-3545-439e-a313-f1ccf41323cf.jpg)


### 10. 組み立て

  4.5mmスペーサーと4mmネジでトッププレート表面から8箇所ねじ止めを行います。

  ![cocot46_lp_bg_10_1_rev](https://user-images.githubusercontent.com/88039287/151133528-630fddd4-10a9-4c06-bb7a-73707107037c.jpg)

  8で組み立てたトラックボールユニットをPCBのL型ピンソケットに差し込みます。ケーブルがPCBの溝部分におさまるように折りたたみます。

  ![cocot46_lp_bg_10_2](https://user-images.githubusercontent.com/88039287/150942217-2cb88b5a-e8d3-4587-9f7a-430a67433ebf.jpg)

  ProMicroもしくはBLE Micro ProをPCBに差し込みます。コンスル―を用いている場合ははんだ付け不要です。

  ![cocot46_lp_bg_10_3](https://user-images.githubusercontent.com/88039287/150942398-e0f602d1-51c0-4585-954a-79349a622c04.jpg)

  BLE Micro Proの場合、12ピンコンスル―を写真のように通してください。

  ![cocot46_lp_bg_10_6_bmp_rev](https://user-images.githubusercontent.com/88039287/151134459-6b6ae404-f12c-42fe-b8fb-9113084fa8be.jpg)

  ミドルプレートの保護紙をはがし、PCB裏面に重ねます。  
  リセットスイッチの足やコンデンサの位置が干渉しないように向きに注意してください。

  ![cocot46_lp_bg_10_4](https://user-images.githubusercontent.com/88039287/150942763-995c6a78-cce3-4301-9974-b792d05e7a83.jpg)

  ミドルプレートにボトムプレートを重ね、4mmネジで8箇所ねじ止めをします。

  ![cocot46_lp_bg_10_5_rev](https://user-images.githubusercontent.com/88039287/151165901-e6e5c017-835f-4644-a855-4b4f68e0ce85.jpg)

  トラックボールカバープレートの固定のため、PCB上に7mmスペーサーを立て、ボトムプレート側から8mmネジで固定します。

  ![cocot46_lp_bg_10_6](https://user-images.githubusercontent.com/88039287/150943154-ad37ad85-0dc8-4efe-ba9f-9b5006692d90.jpg)

  トラックボールカバープレートを4㎜ネジで固定します。

  ![cocot46_lp_bg_10_7](https://user-images.githubusercontent.com/88039287/150943464-e09c6d30-1074-456a-b5e0-aee56a30bd53.jpg)

  ボトムプレートにゴム足を6箇所貼り付けます。

  ![cocot46_lp_bg_10_8](https://user-images.githubusercontent.com/88039287/150943562-b9298f73-7e93-4f6a-aecd-9b969f3ade3b.jpg)

  お好みのキーキャップを付けて完成です！

  ![cocot46_lp_bg_10_9](https://user-images.githubusercontent.com/88039287/150943634-fee76eb2-479d-44df-a9be-66271fd34549.jpg)

### 11. 無線化（オプション）

  下記パーツが揃っていることを確認してください。

  ![cocot46_lp_bg_11_1_rev](https://user-images.githubusercontent.com/88039287/151170785-1f6c086d-bfd1-4f4a-9236-6e33dbf20496.jpg)

  単四電池ホルダーを電池基板に通し、裏側からはんだ付けを行います。裏側のピンは本体と干渉するので、根本でカットしてください。はんだも盛り過ぎず、出っ張りを最小限とするよう意識すると良いです。

  ![cocot46_lp_bg_11_2](https://user-images.githubusercontent.com/88039287/151171050-678c2596-725c-4a84-8a0b-77e0daeb6256.JPG)

  電池用ピンヘッダを電池基板にはんだ付けします。

  ![cocot46_lp_bg_11_3](https://user-images.githubusercontent.com/88039287/151171705-6e8ef9cd-880b-451e-a0ad-0adbc028aec7.JPG)

  電池用ピンソケットを基板の左右に固定します。表側からピンソケットを差し、裏面からはんだ付けを行います。はんだ付けを行う際はボトムプレート・ミドルプレートを外した状態で行ってください。

  ![cocot46_lp_bg_11_4](https://user-images.githubusercontent.com/88039287/151173851-0c0f9f9b-5d59-4924-b8cc-56dc3dea0f08.JPG)

  6mmスペーサーをPCB裏側からねじ止めします。電池基板に取り付けたピンヘッダをピンソケットに差し込みます。

  ![cocot46_lp_bg_11_5](https://user-images.githubusercontent.com/88039287/151176307-f00ad4e8-c2a5-4ec8-a0fa-af2dfc58e60d.JPG)

  電池カバープレートをねじ止めし、単四電池を入れれば完成です。

  ![cocot46_lp_bg_11_6](https://user-images.githubusercontent.com/88039287/151176656-036ee8f1-8592-4f93-9be0-642318d22ab4.jpg)

  BLE Micro Pro横のスライドスイッチ×2電源廻りの制御が可能です。  
  無線接続を行う場合は両方のスライドスイッチを内側にして使用してください。

  ![cocot46_lp_bg_11_7_rev](https://user-images.githubusercontent.com/88039287/151319234-54ed1400-8f3e-4ea8-9201-aef4f9e67fbe.jpg)

## ファームウェア

***ファームウェアはcocot46と共通です。***

### ProMicro

ProMicroを用いる場合は[こちら](https://github.com/aki27kbd/cocot46/blob/main/doc/buildguide.md#%E3%83%95%E3%82%A1%E3%83%BC%E3%83%A0%E3%82%A6%E3%82%A7%E3%82%A2)を参照してください。

### BLE Micro Pro

BLE Micro Proを用いて無線化する場合は[こちら](https://github.com/aki27kbd/cocot46/blob/main/doc/bmp_setup.md#%E3%83%95%E3%82%A1%E3%83%BC%E3%83%A0%E3%82%A6%E3%82%A7%E3%82%A2)を参照してください。

## 終わりに
何かトラブルがあれば[Twitterアカウント](https://twitter.com/aki27kbd)までご連絡ください。

また、完成写真をSNSにアップいただけるととても励みになります。（アップするのがはばかられる方はDMで直接送りつけていただいても構いません。）

ハッシュタグは #cocot46 です。
