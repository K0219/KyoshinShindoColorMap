# KyoshinShindoColorMap
強震モニタのリアルタイム震度での各地点の色を震度に変換するテーブルです。  
テーブルって書いてるくせにMapになってるのは仕様です。

## 解説
強震モニタのリアルタイム震度では、震度0.1刻みで-3から6.9まで~~合計100段階で色が変化します~~。(未だ確定しているわけではないので、間違っている可能性もあります。)

**2019年7月5日12時25分26秒のデータにて、計測震度7.0以上相当の色が確認されたため、試験的に7.0の色を追加しています。**  
7.0以上の場合にこの色になるようですので、ソフトで使用する際は `7.0+` といった表記をしてみてもいいかもしれません。

その段階を網羅してしまおうということでこの変換テーブルが作成されました。  
防災アプリケーションの今後の発展のために公開しています。

強震モニタの画像での色の取得座標に関しては、[KyoshinShindoPlaceEditor](https://github.com/ingen084/KyoshinShindoPlaceEditor)もご利用ください。

## CSVファイルの仕様
`震度,R値,G値,B値` となっています。

## ライセンス
作成: [ingen084](http://twitter.com/ingen084)  
協力: [こんぽ](https://twitter.com/compo031)さん

使用する際の報告は不要ですが(していただけると喜びます)、クレジットの表記はなるべくしていただけると助かります。(モチベがだいぶ上がるので)

## データ/値が間違っている or もっと細かいのあるよ
Issueを立てていただくか、プルリクを送っていただくと対処します。

## 注意事項
震度6.9の色に関しては概算値から割り出しています。  
このデータの震度は必ずしも正しいとは限りません。  
また、このデータの利用はすべて自己責任で行ってください。