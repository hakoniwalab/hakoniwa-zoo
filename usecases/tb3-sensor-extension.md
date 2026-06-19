# Robot Sensor Extension

## Summary

既存のロボットに新しいセンサを追加し、シミュレータと制御プログラムを連携させたい人向けのユースケースです。

箱庭では、センサモデル、PDU定義、Endpoint実装、制御プログラムを組み合わせることで、実機と同じ構成を仮想環境上で再現できます。

本ユースケースでは、超音波センサ、カメラ、LiDARなどの追加方法を整理し、ロボット機能拡張の標準パターンを示します。

## Persona

* ロボット開発者
* ROS2利用者
* MuJoCo利用者
* 教育・研究用途でロボットを拡張したい人

## Problem

ロボットにセンサを追加する際には、

* ロボットモデルの修正
* センサ設定
* PDU定義
* Endpoint実装
* 制御プログラム修正

が必要になります。

これらの対応関係が見えにくいため、拡張作業の難易度が高くなります。

## Goal

* ロボットへのセンサ追加手順を整理する
* モデルとPDUの対応関係を見える化する
* 制御プログラムとの接続方法を標準化する
* センサ拡張の再利用可能なパターンを提供する

## Why Hakoniwa

箱庭では、センサ・アクチュエータをPDUとして抽象化します。

そのため、物理シミュレータと制御プログラムを疎結合に保ちながら機能拡張できます。

また、Asset Manifestを利用することで、ロボット構成全体を整理しながら開発できます。

## Components

| Component              | Role          |
| ---------------------- | ------------- |
| hakoniwa-mujoco-robots | ロボットモデルとセンサ実装 |
| hakoniwa-core-pro      | PDU通信・時刻同期    |
| hakoniwa-pdu-python    | Python制御プログラム |
| Asset Manifest         | 構成管理          |
| PDU Definitions        | データ型定義        |

## Existing Tutorials

### Ultrasonic Sensor

既存ロボットへ超音波センサを追加する例。

対象:

* MJCFモデル拡張
* PDU定義追加
* Endpoint実装
* Python制御プログラム連携

### Camera Sensor

既存ロボットへカメラセンサを追加する例。

対象:

* カメラ設定
* PDU画像転送
* 制御プログラム連携

### Future Examples

* LiDAR
* GPS
* IMU
* 深度カメラ

## Demo

* TurtleBot3 Ultrasonic Sensor
* TurtleBot3 Camera Sensor
* Asset Manifestによる構成確認

## Missing Pieces

* センサ追加テンプレート
* Asset Manifest Inspector
* PDU Adapterサンプル
* センサ追加ウィザード

## Collaboration

* ロボット教材整備
* センサ追加サンプル拡充
* ROS2連携事例
* 教育向けコンテンツ整備

## Status

Draft
