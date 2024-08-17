# プロジェクト構成

このプロジェクトはビルド設定からプロジェクトの構成全体を確認できることを目的としています。

## 環境

このプロジェクトは新しい環境でも使えるようにテンプレートとして利用できます。

## 主な使用アセット（UMP経由で管理）は以下
    /Users/tanabeyoshihiro/UnityProjects/InfinityBrade/Packages/manifest.jsonの中身を見てください。
    以下はその抜粋です。

    "com.google.ads.mobile": "9.2.0",

    // androidのストアレビューとその依存が以下の四つだが、ump経由だと必要なバージョンが選択できず仕方なくバージョンが無いやつはtgzで入れた。
    "com.google.play.review": "1.8.2",
    "com.google.android.appbundle": "file:../Assets/GooglePlayPlugins/com.google.android.appbundle-1.9.0.tgz",
    "com.google.play.common": "file:../Assets/GooglePlayPlugins/com.google.play.common-1.9.1.tgz",
    "com.google.play.core": "file:../Assets/GooglePlayPlugins/com.google.play.core-1.8.4.tgz",

    "com.neuecc.unirx": "https://github.com/neuecc/UniRx.git?path=Assets/Plugins/UniRx/Scripts",
    "com.unity.ads.ios-support": "1.0.0",
    "com.unity.cinemachine": "2.10.1",
    "com.unity.localization": "1.5.2",


## 主な使用アセットは以下（Asset Storeから落としてる。ので、asset/直下に入ってるからスマートではない）
feel

## ローカライズ
ローカライズ対象言語もオーソドックスな国をチョイスしている
metadataテーブルを参照して、DisplayNameとATTの乳ディスクリプションも設定してるから、テーブルの中身を書き換えて
asset,managementからlocalizetableのタブ開けるから

## admob
アプリIDも設定しなおして。今は別プロフェくとのID入っているから。
Assetsたぶ/google admob/settingから設定できる

## playersetting
ターゲットSDK,minSDKも適宜変えること。minSDKはadmobの要件に従いつつ、そこまで古すぎない程度を選んでおけばいい。