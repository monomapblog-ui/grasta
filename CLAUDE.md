# GRASTA サイト運用メモ

## サイト情報
- 本番URL: https://gravurestation.jp
- リポジトリ: monomapblog-ui/grasta
- 静的HTMLサイト（GitHub Pages）

## ニュースリリースの更新方法
`company.html` のニュースリリースセクションへの追記は、**このセッション内で「〇〇のニュースを追加して」と伝えればOK**。
Claude が HTML を編集→コミット→mainへ反映まで対応する。

追記テンプレート（`<!-- ▼ 新しいニュースをここに追加 ▼ -->` の直下に挿入）:
```html
<li class="flex flex-col sm:flex-row sm:items-center gap-2 sm:gap-4 px-5 py-4 hover:bg-slate-50 transition">
  <time class="text-xs text-gray-400 whitespace-nowrap font-mono">2026.XX.XX</time>
  <span class="inline-block bg-[#b32b47]/10 text-[#b32b47] text-xs font-medium px-2 py-0.5 rounded whitespace-nowrap">お知らせ</span>
  <span class="text-sm text-gray-800">タイトル</span>
</li>
```

カテゴリラベルの種類: `お知らせ` / `プレスリリース` / `イベント` / `採用` / `メディア`

## 会社情報
- 会社名: 合同会社グラステ（GRASTA LLC）
- 設立: 令和8年7月2日（2026年7月2日）
- 法人番号: 5011103017693
- 所在地: 東京都新宿区
- メール: info@gravurestation.jp
