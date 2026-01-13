# depth-view-with-cc

Webカメラで顔を追跡し、視点に応じたパララックス（視差）効果で奥行きを感じる3Dデモです。

## 実行方法

ローカルで実行する場合、GLBファイルの読み込みにCORS制限がかかるため、ローカルサーバーが必要です。

```bash
# プロジェクトディレクトリで実行
python -m http.server 8000
```

ブラウザで http://localhost:8000 を開くと、Webカメラが起動し、顔の位置に応じて3Dシーンの視点が変化します。

## 特徴

- **顔追跡**: MediaPipe Face Detectionによるリアルタイム顔検出
- **パララックス効果**: Off-Axis Projection（非軸投影）による自然な奥行き表現
- **3Dシーン**: グリッド付きの部屋と3Dモデルを表示
- **モデル切り替え**: 猫モデルとキューブを切り替え可能
- **サイズ調整**: スライダーでモデルサイズを変更可能

## 使用ライブラリ

- [Three.js](https://threejs.org/) v0.160.0 - 3Dレンダリング
- [MediaPipe Face Detection](https://developers.google.com/mediapipe/solutions/vision/face_detector) - 顔検出

## 使用ツール

- **コード**: Claude Code (Opus 4.5)
- **3Dモデル**: Tripo Studio
