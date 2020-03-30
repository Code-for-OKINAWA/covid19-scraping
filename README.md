# COVID19 Hyogo Scraping Script

## What's this?
沖縄県公式サイトで公開されている情報を集め、jsonとして出力するPythonスクリプトです。
[沖縄県 新型コロナウイルスまとめサイト](https://friendly-lamport-e7cdf4.netlify.com/)で使用する形に整形し、出力します。

## Make date
```shell script
pip install -r requirements.txt
python3 main.py
```

## Reference data list
このスクリプトでは、以下のデータを参照し、jsonを出力しています。

|ファイル名|データの詳細|データの参照元|
|---|---|---|
|main_summary.json|検査状況/患者状況の総まとめ|[オープンデータカタログサイト](http://open-data.pref.hyogo.lg.jp/index.php?key=muq1trrqj-175#_175)|
|patients.json|患者についての情報|[兵庫県公式サイト](https://web.pref.hyogo.lg.jp/kk03/corona_kanjyajyokyo.html)|
|patients_summary.json|日別患者数|[オープンデータカタログサイト](http://open-data.pref.hyogo.lg.jp/index.php?key=muve6rx2r-175#_175)|
|inspections.json|PCR検査数(ページでは未使用のデータ)|[オープンデータカタログサイト](http://open-data.pref.hyogo.lg.jp/index.php?key=muve6rx2r-175#_175)|
|inspections_summary.json|PCR検査の総合計等|[オープンデータカタログサイト](http://open-data.pref.hyogo.lg.jp/index.php?key=muve6rx2r-175#_175)|
|last_update.json|データの最終更新日|スクリプト実行日時|

以上が東京都版で使われていて、沖縄県版でも使っているデータです。そして、以下が沖縄県版で独自に生成、使用しているデータです。


## License
このスクリプトは[MITライセンス](LICENSE)で公開されています。
