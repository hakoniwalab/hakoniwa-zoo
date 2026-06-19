# TurtleBot3 Sensor Extension

## Summary

TurtleBot3にカメラ、LiDAR、超音波センサなどを追加し、MuJoCoモデル・PDU定義・制御プログラムを連携させるためのユースケースです。

センサ追加時の設定手順を整理し、箱庭による拡張方法を分かりやすくすることを目的としています。

## Persona

* TurtleBot3利用者
* ROS2利用者
* MuJoCoベースのロボット開発者
* センサ拡張を試したい学生・研究者

## Problem

ロボットにセンサを追加すると、

* MJCF修正
* PDU定義追加
* endpoint設定
* 制御コード修正

が必要になります。

それぞれの関係が見えにくく、どこを変更すればよいか分かりづらいことがあります。

## Goal

* センサ追加手順を整理する
* MJCFとPDUの対応関係を見える化する
* asset manifestから構成を確認できるようにする
* 最小サンプルを提供する

## Why Hakoniwa

箱庭ではセンサ入出力をPDUとして扱うため、物理シミュレータと制御プログラムを疎結合に保てます。

また、asset manifestによってロボット構成を可視化できるため、拡張ポイントを理解しやすくなります。

## Components

| Component              | Role          |
| ---------------------- | ------------- |
| hakoniwa-mujoco-robots | TurtleBot3モデル |
| hakoniwa-core-pro      | PDU通信・時刻同期    |
| hakoniwa-pdu-python    | Python制御プログラム |
| Asset Manifest         | 構成管理          |
| PDU Definitions        | データ型定義        |

## Demo

候補:

* TurtleBot3カメラ追加
* 超音波センサ追加
* Asset Manifestによる構成確認

## Missing Pieces

* センサ追加チュートリアル
* テンプレートJSON
* Manifest Inspector
* PDU Adapterサンプル

## Collaboration

* センサ追加サンプル作成
* ロボット教材整備
* ROS2接続例
* センサ構成テンプレート整備

## Status

Draft
