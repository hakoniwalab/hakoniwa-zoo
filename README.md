# Hakoniwa Zoo

Hakoniwa Zoo は、箱庭で実現できるユースケースを集めたカタログです。

ここでは、箱庭の機能を説明するのではなく、利用者が抱える「やりたいこと」や「困りごと」から、どの箱庭コンポーネントを組み合わせればよいかを整理します。

## Use Case Cards

| Use Case                                                             | 誰向け             | 困りごと                              | 状態    |
| -------------------------------------------------------------------- | --------------- | --------------------------------- | ----- |
| [PX4 Motor Fault Injection](./usecases/px4-motor-fault-injection.md) | ドローンR&D / 大学研究室 | 実機で故障試験を行うのは危険で再現性が低い             | Draft |
| [LEGO Digital Twin](./usecases/lego-digital-twin.md)                 | ロボット教育 / PoC担当者 | 実機とシミュレータで同じ制御コードを使いたい            | Idea  |
| [Robot Sensor Extension](./usecases/robot-sensor-extension.md)    | ROS / MuJoCo利用者 | センサ追加時のPDU・MJCF・endpoint設定が分かりにくい | Draft |

## Cardの読み方

各 Use Case Card は、次の観点で整理します。

| 項目             | 意味            |
| -------------- | ------------- |
| Persona        | 誰のためのユースケースか  |
| Problem        | 何に困っているか      |
| Goal           | 何を実現したいか      |
| Why Hakoniwa   | なぜ箱庭でやる意味があるか |
| Components     | 関連するリポジトリ・機能  |
| Demo           | 動作デモや動画       |
| Missing Pieces | まだ足りないもの      |
| Collaboration  | 一緒に作りたいこと     |

## Status

| Status     | 意味        |
| ---------- | --------- |
| Idea       | まだ構想段階    |
| Draft      | カードとして整理中 |
| Demo Ready | 最小デモあり    |
| Published  | 外部公開済み    |
