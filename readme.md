# finardry とは

FC 時代のウィザードリィを FC 時代の FF 風の UI にアレンジした二次創作ゲームです。レトロゲームエンジン Pyxel を使って制作しています。

ウィザードリィ初心者の方でも快適にプレイできるように、かなり難易度を下げたり、ウィザードリィ特有のリスキーな要素（キャラクタのロスト、いしのなかにワープ etc）は除いて、プレイしやすくしています。

タイトルは「フィナードリィ」と読んでください。

![Finardryイメージ画像](./static/ogp.jpg)

イメージ画像寄稿：ぽんた（@crumpets202204）様

## プレイ用 URL

https://finardry.web.app/

PC でもスマホでもプレイできますが、PC のほうが操作は快適だと思います。

PC に市販の USB 接続のゲームパッドを接続してプレイいただくことも可能です。ただし、稀に十字キーやパッドが反応しない場合もあるようです。

ゲームパッドをとりつけたスマホ、もしくは画面の小さいゲーム機などで、バーチャルパッドが不要という方は以下にアクセスください。

https://finardry.web.app/nopad.html

なおスマホ版は PWA 対応しているため、URL をホーム画面に追加すれば、アプリのような起動方法・見栄えでプレイすることもできます。

## ゲームデータのセーブ・ロードについて（必ずお読みください！）

- ゲームデータはお使いのブラウザのローカルストレージに保存されます。そのため、複数の端末で（PC とスマホなど）同じデータでプレイすることはできません。また、ブラウザのデータの全消去をするとゲームデータが消えてしまいますのでご注意ください。

- ブラウザがプライベート（シークレット）モードだったり、Cookie/ローカルストレージの使用を許可していない場合、セーブが行えないことがあります。一見セーブができているように見えてもブラウザを閉じるとデータが消えていることがあるため、ご注意ください。

- Safari を使用している場合、前回プレイから 7 日以上経過してからロードすると、セーブデータが初期化されてしまいます。これは Safari の場合にローカルストレージのデータが自動的に削除される仕様によるもので、対策検討中です。

## 原作 Wiz との主な違い（Wiz 経験者向け）

- キャラクタの蘇生失敗がありません。したがってロストもありません。
- 全滅しても迷宮内に放置されず、キャッスルに戻されます。
- テレポートで石の中にワープしません。
- エナジードレインでレベルを下げられません。ドレインは HP 吸収攻撃（FF のドレイン）になっています。
- パーティ編成は 6 人ではなく 5 人です（後列 2 人）。
- モンスターはグループ構成ではなく単体で最大 5 体です。グループ対象の呪文は全体対象になります。
- モンスターの呪文無効化がダメージ呪文以外（マカニト等）にも発動します。
- 宝箱の罠解除がありません。宝箱については後述します。
- 罠解除できない代わりに盗賊を少し強化、僧侶を弱体化させています。初期パーティの隊列は「戦士 → 僧侶 → 盗賊 → 魔法使い」ではなく「戦士 → 盗賊 → 僧侶 → 魔法使い」が基本となります。
- キャラクタメイキングにおけるステータス割り振りはなく、強制的に決まります。名前も自動的に付与されます（変更はできます）。
- 呪文の数が原作に比べて少なく、レベルは 7 までではなく 6 までです。また、魔法使いと僧侶の MP 枠が同じです。
- レベルアップは宿屋ではなく戦闘終了時に行います。さらに、キャッスルに戻ると HP/MP が回復するので、そもそも宿屋がありません。
- 原作 FC 版で有名な AC バグ（自分ではなく相手の AC を参照する）は再現していないので、防具はちゃんと機能します。
- 識別やモンスターの不確定名がありません。そのかわりビショップは戦闘中に「しきべつ」ができて、敵のステータスを調べられます（FF の「ライブラ」の効果です）。
- アイテムは各キャラ所持ではなく共通インベントリ方式です。
- まきものやくすり以外のアイテムは使ってもなくなりません。
- 一部の武器防具に、FC 版にない耐性や種族特攻があります。
- 素手で攻撃できません。忍者も武器必須になります（クリティカルは出ます）。

## Wiz 未経験者の方へ

- ダンジョン内には「玄室」と呼ばれる、必ずモンスターが出現するマスがあります（モンスターは見えません）。また、戦闘から逃走すると一歩前に戻されます。つまり玄室のモンスターは倒さないと先へ進むことができません。玄室のモンスターを倒すと、宝箱を見つけることができます。
- ダンジョン内には「隠し扉」があります。「隠し扉」の先に重要アイテムがあったりするのでくまなく探しましょう。ミルワの呪文や「あかりのまきもの」を使うと見つけやすいです。
- たまに「ゆうこうてきなモンスター」が現れます。戦うと善のメンバーの性格が悪に、立ち去ると悪のメンバーの性格が善になることがあります。そして、善のメンバーは悪のメンバーと一緒にパーティを組むことができないのでご注意ください。
- 本作の防御力は「AC（アーマークラス）」で表されます。後年の多くの RPG と異なり、AC は低いほど防御性能が高いことを示しますので注意してください。防具のない裸の状態では AC が 10 で、AC が-10 以下になると「LO」と表示されます。「LO」は基本的に物理攻撃に対して無敵の状態です。

## ダンジョン内の宝箱について

- 宝箱には一定の確率で罠が仕掛けられています。罠がなければ、宝箱を開けて報酬を獲得することができます。罠が入っている場合は開けると罠が発動します。中身は手に入りますが、少しグレードが下がるものになります（原作同様）。
- (ver 2023/10/26 にて仕様追加) 盗賊がパーティにいる場合のみ、罠がかかっている宝箱を開けた際に罠解除できることができます。ただし、確率はあまり高くありません。また、忍者にはこのスキルはありません。
- 罠が仕掛けられているか判断する方法として、「しらべる」か、僧侶の呪文「カルフォ」があります。「しらべる」の成功率は「盗賊 → 忍者 → その他」の職業の順に高くなります。また、調べる際に失敗して罠が暴発することがありますが、暴発率は成功率に反比例します。「カルフォ」はほぼ 100%の精度で正しく判断可能で、罠の発動はしません。
- 罠の効果には状態異常を伴うものが多いですが、武器や防具に状態異常耐性がある場合、罠の効果も無効化できます。したがって、たとえばメンバー全員に毒耐性があり、「どくばり」や「ガスばくだん」が仕掛けられている場合であれば、開けても被害を受けません。

| 罠の名前             | 効果                                             | 宝箱の中身                 |
| -------------------- | ------------------------------------------------ | -------------------------- |
| どくばり             | メンバー 1 人が毒状態になります。                | 獲得できます               |
| ガスばくだん         | メンバー複数が毒状態になります。                 | 獲得できます               |
| いしゆみのや         | メンバー 1 人がダメージを受けます。              | 獲得できます               |
| ばくだん             | メンバー複数がダメージを受けます。               | 獲得できます               |
| スタナー             | メンバー 1 人が麻痺状態になります。              | 獲得できます               |
| テレポート           | 同じフロアの違う地点に強制的に飛ばされます。     | 獲得できません             |
| メイジブラスター     | 魔法使い・侍が麻痺または石化状態になります。     | 獲得できます               |
| プリーストブラスター | 僧侶・ビショップが麻痺または石化状態になります。 | 獲得できます               |
| けいほう             | モンスターとの強制戦闘になります。               | 戦闘後、再度宝箱が現れます |

## 更新履歴

※ 小さなバグの修正などは記載していないのでご了承ください。

2023/11/21 ラスボス不在時に代理モンスターが出現するように変更　＊＊＊　 zak (X @zakkas783)様、ありがとうございます　＊＊＊

2023/10/31 ラスボス再戦の仕様変更、カドルトを戦闘中使用可能に、アイテムの所持数を表示

2023/10/29 名前としてカタカナの「ヴ」が入力できるように、ミルワ・ロミルワの説明を変更

2023/10/27 コントローラ Y/上ボタン長押しでソフトリセット、宝箱のアイテムを持っていくか確認する仕様を追加

2023/10/26 コンフィグ機能（オートセーブ、BGM のオン・オフ）追加、盗賊の罠解除スキル、ステータス異常復帰時に自動的に元の隊列に戻す機能を追加

2023/10/23 リセットをソフトリセットに変更、キーを ESC→ESC+1 に（誤操作防止）、HJKL キーでも移動可能に

2023/10/21 初版リリース
