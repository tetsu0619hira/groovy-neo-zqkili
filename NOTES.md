# Groovy-neo デモサイト制作メモ

## 参考サイトと設計への反映（2026-09-19実閲覧）
- https://vench-salon.com/ ：FVは店名・店内写真。予約→紹介→特徴3点→新着→人気記事→店舗情報の6ブロック。白・黒と広い余白、サンセリフ、主導線は予約／LINE。紹介と予約の近さを採用し、本サイトは電話を主導線に変更。
- https://slow-salon.com/ ：FVはロゴ・ヘア写真。紹介→写真／予約→料金→お知らせの4ブロック。白地・細めの文字・余白多め、主導線はWEB予約。主要メニューの一覧性を採用し、営業時間と電話をFVへ移動。
- http://nico-hair-design.net/ ：FVはロゴ・左ナビ・予約ボタン（閲覧時メイン画像は未表示）。写真枠→SPECIAL CONTENTS→LINE UPの3ブロック。白基調・細めのサンセリフ・サーモン色の予約ボタン。常設の予約導線を採用し、スマホでは電話・地図・Instagramの固定バーに変更。
- https://atelier-blanche.net/ ：追加の構成参考。FVはスタイル写真。紹介→LINE UP→NEWS→BLOG→季節写真→SPECIAL CONTENTS→店舗情報の7ブロック。白地と繊細なロゴ、予約ボタンが目立つ。写真の余白感のみ参考にし、人物写真・多段の告知・クーポンは採用しない。好評口コミの裏付けは今回得られず、評判による選定3店には含めない。
- 美容室で探されるメニュー・料金、予約、営業時間、場所・駐車場、スタイリスト、店内の雰囲気、初回来店の案内を整理。構成は「ヒーロー／基本情報→メニュー→お店→予約・営業時間→アクセス→問い合わせ」。各サイトの文章・写真・ロゴ・固有レイアウトは転用していない。

## 評判の確認元
- vench： https://beauty.hotpepper.jp/slnH000751592/review/ （希望への対応・落ち着いて過ごせる点を評価する投稿を確認）
- SLOW： https://www.ekiten.jp/g0201/a20220/?f%5B%5D=14 （評価3.63・口コミ5件の掲載を確認）
- nico hair design：同上（評価4.51・口コミ35件）、 https://hairlog.jp/nagano/2005/%E8%B1%8A%E7%A7%91%E9%A7%85/S149252 （カラーの仕上がりへの好意的な掲載を確認）
- 評価値は参考店選定の調査メモにのみ記載。Groovy-neoのページには評価・件数を掲載していない。

## 仕様・情報の扱い
- 店名・住所・電話・ヘア営業時間は依頼文の記載を使用。現在の営業中表示は臨時休業が不明なため実装しない。
- 一般的な4メニューは仮の掲載項目。提供有無・施術内容も未確認として表示。具体的な金額、担当者名、確定していないサービスは記載しない。
- ヘアとアイラッシュの営業情報は混在させない。アイラッシュはお店についての1行のみ。
- 店舗紹介の表現は依頼文で許可された口コミ傾向の言い換え。原文引用なし。
- noindex／公式サイトではない旨／制作名を表示。CSSとJSはindex.html内、画像は相対パス。
- 依頼のGitHub Pages・public指定をAGENTS.mdの標準設定より優先。フォーム・解析は追加していない。

## Pexels素材（すべてイメージ写真）
| ID | 用途 | 写真ページ | 作者 |
|---|---|---|---|
| 7465903 | ヒーロー・ハサミとコーム | https://www.pexels.com/photo/a-pair-of-scissors-and-a-comb-7465903/ | Cleber wendder Nascimento |
| 8834030 | メニュー・道具 | https://www.pexels.com/photo/scissors-and-comb-laid-on-blue-towel-8834030/ | Kampus Production |
| 6207525 | 紹介・タオルと植物 | https://www.pexels.com/photo/potted-green-ficus-arranged-with-stack-of-towels-6207525/ | Skylar Kang |

取得URL形式：`https://images.pexels.com/photos/<ID>/pexels-photo-<ID>.jpeg?auto=compress&cs=tinysrgb&w=1200`。全3枚200KB以内。全写真に差し替えを明記したキャプションを重ねる。人物の顔、外観、看板、店内全景なし。Googleマップの写真・Instagram画像・併設サロンの写真は不使用。

## 地図
- 埋め込みは店名検索：`https://www.google.com/maps?q=Groovy-neo%20白馬村神城&output=embed`。
- 外部リンクは依頼のplace_id `ChIJm7t716XR918R2qlbRZQkILI` を使用。
- ピンと住所の目視確認結果は最終検証後に追記。

## 公開前に人が確認する事項
- 【要確認：Instagramアカウントが当店のものか（公開前に人が確認）】
- 【要確認：CutHouseGroovy（北城）との関係・移転前の店か】
- 実店舗の写真への差し替えと撮影・掲載許可。
- デモ公開は依頼に従って実施。公式サイトとしての公開・noindex解除は店舗確認後。
- 画面上の確認欄の全件は同梱の CHECKLIST.md に記録。

- 外部Googleマップのplace_idリンクで、Groovy-neoのピン、神城22742-1、電話0261-85-0990の一致を目視確認。
