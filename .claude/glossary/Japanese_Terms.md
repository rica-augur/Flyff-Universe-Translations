# 日本語 用語集（単語・定訳集）

このファイルは Claude Code の作業補助用ファイルであり、リポジトリ本体の翻訳対象ファイル（83ファイル構成）には含まれません。

## 使い方

1. `Japanese/` 配下のファイルを翻訳・修正する前に、対象の英単語がこの表に存在するか確認する。
2. 存在する場合は、原則としてここに記載された訳語に合わせる。
3. まだ載っていない頻出語句（ゲーム内の共通UI語句、システム名、ステータス名など）を新しく訳した場合は、この表に追記する。
4. 表記揺れ（同じ英単語に対して複数の訳語が既存ファイル内に混在している）を見つけた場合は「備考」欄に記録する。表記揺れの統一自体は既存翻訳の修正になるため、別途ユーザーの指示・PRで対応すること（この用語集への記録だけで既存ファイルを一括置換しない）。

## 用語一覧

| English | 日本語（標準訳） | 備考 |
| --- | --- | --- |
| Level | レベル | |
| Guild | ギルド | |
| Quest | クエスト | |
| Item | アイテム | |
| Skill / Skills | スキル | |
| Monster | モンスター | |
| Dungeon | ダンジョン | |
| Inventory | インベントリ | UI名称としては「インベントリウィンドウ」表記も存在 |
| Weapon | 武器 | |
| Armor | 防具 | 「防御具」「アーマー」の表記揺れあり。要統一検討 |
| Penya | ペニャ | |
| Party | パーティー | 「パーティ」（長音なし）の表記揺れあり。要統一検討 |
| Character | キャラクター | |
| Attack（ステータス値） | 攻撃力 | 動作としての「攻撃」を指す場合は文脈で判断 |
| Defense（ステータス値） | 防御力 | |
| HP / MP / FP | HP / MP / FP | 略語のまま表記し、和訳しない |
| Gold | ゴールド | |
| NPC | NPC | 略語のまま表記し、和訳しない |
| Boss | ボス | |
| Equipment | 装備 | |
| Login | ログイン | |
| Server | サーバー | 複合語では「サーバ分類」等の表記も存在 |
| Buff | バフ | |
| Title | タイトル | |
| Achievement(s) | 実績 | 「業績」の表記揺れあり。要統一検討 |
| Friend | フレンド | |
| Shop | 商店 | |
| House（住宅オブジェクト） | ハウス | パーソナルハウス関連の設置物名。地名の一般名詞としての「家」ではなくハウジングシステムの建物オブジェクトを指す |
| Guardiane（地名そのもの） | ガルディア | マップ名`PROPMAP_TXT_000020`に準拠。ただし合成語「Guardiane Sanctuary」はダンジョン名として定着した「ガーディアンサンクチュアリ」を使う（住宅設置物や地名単体では「ガルディア」、ダンジョン名の一部としては「ガーディアン」で使い分け） |
| Ordinary（採集ノード等級） | 一般的な | `UI_LIFE_MASTERY_ORDINALY_*`の説明文に準拠 |
| Regular（採集ノード等級） | ありふれた | `UI_LIFE_MASTERY_REGULAR_*`の説明文に準拠 |
| Unique（採集ノード等級） | 独特な | `UI_LIFE_MASTERY_UNIQUE_*`の説明文に準拠 |
| Rare（採集ノード等級） | 希少な | `UI_LIFE_MASTERY_RARE_*`の説明文に準拠。UI上の品質表記としての「レア」とは別用途 |
| Legendary（採集ノード等級） | 伝説の | `UI_LIFE_MASTERY_LEGENDARY_*`の説明文に準拠 |
| Alchemy Desk | 錬金デスク | `ProductionRecipes.csv`の定訳に準拠 |
| Hearth | 暖炉 | `ProductionRecipes.csv`の定訳に準拠 |
| Carpentry Workspace | 木工作業台 | `ProductionRecipes.csv`の定訳に準拠 |
| Smithing Workspace | 鍛冶作業台 | `ProductionRecipes.csv`の定訳に準拠 |
| Medieval（家具シリーズ） | 中世 | |
| Pastel（家具シリーズ） | パステル | |
| Neon Valentines（家具シリーズ） | ネオンバレンタイン | `PROPITEM`のシングルパック名に準拠 |
| Drawer | ドロワー | 「Wooden Drawer」のみ「引き出し」表記あり（表記揺れ） |
| Bookcase / Bookshelf | 本棚 | |
| Sign（設置物） | サイン | |
|Darkon|ダーコン|地名|
|Coral Island|コーラルアイランド|地名|
|Azria|アズリア|地名|
|Rhisis|リシス|地名|
|Madrigal|マドリガル|地名|
|Flaris|フラリス|地名|
|Flarine|フラリス|地名|
|Saint Morning（地名） | セイントモーニング ||
|St Morning（地名） | セイントモーニング ||
| Couple Menu | カップルメニュー | `Help.csv`準拠 |
| Life（ライフスキルメニュー） | ライフスキル | `Help.csv`準拠。生活スキル全般を指すメニュー名 |
| Fishing Menu | フィッシングメニュー | `Help.csv`準拠 |
| Pet Training | ペットトレーニング | `Help.csv`準拠 |
| Housing Objects | ハウジングオブジェクト | `Help.csv`準拠 |
| Production（生産メニュー） | 生産 | `Help.csv`準拠 |

## 防具シリーズ名の語幹（音訳）

`Items.csv`（Helmet/Suit/Gauntlets/Boots等）と`EquipSets.csv`（Set名）で共通して使われる防具シリーズ名の語幹。いずれも`Items.csv`内の既存訳（ヘルメット表記）に準拠した音訳。同じ語幹が複数ファイルに出現するため、新規シリーズを翻訳する際は先にこの表と`Items.csv`を確認すること。

| English（語幹） | 日本語（音訳） | 備考 |
| --- | --- | --- |
| Runthiel | ランティエル | |
| Runthien | ランティエン | |
| Rethanor | レサノール | |
| Rethanar | レサナー | |
| Zendric | ゼンドリック | |
| Zendricar | ゼンドリカー | |
| Khorviel | コルヴィエル | |
| Khorvien | コルヴィエン | |
| Zaythor | ゼイソー | |
| Zaythar | ゼイサー | |
| Vornithic | ヴォルニシック | |
| Vornithicar | ヴォルニシカー | |
| Dornith | ドルニス | |
| Dornyth | ドルニュス | |
| Quostrel | クォストレル | |
| Quostren | クォストレン | |
| Chyrelle | シレル | |
| Chyrella | シレラ | |
| Noltrave | ノルトレイヴ | |
| Noltrava | ノルトラヴァ | |
| Frodral | フロドラル | |
| Frodrel | フロドレル | |
| Treviron | トレヴィロン | |
| Treviran | トレヴィラン | |
| Lenvire | レンヴィール | |
| Lenvira | レンヴィラ | |
| Ordelin | オルデリン | |
| Ordelyn | オルデリュン | |
| Tracien | トラシエン | |
| Tracior | トラシオール | |
| Lorvenic | ロルヴェニック | |
| Lorvenicar | ロルヴェニカー | |
| Etranor | エトラノール | |
| Etranar | エトラナー | |
| Lyzarel | リザレル | |
| Lyzaren | リザレン | |
| Exiran | エクシラン | |
| Exiren | エクシレン | |
| Haskrel | ハスクレル | |
| Haskren | ハスクレン | |
| Kevric | ケブリック | |
| Kevricar | ケブリカー | |
| Brakiven | ブラキヴェン | |
| Brakivar | ブラキヴァー | |
| Zorect | ゾレクト | |
| Zoracet | ゾラセット | 語幹自体が「セット」で終わるため、Set表記では「ゾラセットセット」となる（Items.csvの既存音訳に準拠） |
| Sholthar | ショルサー | |
| Sholtharen | ショルサレン | |
| Ustamel | ウスタメル | |
| Ustamen | ウスタメン | |
| Obbric | オブリック | |
| Obbricar | オブリカー | |
| Yrenoth | イレノス | |
| Yrenath | イレナス | |
| Vostran | ヴォストラン | |
| Vostren | ヴォストレン | |
| Virashon | ヴィラション | |
| Verashan | ヴェラシャン | |
| Menicor | メニコール | |
| Maenicar | メニカー | |
| Tremiel | トレミエル | |
| Tramien | トラミエン | |
| Calthien | カルシエン | |
| Calthior | カルシオル | |
| Celestial Phoenix（防具シリーズ接頭語） | セレスティアルフェニックス | |
| Primordial（防具シリーズ接頭語） | プリモーディアル | |



