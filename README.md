# vietnam

一個由 LLM 維護的個人知識庫，記錄跟越南有關的事。架構與規則沿用 pey-knowledge，方法出自 Andrej Karpathy 的 llm-wiki。

**分工只有一條線：素材與判斷是人的，整理與記帳是 agent 的。**

## 從哪裡開始

| 想做什麼 | 去哪 |
|---|---|
| 看有哪些東西 | [wiki/index.md](wiki/index.md) |
| 查規則原文 | [CLAUDE.md](CLAUDE.md) |
| 看做過什麼 | [log.md](log.md) |
| 看知識庫自己的維護頁 | [wiki/kb-maintenance/](wiki/kb-maintenance/README.md) |

## 四棵樹

```
raw/       原始素材，不可變。按「輸入情境」分批
wiki/      agent 整理出來的 markdown。一個「事」一個資料夾
archive/   已失效的文件，手動搬進來
output/    產出物（簡報、PDF、HTML），平放。內容只取自 wiki
```

資料只往一個方向流：`raw/` → `wiki/` → `output/`。

## 五條要記住的規則

完整版在 [CLAUDE.md](CLAUDE.md)。

1. **raw 不動。** 內容和檔名都不改。新查的資料（網頁、地圖查詢、sub-agent 回報）先存進 raw
2. **wiki 的每一條都能走回去。** 走回 raw 的檔案和位置；你的決定走回 `log.md`。找不到的標「raw 沒有存」或「未確認」，不補值
3. **output 只取 wiki。** 改行程頁這類產出物，先改 wiki，再照 wiki 改
4. **你決定，agent 記帳。** 矛盾和選項並排列給你，agent 不挑一邊
5. **會重用的跟一次性的分開。** 景點放 `hanoi-sights/`，這一趟的行程放 `hanoi-trip-2026-10/`

根層只有三個檔：本檔、[CLAUDE.md](CLAUDE.md)、[log.md](log.md)。

## 怎麼用

丟新素材進 `raw/`，然後跟 Claude Code 說「幫我 ingest」。
要改產出物就直接說要改什麼，例如「12/31 改去 Diamond」。agent 會先改 wiki，再改 `output/`。
想健檢就說「跑一次 lint」。
想知道缺什麼就問「還需要釐清什麼」。

規則寫在 [CLAUDE.md](CLAUDE.md)，Claude Code 每次開啟自動讀。
