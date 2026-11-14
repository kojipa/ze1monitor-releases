# ZE1 Monitor

2代目日産リーフ（ZE1、2017〜2025年式）用の車両モニターアプリ（Android）です。
日産自動車とは関係のない、個人が作った非公式のアプリです。

[English](README.en.md)

## できること

- ホーム画面：SOC、出力（回生を含む）、パック電圧、車速、航続可能距離、電池温度、12Vバッテリー、外気温、走行距離
- 電池画面：SOH、電池の容量、セル96本の電圧、電池温度、急速・普通充電の回数、記録と推移
- 充電中の表示、トリップ、エコ運転チャレンジ、キリ番、しきい値の通知
- 走行と充電の記録（CSV）、デモモード、文字の大きさ、日本語と英語

## 必要なもの

- Android 8.0 以上のスマートフォン、タブレット、カーナビ（Android）
- ELM327 互換の OBD2 アダプター（Bluetooth、BLE、Wi-Fi）

## 入れ方

1. [Releases](https://github.com/kojipa/ze1monitor-releases/releases) から `ze1monitor-0.1.0.apk` をダウンロードします。
2. ダウンロードしたファイルを開いてインストールします（「提供元不明のアプリ」の許可を求められたら許可してください）。
3. アダプターを車の OBD2 端子に挿し、アプリでアダプターを選んで接続します。

## ご注意

- 車に送るのは読み取りの命令だけです。車の設定を変える命令は送りません。
- 自己責任でご利用ください。運転中は操作しないでください。
- 急速充電中と62kWh（e+）は確認中です。
- 調査版（ZE1 Monitor 調査版）とは別のアプリです。両方入れたまま使えます。

## 参考にした資料

車からの値の読み方は、次の公開資料を参考にしました（コードの複製はしていません）。

- [OVMS v3](https://github.com/openvehicles/Open-Vehicle-Monitoring-System-3)（vehicle_nissanleaf、MIT License）
- [zerinrc/ze1tcu](https://github.com/zerinrc/ze1tcu)（MIT License）
- [dalathegreat/leaf_can_bus_messages](https://github.com/dalathegreat/leaf_can_bus_messages)（Nissan Leaf 2018 ECU polling）
