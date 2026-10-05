# Excel/VBA 開発の手順とソース管理

Windows版デスクトップExcelとVBAで業務ツールを作るための、実装手順とソース管理の方針をまとめたリポジトリです。特定の業務・案件の要件は含みません。

現在は手順と方針の段階で、Excelブック、VBAソース、ビルド用スクリプトは含みません。

## 構成

```text
.
├── README.md
├── .gitignore
├── docs/
│   └── code-and-workbook-management.md
└── skills/
    └── excel-vba-implementation/
        └── SKILL.md
```

- [コード・フォーム・シート管理ガイド](docs/code-and-workbook-management.md)：コード・フォーム・ひな形の正本、ビルドと検証、Excel内で変更した内容の取り込み、スクリプトの呼び出し仕様、AIエージェントの作業規則。
- [Excel実装手順スキル](skills/excel-vba-implementation/SKILL.md)：要件の抽出から、保存と外部連携の実機確認、小さな一連の実装、機能追加、受入までの手順。

## 案件で使うとき

案件ごとの業務要件は、その案件の要件書（例：`docs/requirements.md`）として別に用意します。AIまたは開発担当者に次を渡してください。

> `docs/requirements.md`、`skills/excel-vba-implementation/SKILL.md`、`docs/code-and-workbook-management.md` を読み、Excel/VBA実装を進めてください。未確定事項を推測で本番仕様にせず、まず一つの業務の流れを入力から保存・再起動まで通してください。

同梱スキルはファイルを読んで利用できます。特定のAIへの自動インストールや、個人環境の別スキルは前提にしません。

## 含めないもの

実業務データ、認証情報、端末固有設定を追加しないでください。Excelブックを追加するときは、実データが含まれていないことを確認してください。
