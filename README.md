# ビジネスチーム

> 🎯 **ミッション**
> 四半期、年間、2033年の売上・利益目標達成

---

## 📑 Table of Contents

1. [リポジトリの範囲](#1-リポジトリの範囲)
2. [オンボーディング手順](#2-オンボーディング手順)
3. [タスク管理](#3-タスク管理)
4. [GitHub Projects でのタスク状況可視化](#4-github-projects-でのタスク状況可視化)
5. [ストレージポリシー](#5-ストレージポリシー)
6. [週次サイクル](#6-週次サイクル)
7. [FAQ](#7-faq)

---

## 1. 📦 リポジトリの範囲

このリポジトリは **ビジネスサイド（事業開発・セールス・マーケ・法務・財務・人事・総務）** のタスクを一元管理します。プロダクト / デザイン / AI 研究等の技術系タスクは各担当リポジトリで管理し、プロジェクト単位の横断状況は GitHub Projects で把握します。

| 本リポジトリが扱うもの                                                     | 他リポジトリが扱うもの                                                           |
| --------------------------------------------------------------- | --------------------------------------------------------------------- |
| 市場調査、パートナーシップ、セールスパイプライン、マーケティング企画、契約・法務対応、資金調達、財務報告、HR・採用、社内規程 | UX/UI デザイン（Design）、アプリ / インフラ開発（Application/Infra）、AI 研究（AI Research） |

---

## 2. 🚀 オンボーディング手順

1. **アクセス権**: `Business` チームに追加され、Writer 権限があることを確認。
2. **使用ツール**

   * **Notion**（長文ドキュメント、マニュアル、議事録）
   * **Google Workspace (Drive, Docs, Sheets, Slides)**（契約書、提案書、財務資料）
   * **HubSpot / CRM**（セールスパイプライン）
   * **Slack**（コミュニケーション）
   * **GitHub Issues / Projects**（タスクトラッキング）
3. **Business Board** をブックマーク: <[https://github.com/orgs/](https://github.com/orgs/)<org>/projects/2>

---

## 3. 📝 タスク管理

### 3.1 Issue テンプレート

新規 Issue → `Business Task` を選択し、以下を記入：

* **Problem / Goal** – 解決する課題・目的
* **KPI / 指標** – 達成を測る具体値（MQL 数、ARR、採用完了数 など）
* **Acceptance Criteria** – 完了条件
* **Deliverables** – 例: Notion ページ、Drive 資料、提案書 PDF
* **Reviewers** – チームメンバー 1 名以上 + 経営陣/担当 VP
* **Dependencies** – 関連 Issue（"blocks" / "blocked by"）

> **共通ルール**: *Issue にリンクされていないものは存在しない*。

### 3.2 ラベル

| カテゴリ        | ラベル例                                                                             |
| ----------- | -------------------------------------------------------------------------------- |
| **状態（1 つ）** | `todo`, `in-progress`, `review`, `blocked`, `done`                               |
| **種別（複数可）** | `sales`, `marketing`, `partnership`, `finance`, `legal`, `hr`, `ops`, `research` |
| **優先度**     | `p0`, `p1`, `p2`                                                                 |
| **期間ラベル**   | `q3-2025`, `q4-2025` など四半期単位                                                     |

Projects ボードでカードを移動すると `状態` ラベルが自動更新されます。

---

## 4. 📊 GitHub Projects でのタスク状況可視化

* カラム: Backlog → Todo → In Progress → Review → Done
* スイムレーン: プロジェクト（例: シリーズ B 資金調達、薬機法対応、海外市場調査）ごとに分離
* フィルター例: `label:finance status:in-progress`

---

## 5. 🗂 ストレージポリシー

| 用途                  | プラットフォーム                                      | 運用ルール                                                  |
| ------------------- | --------------------------------------------- | ------------------------------------------------------ |
| 契約書・法務文書            | Google Drive <br>`/Legal/<yyyy>/<案件名>/`       | 編集履歴を残すため Google Docs を推奨。PDF 化したら "v1" など版数をファイル名に追記。 |
| セールス資料・提案書          | Google Drive <br>`/Sales/<client>/<yyyy-mm>/` | 送付版は `-client` サフィックスを付ける。                             |
| 長文ドキュメント (SOP、議事録)  | Notion                                        | テンプレートからページ生成→ ページ URL を Issue に貼付                     |
| 財務モデル / レポート        | Google Sheets                                 | `FY2026_Budget_v*.xlsx` にバージョン付与。                      |
| マーケティングアセット (画像・動画) | Google Drive / Git LFS (小容量)                  | 公開用最終版のみ Git LFS へ同期可。                                 |
| コミュニケーション           | Slack #business                               | 決定事項は必ず Issue へ要約してリンク                                 |

⚠️ **必須**: 上記ストレージで管理し、Issue からリンクで辿れる状態にすること。

### 5.1 命名規則

| 種類         | パターン                         | 例                           |
| ---------- | ---------------------------- | --------------------------- |
| Drive フォルダ | `/Sales/<client>/<yyyy-mm>/` | `/Sales/HospitalX/2025-07/` |
| Drive ファイル | `<topic>_v<version>.<ext>`   | `InvestorDeck_v3.pdf`       |
| Notion ページ | `[Issue-<number>] <title>`   | `[Issue-42] Q3 OKR Draft`   |

---

## 6. 🔄 週次サイクル

| 時間（JST） | 内容                    |
| ------- | --------------------- |
| 月 09:00 | 週次営業・パイプラインレビュー（30 分） |
| 水 15:00 | マーケティング/PR レビュー（30 分） |
| 金 17:00 | OKR 進捗 / Retro（30 分）  |

---

## 7. ❓ FAQ

<details>
<summary>契約書のレビュー依頼フローは？</summary>
Notion テンプレ「📝 Contract Review」を複製 → 法務担当にメンション → 完了後に Drive PDF を Issue にリンクして `done`。
</details>

<details>
<summary>外部ベンダーとの NDA 保存場所は？</summary>
`/Legal/NDA/<yyyy>/` フォルダを守ってください。
</details>

<details>
<summary>機密データの共有制限は？</summary>
Drive ファイルは *社内限定* link。外部共有時は VP 承認必須。
</details>

---

### ビジネス成長を加速させましょう！🚀
