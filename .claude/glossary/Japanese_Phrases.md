# 日本語 意訳・言い回し集

このファイルは Claude Code の作業補助用ファイルであり、リポジトリ本体の翻訳対象ファイルには含まれません。

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

## Guild Siege（`GuildCombat*.txt`）の順位報酬表記（2026-08-08、`GuildCombat60.txt`翻訳時に確認）

`UI.csv`の`UI_GUILDCOMBAT_OFFER_PRESENT1〜3`（既存訳）は「Winning Guild/Second Guild/Third Guild」形式を「優勝ギルド／第2ギルド／第3ギルド」、「x number of participating guilds」を「×参加ギルド数」と訳している。一方`GuildCombat60/80/165.txt`系は原文が「1st Place Guild/2nd Place Guild/…/6th–10th Place Guilds」という**序数＋Place**形式のため、上記の「第Nギルド」ではなく「{数字}位ギルド」（例：1st Place Guild→1位ギルド、6th–10th Place Guilds→6〜10位ギルド、範囲はenダッシュではなく全角チルダ「〜」）に統一する。「x number of participating guilds」は同じく「×参加ギルド数」を踏襲。箇条書きの記号は原文の「-」とインデントをそのまま残す（`UI.csv`側の「・」とは別ファイルなので混同しない）。

その他の定訳（`GuildCombat*.txt`翻訳時に確認）：
- Guild Siege → ギルドコンバット（`TextClient.csv`の`TEXTCLIENT_GUILDCOMBAT*`系に準拠）
- second/third class change → 2次/3次転職
- [Guild Siege Manager] {name} → [ギルコンマネージャー]{カタカナ名}（`Characters.csv`準拠。「ギルコン」は略称として定着済み）
- Blue Chip(s) → ブルーチップ

## `RandomItemOptions.csv`のステータス接尾辞（`of STR`等）の表記（2026-08-12）

`RandomItemOptions.csv`限定のルール。英語原文はアイテム名の後ろに付与される接尾辞（例：`Item of STR`、`Item STR+`）で、英語ではこの位置でも自然に読める。しかし日本語訳は「力の」のようにアイテム名の前に置く前提の言い回しになるため、アイテム名の後ろに付くと「の」で終わって不自然になる。アイテム名の前に付け替えることは翻訳の範囲外（キー・結合順序を変更できない）のため、代わりに角括弧で挟む形式（例：「力の」→「[力]」、「力と体力の」→「[力と体力]」）に統一する（2026-08-12、ユーザー指示で`PROPITEMETC_INC_000083〜000130`の全48件に適用）。**このルールは`RandomItemOptions.csv`に限定**し、他ファイルの同様の「〜の」接頭表現には適用しない。

## 職業（First Job）フレーバーテキストの文体（`TextClient.csv`の`TEXTCLIENT_STATUE_*`、2026-07-30）

北フラリスの職業別銅像の説明文。`TEXTCLIENT_STATUE_VAGRANT`（"The start of all. You are Vagrant."→「すべての始まり。あなたは放浪者。」）の体言止め・詩的な文体に合わせ、他の職業（BP=ビルポスター、RM=リングマスター、JESTER=ジェスター、RANGER=レンジャー、KNIGHT=ナイト、BLADE=ブレード、ELE=エレメンター、PSY=サイキーパー）も「{形容表現}、{役割を表す一文}。」の体言止め＋文語調で統一（例：BP「伝説の戦士、その身に宿るは戦の魂。」）。通常のシステムメッセージ（だ・である調やですます調）とは別扱いの、演出用の特別な文体である点に注意。

## `UI.csv`のダンジョン入場条件表示（`UI_DUNGEON_REQ_LEADER_*`）での「Creator」の扱い（2026-08-12）

`UI_DUNGEON_REQ_LEADER_QUEST`（"Req. Creator Quest: %s"）、`UI_DUNGEON_REQ_LEADER_ITEM`（"Req. Creator Items:"）、`UI_DUNGEON_REQ_LEADER_GOLD`（"Creator Entrance Fee: %s Penya"）は、ダンジョン入場条件一覧に並ぶラベル。原文の「Creator」（パーティ作成者）を律儀に直訳すると読み手に伝わりにくい（当初訳の「創造主」は「神」のように読めて分かりづらいとの指摘あり）ため、この3キーに限っては「Creator」を訳文から落とし、入場条件そのものを簡潔に説明する言い回しに統一した：「必須クエスト: %s」「入場に必要なアイテム:」「ダンジョン入場料: %s ペニャ」（2026-08-12、ユーザーが直接修正）。同じ並びの`UI_DUNGEON_REQ_LEADER_COMPLETE_QUEST`（既存訳「必要クエスト完了者: %s」）も同様にCreator抜きの言い回し。一方`UI_DUNGEON_MIN_LEADER_LEVEL`（"Minimum Creator Level: %d"→「最小作成者レベル: %d」）はプレイヤー個人の属性を指すため対象外（「作成者」表記のまま）。
