# 日本語 意訳・言い回し集

このファイルは Claude Code の作業補助用ファイルであり、リポジトリ本体の翻訳対象ファイル（83ファイル構成）には含まれません。

単語単位の定訳は [Japanese_Terms.md](Japanese_Terms.md) を参照。こちらは、直訳ではなく意訳した表現・定型文・文体（口調、敬語レベルなど）をまとめる。

## 使い方

1. `Japanese/` 配下のファイルを翻訳・修正する前に、似た意味・用途の英文がこの表に存在するか確認する。
2. 存在する場合は、同じ言い回し・文体に合わせる。
3. 直訳ではなく意訳した表現や、繰り返し登場する定型文（例：エラーメッセージ、確認ダイアログ、システム通知などの言い回し）を新しく訳した場合は、この表に追記する。

## 言い回し一覧

| English（原文パターン） | 日本語（採用した意訳） | 使用箇所の例 / 備考 |
| --- | --- | --- |
| {Monster} Slayer {N} | {モンスター名} スレイヤー {N}（名前とスレイヤーの間に半角スペース） | `Achievements.csv`の`ACHIEVEMENT_KILL_*_LVL1〜4`。討伐実績のティア名。同じ実績内で末尾のみ「{モンスター名} ハンター」になるパターンと、スペース無しで「{モンスター名}ハンター{N}」→「{モンスター名}キラー」になるパターンの2系統が既存訳に混在（後者は`CAVEMANCHIEF`等の一部モンスターのみ）。新規追加時は同系統内で先例に合わせる |
| Reach level {N} in the {Year} Flyff World Championship. | Flyff World チャンピオンシップでレベル{N}に到達する。 | `Achievements.csv`のFWCシリーズ実績DESC。plain形（〜する。）で統一 |
| Win / Get second place / Get third place in the {Year} Flyff World Championship {PvP\|PvE} Competition. | 〜で勝利する。／〜で2位を獲得する。／〜で3位になる。 | 同上。2023年分の既存訳は「フリフワールドチャンピオンシップ」表記だったが、2024年以降は「Flyff World チャンピオンシップ」（英語のまま）表記に変わっている。新規は後者に合わせる |
| Achievement DESC全般の文体 | plain形（「〜する。」「〜を上げる。」）が基本。ただしEvents.csv等からそのまま流用された文言（ログインイベント系）は「〜しましょう!」等のますformが混在 | 既存訳の大半（Master Quest系、Pillシリーズ等）はplain形。新規追加時は流用元が無ければplain形に合わせる |
| Newbie / (無印) / Expert / Master ＋ 職業名（ライフスキル実績） | 見習い{職業}／{職業}／エキスパート{職業}／マスター{職業} | `Achievements.csv`の生活スキル系実績（採集・伐採・採掘・釣り・料理・錬金術・木工・鍛冶）。職業名は既存訳「木こり」（`WOOD_CUTTING_TITLE02`）に準拠して統一 |
| Master of {Skill} | {Skill}マスター | 同上POINTS_NAME |
| Raise your {Skill} mastery. | {Skill}のマスタリーを上げる。 | 同上POINTS_DESC。「マスタリーポイント」は`UI.csv`の`UI_LIFE_MASTERY_RANKING_POINT`に準拠した既存訳語 |
| Small / Captain / Giant / Great ＋ モンスター種族名（`Movers.csv`のティア表記） | スモール・{種族名}／キャプテン・{種族名}／ジャイアント・{種族名}／グレート・{種族名}（中黒でつなぐ） | ティア接頭語がカタカナのため、種族名部分が意味を持つ英単語（例：`Cursed Warden`）であっても意味訳（「呪われた番人」）ではなくカタカナ音訳（「カースド・ウォーデン」）に統一する。ここでの種族名は固有名詞的に扱い、`Items.csv`等の一般アイテム名文脈での「Cursed→呪われた」定訳とは別物として扱う（ユーザー指示により2026-07-28修正、対象：`PROPMOVER_TXT_400308〜400316`） |

### 表記揺れ（備考・修正しない）

- `Movers.csv`の「ジャイアント・〇〇」系で漢字混じりの訳が3件ある（`PROPMOVER_TXT_000116` Giant Mr. Pumpkin→「ジャイアント・カボチャ男爵」、`PROPMOVER_TXT_000588` Mutant Giant 2nd Class Fefern→「ジャイアント・2級フェフェルン」、`PROPMOVER_TXT_000600` Mutant Giant Bang King→「ジャイアント・ヴァン改」）。上記の`Cursed Warden`と類似のパターンだが、これらは古くからの既存訳のためユーザー指示により**触らない**（2026-07-28確認）。
