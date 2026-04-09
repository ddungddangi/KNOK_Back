# KNOK (AI Interview Coaching Service)
[![Github Link](https://img.shields.io/badge/GitHub-Repository-181717?style=flat-square&logo=github)](https://github.com/ddungddangi/KNOK_Front)
[![Demo Video](https://img.shields.io/badge/YouTube-Demonstration_Video-FF0000?style=flat-square&logo=youtube)](https://m.youtube.com/watch?v=1BNbFp9NaIE)
[![Figma](https://img.shields.io/badge/Figma-Design_Link-F24E1E?style=flat-square&logo=figma)](https://www.figma.com/design/9A2XCWjwngTpM3VCQUHmFp/AI-interview-website?node-id=0-1&t=8bjxynOs9cGKTaLe-1)

## 📌 プロジェクト概要
- **プロジェクト説明**: リアルタイムの質問生成、音声分析、フィードバックを提供する AI 模擬面接Webサービス
- **開発期間**: 2025.05 ~ 2025.07（10週間）
- **参加人数**：6名
- **技術スタック**: TypeScript, Tailwind CSS, Figma, Django REST Framework, AWS Cognito, S3, Lambda, Bedrock（Claude）, DynamoDB, WebSocket, ECS, CloudWatch, Prometheus, Grafana
- **担当役割**: バックエンド

### 💡 主な担当業務と成果
* **バックエンド API 構成の実装**
  * 認証連携、質問生成、フィードバック処理のためのバックエンド API 構成を実装しました。
* **データ処理構造の改善**
  * データ保存・取得方式を見直し、S3・DynamoDB を活用した構成へ改善しました。
* **応答時間の短縮**
  * ユーザー向けフィードバックの応答時間を約20秒から約5秒へ短縮し、サービスの使用感を向上させました。

---

## 🎯 サービス概要と開発の背景 (Service Overview)

> コーディングブートキャンプ中、同僚の就職活動を支援する実践的なツールを作りたいと考えました。アンケート調査を実施した結果、多くの受講生が「面接段階」に最大の課題を感じていることが分かりました。
> そこで、単純なQ&Aツールにとどまらず、**超現実的でインタラクティブな模擬面接体験を提供するAIサービス「KNOK」**を開発しました。

### 🌟 Our Goal
ユーザーの履歴書に基づいたパーソナライズされた質問、動的な追加質問（深掘り）、姿勢や回答内容に対するリアルタイムなフィードバックを提供することで、実際の面接環境をシミュレーションし、ユーザーの面接に対する自信を高めることを目標としています。

---

## 🏗 アーキテクチャ (Architecture)
<img width="578" height="287" alt="화면 캡처 2025-09-21 153135" src="https://github.com/user-attachments/assets/02b2bd0e-85b1-4ac4-be61-079643d84ae3" />

## Tech Stack
![캡처 JPG](https://github.com/user-attachments/assets/5c096858-7f1a-4a16-8976-5b4fd759f0cd)

## 💻 サイト画面 (Site Image)
<img width="2203" height="1119" alt="image (2)" src="https://github.com/user-attachments/assets/70d97cbe-0049-4a37-ad7b-90a7dd097740" />

---

## 🧠 プロジェクトを通じた学び (Learnings & Takeaways)

### アーキテクチャのトレードオフに関する考察
本プロジェクトを通じて、**「セキュリティの強化」と「アーキテクチャの複雑化・運用負荷の増加」の間にあるトレードオフ**を実務として直接経験しました。

VPCを分離してセキュリティを高めた一方で、ネットワークの複雑性が増した経験から、**「3層アーキテクチャ（3-Tier Architecture）が常にすべての正解ではない」**という結論に至りました。
最も重要なのは、特定のビジネスの規模（Scale）と目標（Goal）に真に最適化されたアーキテクチャを柔軟に設計・選択することであると深く学びました。
