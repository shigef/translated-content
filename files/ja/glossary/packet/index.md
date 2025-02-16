---
title: パケット
slug: Glossary/Packet
---
パケット、またはネットワークパケットはは、ネットワーク上で送られる整形されたデータの塊です。パケットはユーザーデータと制御情報を含みます。ユーザーデータは*ペイロード*として知られています。制御情報はペイロードを送るための制御情報です。この制御情報は、送信元と送信先のネットワークアドレス、順序情報、エラー検知コードで構成されており、通常パケットのヘッダーとフッターで見られます。

## パケットに含まれるもの

### ホップ制限

ホップとは、パケットがあるネットワークから次のネットワークに渡されるときに発生するものです。これは、パケットが通過するたびに 1 ずつ減少するフィールドで、 0 になると失敗してパケットは破棄されます。

時間が経つにつれ、パケット数は閉回路内を循環する原因となり、循環するパケット数は蓄積され、最終的にはネットワークの失敗につながることになります。

### 誤り検出訂正

誤り検出訂正とは、データを受信者に送信する際に発生する誤りを検出して訂正するためのコードです。誤り訂正には、後方誤り訂正と前方誤り訂正の２種類があります。後方誤り訂正とは、受信機が送信機に対してデータ単位全体の再送信を要求する場合です。前方誤り訂正は、受信機が自動的に誤りを訂正する誤り訂正符号を使用する場合です。

送信側では、パケットが送信される前に計算が行われます。宛先で受信すると、チェックサムが再計算され、パケット内のチェックサムと比較されます。

### 優先度

このフィールドは、どのパケットが他のパケットよりも高い優先度を持つべきかを示します。優先度の高いキューは、ネットワークが混雑しているときに、優先度の低いキューよりも早く空になります。

### アドレス

ネットワークパケットをルーティングする際には、送信元ホストの送信元アドレスと受信先ホストの送信先アドレスの 2 つのネットワークアドレスが必要になります。

### ユーザーデータ - ペイロード

ペイロードとは、アプリケーションに代わって運ばれるデータのことである。ペイロードの長さは通常可変で、ネットワークプロトコルや場合によっては経路上の機器によって設定される最大値までの長さがあります。

## 使用したリファレンス

- <https://en.wikipedia.org/wiki/Network_packet>
- [https://en.m.wikipedia.org/wiki/Hop\_(networking)](<https://en.wikipedia.org/wiki/Hop_(networking)>)
- <https://www.techradar.com/news/computing/how-error-detection-and-correction-works-1080736>
