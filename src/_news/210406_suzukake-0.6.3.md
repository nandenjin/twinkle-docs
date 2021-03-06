---
title: 一部の科目が表示されない不具合が修正されました - suzukake@0.6.3
tags:
  - release
  - suzukake
  - kdb
date: 2021-04-06
---

本日 4/6 のアップデートで、[Twinkle "suzukake"](https://app.twinkle.nandenjin.com)はバージョン 0.6.3 になりました。

[[toc]]

## 一部の科目が表示されない不具合が修正されました

大学院授業など、一部の科目がコレクションに表示されない不具合がありました。(Internal Issue `#333`)

これは登録済みの科目データを読み込む際のロジックの誤りによるもので、登録時には正常にコレクションに表示される授業が、次回読み込み時には表示されない問題が発生します。なお、旧UI ["keyaki"](https://twinkle.nandenjin.com/app)はこの問題の影響を受けません。

問題は`v0.6.3`で修正されました。ご迷惑をおかけいたしました。

## 一部の科目の開講時期を修正しました

2021年度のKdBデータの記法を精査し、誤りのあった開講時期を修正しました。

シラバスと異なる開講時期でカレンダーが登録されていた方は、当該科目を再度追加し直すことで新しいデータが反映されます。

なお、これに対応する`parser`のバージョンは後日公開されます。

## そのほかの改善

- 科目リスト上のボタンを押すと、科目詳細が開いてしまう不具合が修正されました。(Internal Issue `#330`)
- モバイルで科目詳細を閲覧する際にも、科目リストのスクロール位置が保持されるようになりました。(Internal Issue `#329`)
- そのほか、軽微な表示不具合が修正されました。(Internal Issue `#155`他)

-> [**Twinkleを開く**](https://app.twinkle.nandenjin.com)

---

ご意見・不具合のご報告をお待ちしています。アプリ内のフィードバック、[`docs`リポジトリのDiscussion](https://github.com/nandenjin/twinkle-docs/discussions)、EmailやTwitterでお寄せください。
