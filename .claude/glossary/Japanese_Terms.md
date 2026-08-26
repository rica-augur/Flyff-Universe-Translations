# 日本語 用語集（単語・定訳集）

このファイルは Claude Code の作業補助用ファイルであり、リポジトリ本体の翻訳対象ファイルには含まれません。

## 使い方

1. `Japanese/` 配下のファイルを翻訳・修正する前に、対象の英単語がこの表に存在するか確認する。
2. 存在する場合は、原則としてここに記載された訳語に合わせる。
3. まだ載っていない頻出語句（ゲーム内の共通UI語句、システム名、ステータス名など）を新しく訳した場合は、この表に追記する。
4. 表記揺れ（同じ英単語に対して複数の訳語が既存ファイル内に混在している）を見つけた場合は「備考」欄に記録する。表記揺れの統一自体は既存翻訳の修正になるため、別途ユーザーの指示・PRで対応すること（この用語集への記録だけで既存ファイルを一括置換しない）。

## 全般的な表記ルール

- **数字は半角（1,2,3…）を使う。全角（１，２，３…）は使わない。** ただし、会話文・クエスト説明文等の地の文中で全角数字が使われている既存箇所は多数あり、これは長年の表記揺れとして広く残っているため、地の文単体では無理に一括修正しない。一方、**「名称＋連番」「N%」のようにパターン化された同一シリーズ内で一部だけ全角になっている場合**（例：`Achievements.csv`の`〇〇 Slayer 1〜4`系実績名で一部だけ「１２３４」、`Items.csv`の`Alien Octopus N% 〇〇 Set`系アイテム名で一部だけ「８６４２」）はコピペミスによる表記揺れの可能性が高く、同シリーズの他エントリに合わせて半角に統一する（2026-07-31、`ProductionRecipes.csv`の`Trimmed 〇〇2`系9件・`Controls.csv`のSt Morning表記統一に伴うユーザー指示で確認・一般化）。
- **「St Morning」「Saint Morning」の複合語表記にスペースを入れない。** 例：「セント モーニング シャーレット」ではなく「セイントモーニングシャーレット」。`Controls.csv`の`PROPCTRL_TXT_000201`,`000426`,`000427`で発見（2026-07-31、Copilotレビュー指摘・ユーザー確認）。詳細は下記「Saint Morning」の項を参照。

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
|Saint Morning（地名） | セイントモーニング | 複合語中でもスペースを入れない（「セイント モーニング」ではなく「セイントモーニング」） |
|St Morning（地名） | セイントモーニング | 同上。`Controls.csv`の`PROPCTRL_TXT_000201`（St Morning Chariot）,`000426`,`000427`（St Morning Rock Arch 2/3）が「セント モーニング」（スペース入り・「イ」抜け）になっていたため2026-07-31に修正 |
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
| Ultimate Weapon / Ultimate Accessory（装備の等級名） | アルティマ武器 / アルティマアクセサリー | `PROPITEM_TXT_122501`等に準拠。同じ「Ultimate」でも「Scroll of Ultimate Bonus」等のバフ・巻物文脈では音訳「アルティメット」を使う（例：アルティメットボーナスの巻物）。等級名としての武器・アクセサリーか、バフ効果名かで訳し分ける。武器名末尾の"〇〇 Ultimate"（強化版武器、例：`PROPITEM_TXT_913787〜913797`）は「〇〇・アルティマ」（中点＋アルティマ、スペース区切りの「アルティメット」ではない）に統一（2026-07-29、ユーザー指示で修正） |
| Lunar（Lunar New Year文脈） | 旧正月 | `PROPITEM_TXT_200302`等に準拠。「Lunar New Year Coupon」等はそのまま「旧正月」を使い、音訳「ルナー」にしない |
| Trans（ペット変身オーブ、`PROPITEM_TXT_006094`等の`~ Trans`） | オーブ | 例：「Aibatt Trans」→「アイバット・オーブ」。「Trans Random Box」のような単独のカテゴリ名としても使う |
| Elixir/Flask/Potion of the Tiger・Rabbit・Fox・Lion（ステータス強化秘薬） | 力の秘薬／敏捷の秘薬／知能の秘薬／体力の秘薬（Flaskは頭に「強力な」、`Potion of Tiger (D)`等の等級付きは「力の秘薬 (D)」のように末尾に等級を残す） | `PROPITEM_TXT_007180〜007326`（Elixir/Flask）および`PROPITEM_TXT_133794〜133816`（Potion、D/C/B/A/A+の5段階）準拠。動物名は直訳せず、付与される効果（STR/DEX/INT/STA）で意訳する。同様に`Elixir of Stone`→防御の秘薬、`Elixir of Anti-Magic`→抵抗の秘薬、`Elixir of the Sorcerer`→魔法攻撃力増幅の秘薬など、Items.csvのElixir/Flask/Potion系は一貫して効果ベースの意訳。2026-07-29にユーザー指摘で発覚した表記揺れ（`PROPITEM_TXT_726136`等のパッケージ説明文で「虎のフラスコ」等の直訳、および`PROPITEM_TXT_133794`等の「虎の秘薬」等の直訳）はユーザー指示によりいずれも効果ベース表記に統一済み |
| Concoction of Accuracy/Evasion/Swiftness（`PROPITEM_TXT_133818〜133834`、D/C/B/A/A+の5段階） | 命中の秘薬／回避の秘薬／攻撃速度上昇の秘薬 | `Potion of Accuracy`（命中の秘薬）・`Elixir of Evasion`（回避の秘薬）・`Potion of Swiftness`（攻撃速度上昇の秘薬）と同じ効果ベース表記に統一。`Concoction of Swiftness`は元々「敏捷の秘薬」（DEXの意）と誤訳されていたが、実際の効果は攻撃速度上昇のため2026-07-29にユーザー指摘で修正済み |
| Concoction of Clarity/Recklessness/Bleeding（`PROPITEM_TXT_133836〜133852`、D/C/B/A/A+の5段階） | 詠唱の秘薬／するどさの秘薬／クリティカルダメージ追加の秘薬 | `Potion of Clarity`（詠唱の秘薬）・`Potion of Recklessness`（するどさの秘薬）・`Elixir of Profuse Bleeding`（クリティカルダメージ追加の秘薬）と同じ表記に統一（2026-07-29、ユーザー指示）。動物名シリーズ（力/敏捷/知能/体力）とは別に、こちらは元の単語（Clarity=明晰、Recklessness=無謀、Bleeding=出血）の直訳ではなく既存の対応アイテム名を踏襲する |
| Concoction of Swift Footsteps/HP Recovery/MP Recovery/FP Recovery（`PROPITEM_TXT_133854〜133876`、D/C/B/A/A+の5段階） | 跳躍の秘薬／HP回復量上昇の秘薬／MP回復量上昇の秘薬／FP回復量上昇の秘薬 | 2026-07-29、ユーザーが直接修正。上記のConcoction系と同じく効果ベースの意訳（Footsteps→跳躍＝ジャンプ力上昇、HP/MP/FP Recovery→対応する回復量上昇）で、末尾に(D)〜(A+)の等級を残す |
| Casting Speed（%上昇バフ・カード） | 詠唱速度 | `PROPITEM_TXT_004373`等。「Attack Speed」→「攻撃速度」と同じ言葉遣い |
| Casting Time（%増減の秘薬・効果文） | 魔法キャスティング時間 | `PROPITEM_TXT_007179`等。「詠唱時間」ではなく、既存の古いアイテムに合わせて必ず「魔法キャスティング時間」を使う（2026-07-29、ユーザー指示で確定。「詠唱速度」と語が異なる点に注意 — 同じCasting系でも「Speed」は詠唱速度、「Time」は魔法キャスティング時間で使い分ける） |
| Set（アイテム名末尾の"〇〇 Set"） | 〇〇セット（英語の語順通り、訳した/音訳したシリーズ名の直後に「セット」を置く。「セット〇〇」のように前置しない） | `PROPITEM_TXT_828037`Mizu Yukata Set→「みず浴衣セット」、`PROPITEM_TXT_828073`Yukata 2025 Set (F)→「浴衣2025セット(F)」、`PROPITEM_TXT_828348`Set of the Rising Moon→「ライジングムーンセット」等に準拠（2026-07-29確認）。性別表記(M)/(F)は英語と同じくセットの後ろに残す |
| Rice Cake Soup（新年イベントのバフ飲食物、`PROPITEM_TXT_144155〜144162`＝2025年版、`PROPITEM_TXT_135044〜135048`＝2026年版） | お雑煮（{色}Rice Cake Soup→{色}のお雑煮、例：Red→赤いお雑煮。効果文は「このお雑煮は、30分間{ステータス}+25を付与します。」） | 直訳「餅スープ」ではなく日本の正月料理「お雑煮」を採用。ただし`PROPITEM_TXT_200294〜200300`（無印Red/Green/Blue/Yellow Rice Cake Soup）は既存訳が「赤餅スープ」等の直訳のため据え置き（別シリーズ扱い、2026-07-29確認） |
| Mr.Kang（NPC名） | Mr.カン | `Characters.csv`の`CHARACTER_INC_100107`（[Event] Mr.Kang→[イベント]Mr.カン）に準拠 |
| New Year Pass（`PROPITEM_TXT_144163〜144164`＝2025年版「正月パス」、`PROPITEM_TXT_135085〜135086`＝2026年版「新年パス」） | 年度により表記が異なる（2025は「正月パス」、2026以降は「新年パス」）。新規追加時は該当年度の既存訳（同じアイテム名内の表記）に合わせる | 2026-07-29確認。統一はせず既存表記をそのまま踏襲 |
| Entaness（`[Queen of Thorns] Entaness`のボスモンスター名） | 単独表記の場合は音訳「エンタネス」、`[Queen of Thorns] Entaness`という完全なタイトル表記の場合は「[棘の女王] エンタネス」 | 旧創作訳「クイーンエンプティネス」（`Movers.csv`の`PROPMOVER_TXT_002070`、`Achievements.csv`のKILL_DREAMQEEN01系6件）は2026-08-12にユーザー指示で「[棘の女王] エンタネス」に置き換え。`Quests.csv`の`PROPQUEST_INC_155091`は元々「[茨の女王]エンタネス」（`茨`表記、ブラケット直後スペースなし）だったが、同時にMovers.csvの新表記（`棘`）に合わせて「[棘の女王]エンタネス」に修正済み（漢字のみ統一、ブラケット後のスペース有無はファイルごとの既存書式を維持） |
| Queen of Thorns（単独、称号としての言及） | 棘の女王 | 上記Entanessの項参照。`Items.csv`の`PROPITEM_TXT_913773`で確認。旧表記「茨の女王」から2026-08-12に統一 |
| Tigar（`Movers.csv`の`PROPMOVER_TXT_110118〜110142`系ボスモンスター種族名。所有格・複合語も含む） | タイガー | `Achievements.csv`の`ACHIEVEMENT_KILL_TIGAR_NAME`や`Movers.csv`のArmored Tigar/Small/Captain/Lord Tigar系で「ティーガー」表記が混在していたため、2026-08-12にユーザー指示で「タイガー」に統一。`Items.csv`（`PROPITEM_TXT_010466〜010471`）、`Quests.csv`（`PROPQUEST_INC_130028`,`130029`,`130036`,`130038`,`130039`,`130041`、うち`130028`/`130029`は「タイガール」という誤記も修正）の「ティーガー」表記も同時に修正済み |
| Meral（`Movers.csv`の`PROPMOVER_TXT_110124〜110144`系ボスモンスター種族名。所有格・複合語も含む） | メレー | `Movers.csv`内で「メラル」（Giant/Violet/[Event] Meral）表記が混在していたため、2026-08-12にユーザー指示で「メレー」に統一。`Achievements.csv`（`ACHIEVEMENT_KILL_MERAL_LVL1〜5`）、`Quests.csv`（`PROPQUEST_INC_130040`,`130044`,`130047`）、`RequestBoxQuests.csv`（`PROPQUEST_REQUESTBOX_INC_020029`,`020038`）、`Items.csv`（`PROPITEM_TXT_010047`,`160001`,`160005`）の「メラル」表記も同時に修正済み |
| Okean（`Movers.csv`の`PROPMOVER_TXT_110115〜110141`系ボスモンスター種族名。所有格・複合語も含む） | オケアノス | `Movers.csv`内で「オケアン」（Giant/Violet Okean）表記が混在していたため、2026-08-12にユーザー指示で「オケアノス」に統一。`Items.csv`（`PROPITEM_TXT_010041`,`160018〜160019`）、`PatrolDestinations.csv`（`PATROL_DESTINATION_000009`）、`Quests.csv`（`PROPQUEST_INC_130072`,`130075`,`130084`）、`RequestBoxQuests.csv`（`PROPQUEST_REQUESTBOX_INC_020034`,`020043`）の「オケアン」表記も同時に修正済み。`Achievements.csv`の`Okean`とは別に`Mystica`という種族が存在するので混同しないこと |
| Ankou（ボスモンスター名。"Ankou's ~"の所有格・複合語も含む） | ベヒモス | `Movers.csv`の`PROPMOVER_TXT_500055〜500061`等、`Map.csv`の`Ankou's Asylum`→「ベヒモス神殿」、`Items.csv`の`Ankou's Scale`→「ベヒモスの鱗」等、10ファイル以上で一貫して使われる確立訳。音訳「アンコウ」（日本語の「鮟鱇」と偶然同音）にしないこと。`UI.csv`の`UI_TOOLTIP_DST_ANKOUHARVEST`（Ankou's Harvest）が誤って音訳「アンコウの収穫」になっていたため2026-07-31にユーザー指摘で「ベヒモスの収穫」に修正 |
| Euphrasia（地名、Entaness武器セットの説明文に登場） | ユーフラシア | `PROPITEM_TXT_913773`。他ファイルに先例なし、音訳で新規採用（2026-07-29） |
| Drifter/Maiden/Reaver/Mystica/Anae/Rifter（`[Forgotten]`系モンスター種族名、`Movers.csv`の`PROPMOVER_TXT_505001〜505030`準拠） | ドリフター／メイデン／リーバー／ミスティカ／アナエ／リフター（接頭語`[Forgotten]`は「[帰らぬ冒険者]」） | `Items.csv`の`PROPITEM_TXT_913758〜913769`（Spirit Shard系アイテムの説明文で種族名のみ再利用、`[Forgotten]`の接頭語は付けない）で確認（2026-07-29）。`Mystica`は`Achievements.csv`の`Okean`とは別モンスター（Okeanは「オケアノス」）。`[Forgotten]`接頭語は当初「[忘却の]」→2026-08-12に「[忘れられし]」→同日中に再度ユーザー指示で「[帰らぬ冒険者]」に変更（`Movers.csv`の`PROPMOVER_TXT_505001〜505030`全30件を修正済み）。`Items.csv`の`Ghost of the Forgotten ~`系（`PROPITEM_TXT_827778〜827790`＝「忘却の幽霊〜」）は別シリーズのためこの変更の対象外 |
| Chip/Chips系交換通貨のナンバリング（`Kalgas Chip`→`Kalgas Chip 2`、`Yellow/Red Chips`→`Yellow/Red Chips 2`等） | 既存の音訳（カルガスチップ／イエローチップ／レッドチップ、単数形カタカナ）の直後に半角スペースなしで数字を付与（カルガスチップ2／イエローチップ2／レッドチップ2） | `PROPITEM_TXT_913716`,`913754`,`913756`で確認（2026-07-29）。`Waforu`は既存訳に「ワフォル」（`PROPITEM_TXT_131907`等）と「ワポール」（`PROPITEM_TXT_008903`,`1902586`等）の表記揺れが既にあり、新規追加時は直前の類似文（同一パターンの既存文）に合わせる |
| Kebaras 2（新ダンジョン名、`Kebaras`の続編） | ケバラス2（「ケバラス」との間にスペースなし） | `PROPITEM_TXT_1902589〜1902626`に先例あり。チケット名は「ケバラス2 {期間}券」のように数字とチケット期間の間にスペースを入れる（`PROPITEM_TXT_913750`,`913752`、番号の連続による可読性低下を避けるため） |
| Update Pass（バージョン番号付き、例：`1.5 Update Pass`→「1.5アップデートパス」） | {バージョン番号}アップデートパス／{バージョン番号}アップデートラッキーボックス（バージョン番号とアップデートの間にスペースなし） | `PROPITEM_TXT_135002〜135009`（1.5系）に準拠して`PROPITEM_TXT_913798〜913800`（1.5.5系）を翻訳（2026-07-29） |
| Life Mastery系スキル名（`PROPITEM_TXT_830003〜830082`のバッグ名等） | Herb Gathering→薬草採集／Wood Cutting→伐採／Mining→採掘／Fishing→釣り／Alchemy→錬金術／Cooking→料理／Carpentry→木工／Smithing→鍛冶 | `UI.csv`の`UI_LIFE_MASTERY_*_SUCCESS`系（`UI_LIFE_MASTERY_HERBGATHERING_SUCCESS`等）に準拠。`{スキル名}バッグ({N}スロット)`／「{スキル名}で入手したアイテムを最大{N}個まで収納できるバッグ。」の定型文で2026-07-29に翻訳 |
| Shop Advertisement（{色}） | ショップ広告({色}、括弧内は英語色名のカタカナ) | `PROPITEM_TXT_201073〜201080`,`155623〜155626`等に準拠。説明文は「この巻物を使用すると、個人商店またはベンダーショップがショップ検索結果の上部に{色}の飾りつきで表示されます。ショップを開くと消費され、閉じると効果が消えます。」で統一 |
| Jewel Conversion（`Lower Scroll of Jewel Conversion`/`Scroll of Jewel Conversion`） | 下級ジュエル変換の巻物／ジュエル変換の巻物 | `PROPITEM_TXT_902535`のパッケージ説明文に先例あり。`PROPITEM_TXT_750000〜750018`翻訳時に確認（2026-07-29） |
| 宝石名（ジュエル合成システム共通） | Topaz→トパーズ／Ruby→ルビー／Sapphire→サファイア／Emerald→エメラルド／Diamond→ダイヤモンド／Amethyst→アメジスト／Onyx→オニキス | `Items.csv`内の既存音訳に準拠（`PROPITEM_TXT_008052〜008060`等） |
| Herneos（ダンジョン/エリア名） | ヘルネオス | `Map.csv`の`PROPMAX_TXT_200023`、`QuestDestinations.csv`に準拠 |
| Livi（NPC名、ライフスキル関連） | リヴィ | `Characters.csv`の`CHARACTER_INC_100104`（[Life Master] Livi→[ライフマスター]リヴィ）に準拠 |
| Turkeylicious（感謝祭コスチュームシリーズ） | ターキーリシャス | `PROPITEM_TXT_801367〜801370`,`726305〜726457`に準拠 |
| Charlie Hunter（コスチューム/武器シリーズ） | チャーリーハンター | `PROPITEM_TXT_726075〜726124`に準拠 |
| Persian Warrior（コスチュームシリーズ） | ペルシャの戦士 | `PROPITEM_TXT_726037〜726111`に準拠。関連の乗り物「Persian Magic Carpet」は同シリーズだが音訳「ペルシアンマジックカーペット」（コスチュームの意訳とは表記を分ける、2026-07-29） |
| 単独の英字/記号アイテム（例：`PROPITEM_TXT_206421〜206425`の I/♥/Y/O/U、`PROPITEM_TXT_723376〜723378`の2/N/D、`OST`,`PSP`等の略語アイテム名） | 翻訳せず英語のまま残す | 「I♥YOU」「2ND」等をコレクションで綴らせるイベント文字アイテムのため、1文字単位の翻訳は不可能。既存の翻訳済み周辺行も同様に英語のまま据え置かれている（2026-07-29確認）。`PROPITEM_TXT_134598`の`#ERROR!`は英語原文自体が壊れているソース側の不具合のため対象外 |

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
| Zoracet | ゾラセト | 当初「ゾラセット」（Items.csvの`PROPITEM_TXT_155400〜155403`）としていたが、`EquipSets.csv`のSet表記で「ゾラセットセット」と「セット」が重複し語呂が悪いとCopilotレビューで指摘されたため、2026-08-04にユーザー指示で促音を落とした「ゾラセト」に統一（Items.csvの防具4件・EquipSets.csvのSet表記1件とも変更済み、いずれも当時PR未送信のため後方互換の問題なし） |
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
| Menhera Kei（コスチュームシリーズ） | ヤンデレ系 | `PROPITEM_TXT_905311`等に準拠。メンヘラ系ではない点に注意（2026-07-29、904883の誤訳をこの表記に修正済み） |

## ペット/マウント名（`PROPITEM_TXT_900xxx〜906xxx`、2026-07-29の未訳分翻訳時に確認）

| English | 日本語 | 備考 |
| --- | --- | --- |
| Breezy | ブリージー | `PROPITEM_TXT_901035`等 |
| Pawsy | パウジー | `PROPITEM_TXT_900444`等（Pawshとは別のペット） |
| Pawsh | ポーシュ | `PROPITEM_TXT_901491`等 |
| Flumos | フルモス | `PROPITEM_TXT_900588`等 |
| Marshall | マーシャル | `PROPITEM_TXT_901582`等 |
| Strawy Jack | ストロージャック | `PROPITEM_TXT_901906`等 |
| Fawkes（セレスティアルフェニックスのマウント） | フォークス | `PROPITEM_TXT_904077`等 |
| Runewhale | ルーンホエール | `PROPITEM_TXT_905851`等 |
| Pocket Shinobi | ポケット忍者 | `PROPITEM_TXT_906043`等。Shinobiは音訳せず「忍者」表記 |
| Thornhart | ソーンハート | `PROPITEM_TXT_900919`等（Forest Spiritセットのマウント） |
| Cyberneon（3rd Anniversary武器シリーズ） | サイバーネオン | `PROPITEM_TXT_900317`等 |

## 部位名の前の中点ルール（2026-07-29、ユーザー指示で追加統一）

「{接頭語}{語幹}{部位名}」がカタカナで連続し読みにくい防具/武器シリーズは、部位名（Helmet/Suit/Gauntlets/Boots や武器種名 Sword/Axe等）の直前にのみ中点(・)を入れる。接頭語と語幹の間のスペース・中点の有無は既存表記を変更しない。

| 対象範囲 | Before → After 例 |
| --- | --- |
| `PROPITEM_TXT_161048〜161063`（PvP 防具、16件） | PvPウスタメルヘルメット → PvPウスタメル・ヘルメット（「PvP」は短く読みやすいため接頭語の直後には中点を入れない） |
| `PROPITEM_TXT_161000〜161047`（Primordial 防具、48件） | プリモーディアルランティエル・ヘルメット → プリモーディアル・ランティエル・ヘルメット（「プリモーディアル{語幹}」がカタカナで長く読みにくいため、2026-08-04にユーザー指示で「プリモーディアル」の直後にも中点を追加。`EquipSets.csv`の`PROPITEMETC_INC_000426〜000441`（Primordial Set系16件）で先に同じ中点追加が行われており、それに揃える形で対応。以前は「プリモーディアルの後には中点なし」だったが本件で上書き） |
| `PROPITEM_TXT_900713〜900831`（Obsidian Flame 武器、104件、Weapon Setは対象外） | オブシディアンフレイムオレンジソード → オブシディアンフレイムオレンジ・ソード |
| `PROPITEM_TXT_905525〜905573`（Japanese Uniform、49件） | 表記バラバラ（日本軍制服ブラックスーツ／グリーン制服スーツ／パープルスーツ等）だったものを「和風制服{色}・{部位}」に統一。Backpack7件（902xxx翻訳時に「和風制服{色}バックパック」で先に訳出済み）にも中点を追加 |
| FWC Golden {武器/防具シリーズ名} | FWCゴールデン・{語幹}{部位名}（スペースは一切入れず、「ゴールデン」の直後にのみ中点） | 年表記なしの`PROPITEM_TXT_120820〜120924`（90件）と`PROPITEM_TXT_724627〜724700`（74件）、計164件。元々スペースの有無が一件ごとにバラバラだったため、2026-07-29にユーザー指示で「FWC Golden 」を含む行（`^PROPITEM_TXT_[0-9]+,FWC Golden `）のみを対象に、余分な半角スペースを全て除去し「ゴールデン」の直後に中点(・)を追加して完全統一。`PROPITEM_TXT_155577〜155590`（FWC 2025 Golden Death Messenger's系）は元から同じ中点表記済みで対象外。`PROPITEM_TXT_155591`（FWC 2025 Golden Tiger）は「Golden Tiger」で1つの固有名詞（マウント名）のため中点なしのまま。`PROPITEM_TXT_015276〜015290`（FWC 2011）は「FWC1位記念〜」という別の意訳のため対象外。`PROPITEM_TXT_900000〜900009`（2025 FWC Golden Lusaka's Crystal〜）は英語未訳のまま残っており別問題（要翻訳） |
| 2026 FWC Golden {武器/防具シリーズ名} | 2026 FWCゴールデン・{語幹}（武器・防具とも「2026FWC」の直後に「ゴールデン・」、スペースなし。防具は語幹の後ろに部位名を直接続ける） | `PROPITEM_TXT_155829〜155903`（75件）。「ゴールデン」と語幹がカタカナで連続し読みにくかったため、2026-07-29にユーザー指示で「ゴールデン」の直後にのみ中点(・)を追加して統一（この時点では武器サブシリーズの末尾に「 アルティメット」を残し、「2026 FWC」と「ゴールデン」の間にスペースもあった）。その後同日、ユーザーが武器サブシリーズ`PROPITEM_TXT_155829〜155839`（11件）について「Ultimate」を訳語なし（削除）とする方針に変更し、末尾の「アルティメット」削除と「2026 FWC」→「2026 FWC」間のスペース除去を手動で実施（結果、防具サブシリーズと同じ「2026 FWCゴールデン・{語幹}」の形に統一）。他言語（仏語「ultime」、西語「Definitiva」で意訳、繁体中文は創作訳、他言語の大半はこのアイテム自体未翻訳）を確認した上での判断。語幹内の「Maw of Judgement」→「マウ・オブ・ジャッジメント」等、既存の中点はそのまま |
| 2025 FWC Flame {武器/防具シリーズ名} | 2025 FWCフレイム・{語幹}（Helmet等の部位名の前にはスペースを残す：例「2025 FWCフレイム・ビラリ ヘルメット(F)」。武器は語幹の後に格助詞「の」で続ける：例「2025 FWCフレイム・ルサカの剣」。Costume Setは部位名前にスペースを入れず語幹に直接続ける：例「2025FWCフレイム・ビラリコスチュームセット(F)」） | `PROPITEM_TXT_134853〜134886`。2026-07-29、ユーザーが手動で「フレイム」の直後に中点を追加。`PROPITEM_TXT_134869〜134872`（Costume Set系4件）も同日ユーザー指示で中点を追加し全件対応済み |
| 2025 FWC Golden Lusaka's Crystal {武器名} | 2025 FWCゴールデン・ルサカのクリスタル{武器名}（Heavyは「ヘビークリスタル」） | `PROPITEM_TXT_900000〜900009`。2026-07-29時点で英語未訳のまま残っていたのをユーザー指示で翻訳。年表記なしの同名シリーズ`PROPITEM_TXT_724691〜724700`（FWCゴールデン・ルサカのクリスタル〜）の表記にそのまま準拠 |
| Archangel White/Black（`PROPITEM_TXT_201043〜201072`、`201057〜201071`、武器パーツ13種×2） | アークエンジェルホワイト・{部位名}／アークエンジェルブラック・{部位名}（部位名の直前のみ中点。「Weapon Set」は中点なし：アークエンジェルホワイトウェポンセット） | 2026-07-29、ユーザー指示で中点追加 |
| Kalgas' Fury（`PROPITEM_TXT_201082〜201114`、武器・防具パーツ、Set/Wings含む） | カルガスフューリー・{部位名}（部位名の直前のみ中点。「Weapon Set」「Set」は中点なし：カルガスフューリーウェポンセット／カルガスフューリーセット(M/F)） | 2026-07-29、ユーザー指示で「カルガスの怒り」（`PROPITEM_TXT_722920`系の旧アイテムの訳に準拠していた表記）から音訳「カルガスフューリー」に変更した上で中点を追加。旧アイテム`PROPITEM_TXT_722920〜722933`（Kalgas' wrath）の「カルガスの怒り」表記はこの変更の対象外（別アイテムのため据え置き） |

## Vendor Shop系ペット名（`Items.csv` 828xxx番台、2026-07-29の未訳分翻訳時に確認）

「{モンスター名} Vendor Shop」＋「This cute {モンスター名} manages a Personal Shop for you!...」の定型ペア（`PROPITEM_TXT_134665〜134852`等に先例あり）。タイトルは「{モンスター名（Movers.csv準拠のカタカナ音訳）}の売り子」、説明文は「この可愛い{モンスター名}は、あなたの代わりに個人商店を開いてくれます。使用後はダブルクリックでショップを閉じることができ、アイテムが戻ってきます。(N日間)」に統一。モンスター名部分は`Movers.csv`の既存訳をそのまま流用する（例：`Captain Cursed Warden`→キャプテン・カースド・ウォーデン、`Lord Drakul`→ロード・ヴァンパイア、`Crystal Demon Lord`→クリスタル・デーモンロード、`Clockworks Butler`→時計ゼンマイのバトラー、`Ghost of the Forgotten Prince`→プリンス・ゴースト）。`PROPITEM_TXT_828038〜828063`で確認。

## Rising Moon（`PROPITEM_TXT_828335〜828348`、2026-07-29に確認）

`Set of the Rising Moon`の説明文（`PROPITEM_TXT_828345/828347`）で先に「ライジングムーンセット」という音訳が使われていたため、他の部位名（Suit/Helmet/Gauntlets/Boots）も同じ音訳に統一。「Setting Sun」「Rising Sun」系の旧防具（`PROPITEM_TXT_012894〜012922`等）は独自の創作名（エビルシェード、ホーリーバブル等）だが、これは別シリーズのため踏襲しない。

## 「〇〇セット」シリーズ名（`Items.csv` 828xxx番台で確認済み、2026-07-29）

`Items.csv`全体には「{シリーズ名} {N}%{色}Set」型のコスチュームセットが非常に多く（機械的に重複排除すると500件以上）存在するため全件の網羅は行っていない。以下は828xxx番台で人手確認済みのシリーズ名のみ。新規シリーズを訳す際は、まず対象範囲内の「(パッケージ説明文などで色指定のない）素のSet」行を探し、そこから正しいシリーズ名を確認すること（色付きの行だけを見て機械的に接頭辞を取り出すと、国コード違い（BR/CN/DE等）や表記ゆれで誤ったシリーズ名になりやすい）。

| English（シリーズ名） | 日本語 | 備考 |
| --- | --- | --- |
| Cyberpunk 2025 | サイバーパンク2025 | 音訳。`PROPITEM_TXT_828026`の説明文で確認。色/%付きは「サイバーパンク2025 2%ブルーセット」のように{シリーズ名} {N}%{色}セットの語順（%の前に半角スペース） |
| Mizu Yukata | みず浴衣 | `PROPITEM_TXT_828037`。色/性別バリエーションのない単一アイテム |
| Yukata 2025 | 浴衣2025 | `PROPITEM_TXT_828064`。色/%バリエーションなし、(M)/(F)のみ |
| Modern Alien | モダンエイリアン | 音訳。`PROPITEM_TXT_828191`の説明文で確認 |
| Easter Rabbit 2025 | イースターラビット2025 | 音訳。`PROPITEM_TXT_828291`の説明文で確認 |
| Rising Moon | ライジングムーン | 音訳。上記参照 |

`PROPITEM_TXT_828183/828188`（Modern Alien 2% Rainbow Set (M)/(F)）と`PROPITEM_TXT_828283/828288`（Easter Rabbit 2025 2% Rainbow Set (M)/(F)）は、本来アイテム名（「モダンエイリアン 2%レインボーセット(M)」等）が入るべき箇所に、隣接する説明文用の「男性/女性キャラクター用の〜」という文言が誤って入っていた（コピペミスと思われる既存の誤訳）。2026-07-29、ユーザー指示で該当4件を正しいアイテム名表記に修正済み。

## モンスター名（`Movers.csv`定訳、`Achievements.csv`のKILL系実績で使用）

**表記の由来について：** `Movers.csv`のモンスター名の多くは、英語名の直訳・音訳ではなく、Flyff（フリフ）の日本国内サービス時代に使われていた**昔の公式和名**を踏襲している（例：`Ankou`→`ベヒモス`、`Meral`→`メレー`、`Tigar`→`タイガー`、`Bang`→`ヴァン`、`Aibatt`→`アイバット`等）。そのため一見すると英語名と対応関係が分かりにくい訳語が多数存在するが、これは誤訳ではなく意図的な踏襲であり、新規に類推・修正しないこと。同じ理由で、英語名をそのままカタカナ音訳すると偶然別の意味の単語と同音になってしまうケース（例：`Ankou`を素直に音訳すると「アンコウ（鮟鱇）」になってしまう）を避ける目的も兼ねている。

`Achievements.csv`の`ACHIEVEMENT_KILL_*`系実績（討伐数実績）の名前は`Movers.csv`の英語名と完全一致するため、翻訳時は`Movers.csv`の既存訳をそのまま流用すること。以下は2026-07-28時点で`Achievements.csv`の未訳分に対応するために採取したモンスター名。

| English | 日本語（Movers.csv準拠） | 備考 |
| --- | --- | --- |
| Dreadfin | ドレッドフィン | |
| Dreadscale | ドレッドスケイル | |
| Luminfin | ルミンフィン | |
| [Shade Lieutenant] Kriton | [シェードの右腕] クリトン | 旧訳「[シェードの幹部]」から2026-08-12にユーザー指示で修正。`Quests.csv`/`QuestDestinations.csv`の地の文で"the Shade's right hand"→「シェードの右腕」と訳されているのに合わせた。`Achievements.csv`（`ACHIEVEMENT_KILL_SHADEKRITON_NAME`,`_LVL1〜5`）も同時に修正済み |
| Hundur Sharpfoot | ワークウルフ | |
| Samoset | ライカンガード | |
| Kyouchish | ライカンセンチネル | |
| Kanonicus | ライカンアーチャー | |
| Mage Redcloud | ライカンソーサラー | |
| Taiaha | ライカンウォーリアー | |
| Hellhound | スケルトンジャッカル | |
| Chief Keokuk | ライカンバルガ | |
| [God of Death] Demonic Ankou（`PROPMOVER_TXT_500057`） | [死神] 魔界の神獣ベヒモス | 旧訳「[死神] 魔の神獣ベヒモス」から2026-08-12にユーザー指示で変更。同名だが無印の`Demonic Ankou`（`PROPMOVER_TXT_500061`、下記）とは訳し分ける（あちらは変更対象外） |
| Ankou | 神獣ベヒモス | `Map.csv`「Ankou's Asylum」は「ベヒモス神殿」 |
| [God of Death] Blazing Ankou（`PROPMOVER_TXT_500056`） | [死神] 烈火の神獣ベヒモス | 旧訳「[死神] 炎の神獣ベヒモス」から2026-08-12にユーザー指示で変更 |
| Demonic Ankou（`PROPMOVER_TXT_500061`、無印） | 魔の神獣ベヒモス | 上記`[God of Death] Demonic Ankou`とは別表記のまま据え置き（2026-08-12確認） |
| Blossom | フロミー | 直訳ではない既存訳（Movers.csv準拠） |
| Oldroot | オールドルート | |
| Minimusha | ミニムシュ | |
| Lady Bloom | レディブルーム | |
| Mushbro | ラプラ | 直訳ではない既存訳（Movers.csv準拠） |
| Nightmyst | ナイトミスト | |
| [Queen of Thorns] Entaness | [棘の女王] エンタネス | 旧創作訳「クイーンエンプティネス」から2026-08-12に変更。詳細は上記「Entaness」の項参照 |

### 表記揺れ（備考・一括修正はしない）

`Movers.csv`内で同一英語名に対し複数の日本語訳が混在している例（発見時点の記録のみ。統一は別途ユーザー指示のもとで対応）：

- `Santa`：「サンタクロース」/「サンタ」
- `Blue/Yellow/Red/Purple/Pink/Black Flying Sheep`：「色+空飛ぶ羊」と「色+フライングシープ」の2系統が混在
- `Cheirang`／`Mawrang`：表記自体は揺れなしだが重複キーあり（参考情報）

## スキル名（`Skills.csv`）

| English | 日本語 | 備考 |
| --- | --- | --- |
| Lightning Strike（`PROPSKILL_TXT_000190`） | ライトニングストライク | 同ファイル内に別スキル`Thunder Strike`（`PROPSKILL_TXT_150381`）が存在し、双方とも旧訳が「サンダーストライク」で重複していたため2026-07-30にユーザーが手修正 |
| Thunder Strike（`PROPSKILL_TXT_150381`） | サンダーストライク | 上記参照。こちらは訳語を変更せず据え置き |

## 地名・拠点名の追加訳（2026-07-30、未翻訳分の一斉確認で対応）

| English | 日本語 | 備考 |
| --- | --- | --- |
| Wandering Shop | 行商 | `TextClient.csv`の`TEXTCLIENT_WANDERING_SHOP_TICKET_FAIL`に先例あり。`MoverMenus.csv`の`MMI_1101`もこれに統一 |
| Sea Shell（`MoverMenus.csv`の`MMI_1080`「Sea Shell Upgrading」） | 貝殻 | `Items.csv`の`PROPITEM_TXT_121662`（単体アイテム名）に準拠。「Sea Shell Upgrading」→「貝殻のアップグレード」。なおイベント限定アイテム`[Event] Red/Yellow/Blue Sea Shell`は別表記「シーシェル」（音訳）のため混同しないこと |
| Northern Flarine | フラリス北広場 | `World.csv`の`WORLD_WDMADRIGAL_WDMADRIGAL_RGN_000008`（地域名としての表記）に準拠。文中で地の文として使う場合は「フラリス北部」表記の先例もある（`Quests.csv`） |
| Dreknir Ridge/Lionrath Falls/Velora Cliffs/Dreknir Forest（`World.csv`のMadrigal新規地名） | ドレクニルの尾根／ライオンラスの滝／ヴェローラの断崖／ドレクニルの森 | 音訳した固有名詞＋地形語の組み合わせ。地形語が「尾根／滝／断崖／森」の場合は間に「の」を入れる（自然な日本語のため）。同じ並びの`Orbalune Port`（オルバルーン港）のみ「の」なしで直接複合させる（「港」は複合語になりやすいため） |

## Eillun村関連の固有名詞（`Dialogs.csv`のNPC_150xxx/155xxx/156xxx、2026-07-30の未訳分一斉翻訳で確認）

| English | 日本語 | 備考 |
| --- | --- | --- |
| Eillun | エルリウン | `Characters.csv`の`[Eillun Guard]`→`[エルリウン衛兵]`、`[Eillun Farmer]`→`[エルリウンの農夫]`に準拠 |
| Lycan(s) | ライカン | `Items.csv`の`PROPITEM_TXT_155017`等に準拠 |
| Myuran(s) | ムラン | `Quests.csv`の`PROPQUEST_INC_150295`（Myurang→ムラン）に準拠。エルリウン村の住民を指す種族名 |
| Ankou's Asylum（守衛の文脈） | ベヒモス神殿 | 既存の`Ankou's Asylum`→`ベヒモス神殿`訳に準拠して「Asylum Guard」を「ベヒモス神殿の守衛」と訳出 |
| Village Chief / Mayor（Huntrang、村長格） | 族長 | `Characters.csv`の`[Village Chief] Huntrang`→`[族長]フンツラン`に準拠。名前を出さない一般的な「mayor of Eillun」の言及もこれに合わせる |
| Guild Siege | ギルドコンバット | 既存訳（`Dialogs.csv`の`NPC_000198`等）に準拠。マネージャー職の略称は「ギルコン」 |
| Waldo（`NPC_150036`のジョーク的言及） | ワルド | 元ネタ（Where's Waldo）を意識し音訳のみ、意訳しない |
| Khajiit（`NPC_150051`） | カジート | 他作品由来のジョーク的言及、定訳の音訳をそのまま採用 |
| "arrow to the knee"ミーム（`NPC_150024`） | 「昔は冒険者だったんだが……膝に矢を受けてしまってな」 | Skyrimの有名な衛兵セリフの日本語ミーム訳をそのまま踏襲 |
| 標準的な「……」（英語`...`のみの行） | …… | `Quests.csv`の`PROPQUEST_INC_110015`に先例あり |
| IDS_Hael_Letter（`Dialogs.csv`の`NPC_100108`） | 翻訳せず据え置き | 未解決のテンプレートID文字列で実際の対話文ではない（`PROPITEM_TXT_134598`の`#ERROR!`と同様、ソース側の不具合のため翻訳対象外） |

## `UI.csv`のGMコマンド文字列（2026-07-30確認）

`UI.csv`には`UI_GUILDCHAT`（値`guildchat`）～`UI_WHISPERREFUSE`（値`whisperrefuse`）付近、および`UI_FORCEWEEKLYLIFESTYLERESET`（値`forceweeklylifestylereset`）等、**全て小文字・スペースなしの英単語**が200件以上まとまって存在する。これらはチャット/コンソール経由で入力するGM管理コマンドのキーワードそのもの（サーバー側の構文と一致する必要がある識別子）であり、表示用テキストではないため**翻訳しない**。同じファイル内の`UI_MENU_*`（例：`UI_MENU_BAN`→`BAN`、`UI_MENU_GUILDJOIN`→`ギルド参加`）はGM右クリックメニューの表示ラベルであり、これらは通常のUIテキストとして翻訳対象。

| English | 日本語 | 備考 |
| --- | --- | --- |
| PProtect（`UI.csv`の`UI_PVP_UPGRADE_PROTECTSCROLL`等、短いラベル文脈のみ） | PVP編(PProtect) | `Items.csv`の`PROPITEM_TXT_913714`（Scroll of PProtect→鍛冶屋の心得・PVP編）の「PVP編」を使い、SProtect/XProtectと同じ「カテゴリ名+編(英語略称)」形式に統一（2026-07-31、ユーザー指示）。当初は`PROPITEM_TXT_913715`の説明文にある「(通称:PProtect)」を根拠に英語表記のまま据え置いていたが、SProtect/XProtectとの表記統一を優先する方針に変更 |
| XProtect（`UI.csv`の`UI_ULTIMATE_UPGRADE_PROTECTSCROLL`等、短いラベル文脈のみ） | アルティマ編(XProtect) | `UI_UPGRADE_PROTECTSCROLL`（SProtect→精錬編(SProtect)）の「カテゴリ名+編(英語略称)」形式に合わせた表記。この「精錬編(SProtect)」はGame Version 1.5.1導入時点（コミット`58c51bf`、作者lsaos）からの既存のオリジナル訳であり、我々の過去の翻訳ではないため変更せず、これに倣う方針とした（2026-07-30、ユーザー指示）。同コミットで導入されたXProtectの旧訳「エクスプロテクト」（音訳）とは表記スタイルを統一する形で修正。なお`Items.csv`の`PROPITEM_TXT_122510`（Scroll of XProtect）等、アイテム名としてのフル文脈では「鍛冶屋の心得・アルティマ」を使用し続ける（これは変更しない） |
| Tenacity（`UI_TOOLTIP_TENACITY`） | テナシティ | `Skills.csv`の`PROPSKILL_TXT_150331`に準拠 |

## 31件の未訳TXTファイル一斉翻訳時に確認・新規決定した用語（2026-08-08）

`Japanese/`直下の未訳（英語のまま）だった31個の`.txt`ファイル（`BlessingRemove.txt`〜`WeaponConvert_Unique.txt`）を一斉翻訳した際に確認した用語。大半は既存の`Items.csv`/`UI.csv`/`MoverMenus.csv`等の定訳をそのまま流用したが、以下はそれらのファイルに先例がなく新規に決定したもの、または複数の競合する既存訳から1つを選定したもの。

| English | 日本語 | 備考 |
| --- | --- | --- |
| Kalgas Assault | カルガスアサルト | `Items.csv`/`TextClient.csv`等で「カルガスアサルト」「カルガス・アサルト」の表記揺れが既にあるが、`KalgasAssault.txt`/`KalgasAssaultReg.txt`ではナカグロなしの「カルガスアサルト」に統一（既存訳の一括修正はしない） |
| Kalgas Chip（数量表現） | カルガスチップ{N}個 | `Items.csv`の「50x First Refresher」→「50個」等の個数表記パターンに準拠し、`KalgasAssault.txt`の「5x/10x/30x/20x/15x Kalgas Chips」を{N}個形式に変換 |
| artifact（`KalgasAssault.txt`のカルガス防衛オブジェクト） | アーティファクト | `Items.csv`の`PROPITEM_TXT_018325`の音訳に準拠。カルガスアサルト固有のゲームプレイオブジェクトで他ファイルに先例なし |
| Server Lord（`Donation.txt`） | サーバーロード | 他ファイルに先例なし新規決定。`Characters.csv`の`Lord Manager`→「ロードマネージャー」、`UI.csv`の`UI_DONATION_CURRENTLORD`「Current Lord」→「現在のロード」に準拠し、「Lord」の音訳「ロード」を踏襲 |
| Point Circle（`RainbowRaceRules.txt`） | ポイントサークル | レインボーレース固有のゲームプレイオブジェクトで先例なし、音訳で新規決定 |
| Secret Room（`SecretRoom.txt`） | シークレットルーム | `Items.csv`の`PROPITEM_TXT_130051`（Secret Room Reward Box→シークレットルーム報酬ボックス）に準拠。`Dialogs.csv`では同じ機能が創作訳「ギルド・オルタナティヴ」で呼ばれているが、`SecretRoom.txt`はアイテム名に合わせて音訳を採用 |
| Asmodan（`SecretRoom.txt`、ボスとしての言及） | ルシファー | `Movers.csv`の`PROPMOVER_TXT_001186`（モンスター名としての訳）に準拠。ただし「Asmodan clothes」「Asmodan weapon skins」等のアイテム文脈は`Items.csv`の音訳「アスモダン」を使い分ける（モンスター名とアイテム名で表記が異なる既存パターンを踏襲） |
| Story Mode（`StoryDungeon.txt`） | ストーリーモード | 他ファイルに先例なし、音訳で新規決定 |
| Element Upgrading / Item Upgrading（`ElementUpgrade.txt`/`GeneralUpgrade.txt`のヘッダー） | 属性精錬 / アイテムの精錬 | `AttributeRemove.txt`の既存訳「属性精錬の削除」（Remove Element Upgrade）に準拠。SProtect/AProtect/XProtectの説明文は`UI.csv`の`UI_UPGRADE_UNSAFE`等の短縮表記「精錬編(SProtect)」パターンをそのまま踏襲 |
| Remove Element（`MoverMenus.csv`の`MMI_59`） | 属性精錬の除去 | 旧訳「要素の削除」（直訳）から2026-08-12にユーザー指示で修正。同じ概念の`AttributeRemove.txt`（Remove Element Upgrade→属性精錬の削除）とは動詞が「除去」/「削除」で異なる点に注意（表記揺れとして残っている。一括統一はしない） |
| Remove Level Reduction（`LevelDownRemove.txt`） | 装備可能レベル低下キャンセル | `UI.csv`の`UI_LEVELDOWN_CANCEL_TITLE`と完全一致する既存訳をそのまま採用 |
| Item Piercing / Remove Piercing（`Piercing.txt`/`PiercingRemove.txt`） | アイテムのソケット作成 / ソケットカードの削除 | `UI.csv`の`UI_PIERCING_TITLE`（Piercing→ソケットの作成）、`UI_PIERCING_REMOVE_TITLE`（Remove Piercing Card→ソケットカードの削除）に準拠 |
| Pet Sacrificing（`PetRecycle.txt`） | ペットサクリファイス | `MoverMenus.csv`の`MMI_1015`と完全一致する既存訳をそのまま採用 |
| Unbinding（`Unbinding.txt`） | 帰属解除 | `MoverMenus.csv`の`MMI_1003`、`Items.csv`の`Scroll of Unbinding`→「帰属解除の巻物」に準拠。「Soul-Bound」＝キャラクター帰属（解除可能）、「Soul-Linked」＝プレイヤーに帰属（解除不可）という2種類の帰属を訳し分け |
| Remove Ultimate Jewel（`UltimateJewelRemove.txt`） | アルティマジュエルの削除 | `MoverMenus.csv`の`MMI_1097`と完全一致する既存訳をそのまま採用 |
| Prologue.txt固有名詞（マドリガル創世神話） | Madrigal→マドリガル、Rhisis→リシス、Roika→ロイカ、Bubble→バブル、Shade→シェード、Iblis→イブリス、Dwarpet(s)→ドワーフ、Masquerpets→モンスター | いずれも`Dialogs.csv`等の既存訳に準拠。特に「Masquerpets」は種族の固有名詞だが、既存訳では一貫して汎用語「モンスター」に意訳されているため、`Prologue.txt`でもこれを踏襲（意味的ニュアンスより既存表記との統一を優先） |

## 2026-08-12 upstream新規追加分（Movers/TextClient/Items、計198件）で新規決定した用語

`English_Reference`にupstreamから新規追加された198件（`PROPMOVER_TXT_550000〜550046`、`TEXTCLIENT_GUILDCOMBAT_*3`/`TEXTCLIENT_WAVEDEFENSE_*`/`TEXTCLIENT_PVPCONTEST_*`系、`PROPITEM_TXT_904086〜904121`・`PROPITEM_TXT_161078〜161149`）を翻訳した際に新規決定した用語。`PROPMOVER_TXT_550013〜550046`（Serus Uriel、Violet/Giant/Captain/Lord/Small/Grownup/Creep/1st Class + Aibatt系クラシックモンスター）は`Movers.csv`冒頭（`PROPMOVER_TXT_000006〜000092`等）の既存訳をそのまま流用（新規決定なし）。

| English | 日本語 | 備考 |
| --- | --- | --- |
| Fefern（`Movers.csv`のクラシックモンスター、根っこ系の植物モンスター） | フェフェルン（音訳） | `PROPITEM_TXT_004883`（フェフェルンがドロップする「乾燥した根」）が示す通り植物・根系のモンスターで火属性ではない。そのため`PROPITEM_TXT_161101`/`161145`の"fiery Fefern"の"fiery"は火属性の意味ではなく気性（怒りっぽい・気性が荒い）を表す形容と解釈し「気性の荒い」と訳す（2026-08-12、ユーザー指摘で「炎のような」から修正） |
| The Last Beacon（新規ダンジョン名、`PROPITEM_TXT_904102〜904103`で確認） | ラストビーコン | 他ファイルに先例なし、音訳で新規決定 |
| Wraithbark / Ironback / Swift Spiderling / Caboom（`PROPMOVER_TXT_550000〜550003`、The Last Beaconの雑魚モンスター） | レイスバーク／アイアンバック／スウィフト・スパイダーリング／カブーム | 音訳で新規決定。「Spiderling」単体は`PROPMOVER_TXT_001225`の既存訳「スパイダーリング」に準拠 |
| Winged Manticore / Gorvak Bonecrusher / Chief Zekaru（`PROPMOVER_TXT_550007〜550009`、The Last Beaconのボス） | ウィングド・マンティコア／ゴーヴァク・ボーンクラッシャー／チーフ・ゼカル | 音訳で新規決定 |
| Tyrant Ankou（`PROPMOVER_TXT_550008`、The Last Beaconのボス） | 暴君の神獣ベヒモス | `Ankou`→`ベヒモス`の既存音訳に加え、`Achievements.csv`の`Demonic Ankou`→「魔の神獣ベヒモス」等の「{形容語}の神獣ベヒモス」パターンに準拠して意訳 |
| [Common] / [Healthy] / [Fast] / [Explosive] / [BOSS] / [Friendly]（Movers.csvの角括弧タグ、The Last Beacon系） | [一般] / [健康] / [俊敏] / [爆発] / [ボス] / [フレンドリー] | 他の`[Guildwar Manager]`等の角括弧タグ同様、意訳（`[Event]`→`[イベント]`と同じ方針）。`[Friendly] Sailor Sniper/Gunner/Cannoneer`→`[フレンドリー] セーラー・スナイパー/ガンナー/キャノニア` |
| Trans（新規ペット、`PROPITEM_TXT_904086〜904101`） | {カタカナ名}・オーブ（アイテム名）／{カタカナ名}に変身できる魔法の水晶球（説明文） | 既存の`Aibatt Trans`→「アイバット・オーブ」（`PROPITEM_TXT_006096`等）パターンをそのまま踏襲 |
| Cage（モンスター捕獲アイテム、`PROPITEM_TXT_161082〜161149`） | {カタカナ名}ケージ（間に中点なし、直接結合） | 既存の`Angel Cage`→「エンジェルケージ」（`PROPITEM_TXT_008673`等）パターンに準拠 |
| Rare sighting! / Very rare sighting!（Cage説明文の目撃レア度） | 珍しい目撃情報! / 非常に珍しい目撃情報! | `PROPITEM_TXT_724385`等の既存訳に準拠 |
| Uncommon sighting!（Cage説明文の目撃レア度、新規追加分で初出） | やや珍しい目撃情報! | 「Rare」より低いレア度のため上記2段階に対して新規決定（2026-08-12） |
| Mars Dungeon（`PROPITEM_TXT_161083`） | フラリスダンジョン | `Map.csv`の`PROPMAP_TXT_000263`、`World.csv`の`Mars Mine`表記に準拠（英語名と日本語名が対応しない既存パターン） |
| Wave Defense（新規ゲームモード、`TEXTCLIENT_WAVEDEFENSE_*`系） | ウェーブディフェンス | 他ファイルに先例なし、音訳で新規決定。「sailor」（防衛NPC）→「船員」、「match」→「マッチ」、「room」→「ルーム」、「milestone」→「マイルストーン」（`UI_EVENT_ANNIVERSARY_DESC`等の既存訳に準拠） |
| Prune（`TEXTCLIENT_GUILDCOMBAT_OPEN_MSG3`、Lv165ギルドコンバット担当NPC） | プルーン | 既存のAtlas→アトラス、Olivia→オリビア（Lv80/60版）と同じNPC音訳パターン |

## Items.csv batch翻訳（PR#276前後）で確認した表記揺れ・追加用語

| English | 日本語定訳 | 備考 |
|---|---|---|
| Mars Mine | フラリスダンジョン | World.csv, Dialogs.csv, Quests.csv, ScenarioQuests.csv で多数使用。ただし ScenarioQuests.csv の一部（PROPQUEST_SCENARIO_INC_002830, 002832, 002836, 002837）のみ「火星鉱山」という直訳の表記揺れが残っている（既存の誤訳、要ユーザー指示のもと一括修正） |
| Shade | シェード | 旧「シェイド」表記が一部残存（表記揺れ）。PR#276で一部統一済み |
| Freeze（露店/個人商店を開いている間の行動不可状態） | フリーズ中 / 取り込み中 | 氷属性の状態異常ではなく、個人商店（露店）展開中にキャラクターがその場から動けなくなる状態を指すゲーム内用語。MoverMenus.csv (MMI_1010), UI.csv (UI_MENU_FREEZE) では「フリーズ中」表記。TEXTCLIENT_FREEZE_NOTUSE (You cannot teleport if you're frozen.) は PR#276 で「取り込み中のためテレポートできません。」に変更・採用（ユーザー確認済み）。関連: TEXTCLIENT_VENDOR_NOTUSE (個人商店を開いてる時は)。UI側「フリーズ中」とエラーメッセージ側「取り込み中」で表記が分かれている点は表記揺れとして留意 |

