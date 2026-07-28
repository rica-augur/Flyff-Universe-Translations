# 日本語 用語集（単語・定訳集）

このファイルは Claude Code の作業補助用ファイルであり、リポジトリ本体の翻訳対象ファイルには含まれません。

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
| Mysterious Castle | 神秘の城 | `UI.csv`の`UI_MYSTCASTLE_*`、`Items.csv`準拠 |
| Mysterious Box | ミステリアスボックス | `Items.csv`の`Mysterious Box Lv1〜4`準拠。「Mysterious Castle」とは訳し分ける（意訳の神秘の城 / 音訳のミステリアスボックス） |
| Hoe（採集道具） | くわ | `PROPITEM_TXT_133000〜133007`。「鍬」は難読漢字のためユーザーがひらがな表記に修正（2026-07-29）。他の採集道具名で似た難読漢字が出た場合もひらがな表記を検討する |
| Bundle | バンドル | `Items.csv`のパッケージ系アイテム名 |
| Door Prize | ドア賞品 | `Items.csv`のイベント抽選アイテム名 |
| Soul-Linked / (Scroll of Unbinding文脈のSoul-Bound) | 帰属 | 「All items are Soul-Linked.」→「全てのアイテムはプレイヤーに帰属されています。」（パッケージ説明文の「All items are also linked.」→「アイテムは全て帰属です。」とは文体が少し異なるが同義） |
| Ultimate Weapon / Ultimate Accessory（装備の等級名） | アルティマ武器 / アルティマアクセサリー | `PROPITEM_TXT_122501`等に準拠。同じ「Ultimate」でも「Scroll of Ultimate Bonus」等のバフ・巻物文脈では音訳「アルティメット」を使う（例：アルティメットボーナスの巻物）。等級名としての武器・アクセサリーか、バフ効果名かで訳し分ける |
| Lunar（Lunar New Year文脈） | 旧正月 | `PROPITEM_TXT_200302`等に準拠。「Lunar New Year Coupon」等はそのまま「旧正月」を使い、音訳「ルナー」にしない |
| Trans（ペット変身オーブ、`PROPITEM_TXT_006094`等の`~ Trans`） | オーブ | 例：「Aibatt Trans」→「アイバット・オーブ」。「Trans Random Box」のような単独のカテゴリ名としても使う |
| Elixir/Flask/Potion of the Tiger・Rabbit・Fox・Lion（ステータス強化秘薬） | 力の秘薬／敏捷の秘薬／知能の秘薬／体力の秘薬（Flaskは頭に「強力な」、`Potion of Tiger (D)`等の等級付きは「力の秘薬 (D)」のように末尾に等級を残す） | `PROPITEM_TXT_007180〜007326`（Elixir/Flask）および`PROPITEM_TXT_133794〜133816`（Potion、D/C/B/A/A+の5段階）準拠。動物名は直訳せず、付与される効果（STR/DEX/INT/STA）で意訳する。同様に`Elixir of Stone`→防御の秘薬、`Elixir of Anti-Magic`→抵抗の秘薬、`Elixir of the Sorcerer`→魔法攻撃力増幅の秘薬など、Items.csvのElixir/Flask/Potion系は一貫して効果ベースの意訳。2026-07-29にユーザー指摘で発覚した表記揺れ（`PROPITEM_TXT_726136`等のパッケージ説明文で「虎のフラスコ」等の直訳、および`PROPITEM_TXT_133794`等の「虎の秘薬」等の直訳）はユーザー指示によりいずれも効果ベース表記に統一済み |
| Concoction of Accuracy/Evasion/Swiftness（`PROPITEM_TXT_133818〜133834`、D/C/B/A/A+の5段階） | 命中の秘薬／回避の秘薬／攻撃速度上昇の秘薬 | `Potion of Accuracy`（命中の秘薬）・`Elixir of Evasion`（回避の秘薬）・`Potion of Swiftness`（攻撃速度上昇の秘薬）と同じ効果ベース表記に統一。`Concoction of Swiftness`は元々「敏捷の秘薬」（DEXの意）と誤訳されていたが、実際の効果は攻撃速度上昇のため2026-07-29にユーザー指摘で修正済み |
| Concoction of Clarity/Recklessness/Bleeding（`PROPITEM_TXT_133836〜133852`、D/C/B/A/A+の5段階） | 詠唱の秘薬／するどさの秘薬／クリティカルダメージ追加の秘薬 | `Potion of Clarity`（詠唱の秘薬）・`Potion of Recklessness`（するどさの秘薬）・`Elixir of Profuse Bleeding`（クリティカルダメージ追加の秘薬）と同じ表記に統一（2026-07-29、ユーザー指示）。動物名シリーズ（力/敏捷/知能/体力）とは別に、こちらは元の単語（Clarity=明晰、Recklessness=無謀、Bleeding=出血）の直訳ではなく既存の対応アイテム名を踏襲する |
| Concoction of Swift Footsteps/HP Recovery/MP Recovery/FP Recovery（`PROPITEM_TXT_133854〜133876`、D/C/B/A/A+の5段階） | 跳躍の秘薬／HP回復量上昇の秘薬／MP回復量上昇の秘薬／FP回復量上昇の秘薬 | 2026-07-29、ユーザーが直接修正。上記のConcoction系と同じく効果ベースの意訳（Footsteps→跳躍＝ジャンプ力上昇、HP/MP/FP Recovery→対応する回復量上昇）で、末尾に(D)〜(A+)の等級を残す |
| Casting Speed（%上昇バフ・カード） | 詠唱速度 | `PROPITEM_TXT_004373`等。「Attack Speed」→「攻撃速度」と同じ言葉遣い |
| Casting Time（%増減の秘薬・効果文） | 魔法キャスティング時間 | `PROPITEM_TXT_007179`等。「詠唱時間」ではなく、既存の古いアイテムに合わせて必ず「魔法キャスティング時間」を使う（2026-07-29、ユーザー指示で確定。「詠唱速度」と語が異なる点に注意 — 同じCasting系でも「Speed」は詠唱速度、「Time」は魔法キャスティング時間で使い分ける） |

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

## イベントコスチューム/セット名（`Items.csv` 900000番台のLucky Box系装備、`PROPITEM_TXT_902xxx`で確認）

`900000`番台にはイベント限定コスチューム（Hat/Suit/Shoes/Hands等の各パーツとSet名）が大量に存在し、同じシリーズ名が1つのセット内で十数回繰り返される。`EquipSets.csv`側にも同名シリーズが追加される可能性があるため、翻訳前に必ずこの表と`Items.csv`内の既存訳を確認すること。2026-07-28時点で`PROPITEM_TXT_902xxx`の未訳分翻訳時に確認した語幹。

| English（シリーズ名） | 日本語 | 備考 |
| --- | --- | --- |
| Sewn Demon | 縫い目の悪魔 | |
| Spellbat | スペルバット | |
| Muran | ムラン | |
| Thanksgiving 2025 | 感謝祭2025 | 音訳「サンクスギビング」ではなく意訳「感謝祭」を使う年度あり（`Thanksgiving 2023`は「サンクスギビング」表記のため年度によって表記揺れがある。新規追加時は前後の既存キーに合わせる） |
| 2025 Christmas | 2025クリスマス | |
| Snow Masquerade | 雪の仮面舞踏会 | |
| Onmyoji 2026 | 陰陽師2026 | |
| Noble Jockey Red | ノーブルジョッキーレッド | |
| Button Mark | ボタンマーク | |
| Heart Punk | ハートパンク | |
| Oni-Style Kimono | 鬼柄着物 | |
| Floating Oni（ペット） | 浮き鬼 | `PROPITEM_TXT_122080`等に準拠 |
| FWC Golden {武器/防具シリーズ名} | FWCゴールデン・{語幹}{部位名}（スペースは一切入れず、「ゴールデン」の直後にのみ中点） | 年表記なしの`PROPITEM_TXT_120820〜120924`（90件）と`PROPITEM_TXT_724627〜724700`（74件）、計164件。元々スペースの有無が一件ごとにバラバラだったため、2026-07-29にユーザー指示で「FWC Golden 」を含む行（`^PROPITEM_TXT_[0-9]+,FWC Golden `）のみを対象に、余分な半角スペースを全て除去し「ゴールデン」の直後に中点(・)を追加して完全統一。`PROPITEM_TXT_155577〜155590`（FWC 2025 Golden Death Messenger's系）は元から同じ中点表記済みで対象外。`PROPITEM_TXT_155591`（FWC 2025 Golden Tiger）は「Golden Tiger」で1つの固有名詞（マウント名）のため中点なしのまま。`PROPITEM_TXT_015276〜015290`（FWC 2011）は「FWC1位記念〜」という別の意訳のため対象外。`PROPITEM_TXT_900000〜900009`（2025 FWC Golden Lusaka's Crystal〜）は英語未訳のまま残っており別問題（要翻訳） |
| 2026 FWC Golden {武器/防具シリーズ名} | 2026 FWCゴールデン・{語幹}（武器・防具とも「2026FWC」の直後に「ゴールデン・」、スペースなし。防具は語幹の後ろに部位名を直接続ける） | `PROPITEM_TXT_155829〜155903`（75件）。「ゴールデン」と語幹がカタカナで連続し読みにくかったため、2026-07-29にユーザー指示で「ゴールデン」の直後にのみ中点(・)を追加して統一（この時点では武器サブシリーズの末尾に「 アルティメット」を残し、「2026 FWC」と「ゴールデン」の間にスペースもあった）。その後同日、ユーザーが武器サブシリーズ`PROPITEM_TXT_155829〜155839`（11件）について「Ultimate」を訳語なし（削除）とする方針に変更し、末尾の「アルティメット」削除と「2026 FWC」→「2026 FWC」間のスペース除去を手動で実施（結果、防具サブシリーズと同じ「2026 FWCゴールデン・{語幹}」の形に統一）。他言語（仏語「ultime」、西語「Definitiva」で意訳、繁体中文は創作訳、他言語の大半はこのアイテム自体未翻訳）を確認した上での判断。語幹内の「Maw of Judgement」→「マウ・オブ・ジャッジメント」等、既存の中点はそのまま |
| 2025 FWC Flame {武器/防具シリーズ名} | 2025 FWCフレイム・{語幹}（Helmet等の部位名の前にはスペースを残す：例「2025 FWCフレイム・ビラリ ヘルメット(F)」。武器は語幹の後に格助詞「の」で続ける：例「2025 FWCフレイム・ルサカの剣」。Costume Setは部位名前にスペースを入れず語幹に直接続ける：例「2025FWCフレイム・ビラリコスチュームセット(F)」） | `PROPITEM_TXT_134853〜134886`。2026-07-29、ユーザーが手動で「フレイム」の直後に中点を追加。`PROPITEM_TXT_134869〜134872`（Costume Set系4件）も同日ユーザー指示で中点を追加し全件対応済み |
| 2025 FWC Golden Lusaka's Crystal {武器名} | 2025 FWCゴールデン・ルサカのクリスタル{武器名}（Heavyは「ヘビークリスタル」） | `PROPITEM_TXT_900000〜900009`。2026-07-29時点で英語未訳のまま残っていたのをユーザー指示で翻訳。年表記なしの同名シリーズ`PROPITEM_TXT_724691〜724700`（FWCゴールデン・ルサカのクリスタル〜）の表記にそのまま準拠 |

## モンスター名（`Movers.csv`定訳、`Achievements.csv`のKILL系実績で使用）

`Achievements.csv`の`ACHIEVEMENT_KILL_*`系実績（討伐数実績）の名前は`Movers.csv`の英語名と完全一致するため、翻訳時は`Movers.csv`の既存訳をそのまま流用すること。以下は2026-07-28時点で`Achievements.csv`の未訳分に対応するために採取したモンスター名。

| English | 日本語（Movers.csv準拠） | 備考 |
| --- | --- | --- |
| Dreadfin | ドレッドフィン | |
| Dreadscale | ドレッドスケイル | |
| Luminfin | ルミンフィン | |
| [Shade Lieutenant] Kriton | [シェードの幹部] クリトン | |
| Hundur Sharpfoot | ワークウルフ | |
| Samoset | ライカンガード | |
| Kyouchish | ライカンセンチネル | |
| Kanonicus | ライカンアーチャー | |
| Mage Redcloud | ライカンソーサラー | |
| Taiaha | ライカンウォーリアー | |
| Hellhound | スケルトンジャッカル | |
| Chief Keokuk | ライカンバルガ | |
| [God of Death] Demonic Ankou | [死神] 魔の神獣ベヒモス | |
| Ankou | 神獣ベヒモス | `Map.csv`「Ankou's Asylum」は「ベヒモス神殿」 |
| Blazing Ankou | 炎の神獣ベヒモス | |
| Demonic Ankou | 魔の神獣ベヒモス | |
| Blossom | フロミー | 直訳ではない既存訳（Movers.csv準拠） |
| Oldroot | オールドルート | |
| Minimusha | ミニムシュ | |
| Lady Bloom | レディブルーム | |
| Mushbro | ラプラ | 直訳ではない既存訳（Movers.csv準拠） |
| Nightmyst | ナイトミスト | |
| [Queen of Thorns] Entaness | クイーンエンプティネス | |

### 表記揺れ（備考・一括修正はしない）

`Movers.csv`内で同一英語名に対し複数の日本語訳が混在している例（発見時点の記録のみ。統一は別途ユーザー指示のもとで対応）：

- `Santa`：「サンタクロース」/「サンタ」
- `Blue/Yellow/Red/Purple/Pink/Black Flying Sheep`：「色+空飛ぶ羊」と「色+フライングシープ」の2系統が混在
- `Cheirang`／`Mawrang`：表記自体は揺れなしだが重複キーあり（参考情報）

