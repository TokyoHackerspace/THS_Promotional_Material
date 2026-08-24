# Booth Table Cloth — Layout & Design Rationale
# ブース用テーブルクロス — 割付と設計意図

**Tokyo Hackerspace / For Maker Faire Tokyo 2026**

English is the primary text. Each section is followed by a Japanese block carrying the same information.

> 英語のあとに、同じ内容の日本語を引用ブロックで併記した。

---

## 1. Summary / 概要

A single-piece 1800 × 1300 mm flame-retardant cloth covering the table top and the front drop. Navy ground, white logo, one colour. The table top is left plain; the logo sits on the front drop.

> 天板と前面だけを覆う1枚布のテーブルクロス（1800×1300mm、防炎）。ネイビー地に白ロゴの1色刷り。天板は無地にして、ロゴは前垂れにだけ入れる。

| Item / 項目 | Value / 値 |
| --- | --- |
| Cloth size / 仕上がりサイズ | 1800 × 1300 mm |
| Material / 素材 | Tarpaulin ターポリン, 510 g/m² |
| Fire retardancy / 防炎 | JFRA certified, label included / 日本防炎協会認定品・防炎ラベル付き |
| Print / 印刷 | Latex inkjet, single pass / ラテックスインクジェット・1パス |
| Logo size / ロゴ寸法 | 921.232 × 360 mm |
| Logo datum / ロゴ基準 | 170 mm up from the bottom edge / 布の下端から170mm |
| Side margins / 左右マージン | 439.384 mm each / 左右それぞれ439.384mm |
| Vendor / 発注先 | Shiropri しろプリ（オーエムカラーコピー株式会社） |
| Price / 価格 | ¥9,400 + tax = ¥10,340, shipping excluded / 税別9,400円・税込10,340円、送料別 |
| Lead time / 納期 | Approx. 5 business days / 約5営業日 |

Vendor prices surveyed 24-AUG-2026. / 価格は2026年8月24日時点の調査結果。

---

## 2. Target table / 対象のテーブル

Maker Faire Tokyo supplies rental tables of 1800 × 600 mm, and the height is 600 mm. Japanese event tables are commonly 700 mm high, but 600 mm units are also in circulation, so the layout below is designed to work with either height.

> Maker Faire Tokyo のレンタル備品は 1800×600mm、高さは600mm。
> 日本のイベント用長机は高さ700mmが一般的だが600mmのものも流通しているため、以下の割付はどちらの高さでも成立するようにした。

---

## 3. Flat layout / 展開図

```
        |<------------------------ 1800 ------------------------>|
        +--------------------------------------------------------+ --+
        |                                                        |   |
        |        TABLE TOP -- navy only, no print                |   |
        |                                                        |   | 600
        |                                                        |   |
        |                                                        |   |
     ---+- - - - - - - - - - - - - - - - - - - - - - - - - - - - + --+  <- fold A : 700 mm desk
        |                                                        |   | 100
     ---+- - - - - - - - - - - - - - - - - - - - - - - - - - - - + --+  <- fold B : 600 mm desk
        |                                                        |   | 70
        |       +----------------------------------------+       | --+
        |       |                                        |       |   |
        |       |          LOGO  921.232 x 360           |       |   | 360
        |       |           tokyo hackerspace            |       |   |
        |       |                                        |       |   |
        |       +----------------------------------------+       | --+
        |                                                        |   |
        |                                                        |   | 170
        +--------------------------------------------------------+ --+

        bottom edge sits on the floor
        1300 = 600 + 100 + 70 + 360 + 170
```

Legend / 凡例

| Diagram label | Meaning / 意味 |
| --- | --- |
| `TABLE TOP` | Table top surface / 天板 |
| `fold A / fold B` | Fold line for each desk height / 机の高さごとの折り目 |
| `bottom edge` | Bottom edge of the cloth, sits on the floor / 布の下端、床に接する |

- Logo is horizontally centred. Left and right margins are 439.384 mm each.
- Logo top measured from the artboard top edge: 770 mm (1300 − 360 − 170).
- Bleed: 20 mm on all four sides. Extend the navy fill past the trim line so no white edge appears if the cut shifts.
- The fold lines are for reference only. They must not appear in the print data; keep them on a separate guide layer or delete them before submitting.

> - ロゴは左右中央。左右マージンはそれぞれ 439.384mm。
> - アートボード上端からロゴ上端までは 770mm（1300 − 360 − 170）。
> - ぬりたしは四辺 20mm。断裁がずれても白フチが出ないよう、ネイビーのベタを仕上がり線の外まで伸ばす。
> - 折り目の線は参考用。印刷データには含めないこと。別のガイドレイヤーに置くか、入稿前に削除する。

---

## 4. Why the bottom edge is the datum / 基準を布の下端にした理由

The cloth is a fixed 1300 mm. On a 700 mm desk it fits exactly: 600 mm over the top plus a 700 mm drop. On a 600 mm desk there is 100 mm of surplus, which is taken up at the back of the table.

Either way the front bottom edge lands on the floor. That makes the bottom edge the only reference point that does not move with the table height.

If the logo were dimensioned from the fold instead, a 600 mm desk would push it 100 mm closer to the floor — into the zone that gets blocked by chairs, crates and visitors' legs.

> 布は1300mm固定。高さ700mmの机ならぴったり収まる（天板600mm＋前垂れ700mm）。
> 600mmの机では100mm余るので、その分はテーブルの背面で処理する。
>
> どちらの場合も前面の下端は床に来る。つまり「布の下端」は、机の高さによって動かない唯一の基準点になる。
>
> もし折り目を基準に寸法を取っていたら、600mmの机ではロゴが100mm床側に下がり、椅子・機材ケース・来場者の足で隠れる帯に入ってしまう。

```
   700 mm desk                         600 mm desk
   -----------                         -----------
   =================  <- table top     =================  <- table top
   |      170      |                   |       70      |
   +---------------+                   +---------------+
   |               |                   |               |
   |      LOGO     |  360              |      LOGO     |  360
   |               |                   |               |
   +---------------+                   +---------------+
   |      170      |                   |      170      |
   #################  <- floor         #################  <- floor

   centred in the drop                 100 mm surplus hangs
                                       at the BACK of the table
```

Legend / 凡例 — `table top` = 天板の縁, `floor` = 床,
`centred in the drop` = 前垂れの中央に収まる,
`100 mm surplus hangs at the BACK` = 余った100mmは背面に垂らす

**Setup note** — on a 600 mm desk the surplus must hang at the back. Letting it pool on the floor at the front lowers the effective height of the logo by 100 mm and undoes the whole point of this layout.

> **設置時の注意** — 600mmの机では、余った布を必ず背面に垂らすこと。前面で床にたるませると、ロゴの実質的な高さが100mm下がり、この割付の意味がなくなる。

---

## 5. Why the logo is 360 mm tall / ロゴ高さを360mmにした理由

170 + 360 + 170 = 700. On a 700 mm desk the logo is exactly centred in the front
drop.

On a 600 mm desk the clearance below the table edge drops to 70 mm. Setup misalignment is on the order of 20–30 mm, so 70 mm is still enough to keep the logo from wrapping onto the table top.

The width follows from the lockup's aspect ratio of 2.5590 : 1 (921.232 = 895.642 × 360 ÷ 350). Scale with the aspect ratio locked.

If the table height is later confirmed as 600 mm and more clearance is wanted, 340 × 870.052 mm gives 90 mm below the table edge.

> 170 + 360 + 170 = 700。高さ700mmの机では、ロゴが前垂れのちょうど中央に来る。
>
> 600mmの机では天板の縁からの余白が70mmまで詰まる。設置のずれは20〜30mm程度なので、70mmあればロゴが天板側に回り込むことはない。
>
> 幅はロックアップの縦横比 2.5590 : 1 から算出している（921.232 = 895.642 × 360 ÷ 350）。拡大は必ず縦横比を固定して行う。
>
> 後から机の高さが600mmと確定し、もっと余裕を取りたい場合は、340 × 870.052mm にすると天板の縁から90mm確保できる。

---

## 6. Why the table top is left plain / 天板を無地にした理由

1. **It is covered anyway.** Demos, handouts, laptops and power strips hide most of the top surface at a Maker Faire booth.
2. **It gets dirty.** Objects are placed on it and dragged across it. White ink shows every mark; plain navy hides wear.
3. **Printing it is free, and that is the point.** The price is per sheet, not per printed area. Printing the top would neither save money nor cost extra — so there is no upside to offset the two downsides above.

> 1. **どのみち隠れる。** Maker Faire のブースでは、展示物・配布物・ノートPC・電源タップなどで天板の大半が覆われる。
> 2. **汚れる。** 物を置いたり引きずったりする面。白インクは汚れが目立つが、ネイビーの無地なら傷みが分かりにくい。
> 3. **印刷しても無料。それが論点。** 価格は印刷面積ではなく1枚単位で決まる。天板に印刷しても安くならないし高くもならない。つまり上の2つの欠点を打ち消すだけの利点がない。

---

## 7. Why the two-line lockup was kept / 2行ロックアップを維持した理由

The front drop is 1800 × 700 mm — a wide, short area. A single-line lockup was considered to make better use of that width, and rejected.

The Tokyo Tower glyph that replaces the "A" in *hackerspace* defines the top of the lockup. In the two-line arrangement, "tokyo" sits in the space beside the
spire, so the tower's height is already being put to work. Flattening the lockup to one line keeps roughly the same overall height but roughly doubles the width — which makes the letterforms smaller relative to the box, not larger.

The two-line lockup is the most compact form of this mark. Keep it.

> 前垂れは1800×700mmの横長。その幅を活かすため横1行への組み直しを検討したが、不採用とした。
>
> *hackerspace* の「A」にあたる東京タワーが、ロックアップの一番高い点を決めている。
> 2行組みでは、尖塔の横にできる空間に「tokyo」が収まるので、タワーの高さがすでに活用されている。1行に組み直しても全体の高さはほぼ変わらず、幅だけが約2倍になる。
> つまり枠に対して文字が相対的に小さくなり、読みにくくなる。
>
> 2行組みがこのマークの最もコンパクトな形なので、維持することとする。

---

## 8. Horizontal space / 横方向の余白について

With a 921 mm logo on an 1800 mm cloth, roughly 880 mm of navy is left empty.
This is deliberate. Plain ground makes the mark read from further away, and the lower part of the drop is obstructed at a busy booth anyway, so filling the space buys little.

> 1800mmの布に921mmのロゴなので、約880mm分がネイビーの余白になる。これは意図的。
> 無地の余白があるほうがマークは遠くから読める。また前垂れの下側は混雑時にはどのみち隠れるため、余白を埋めても得られるものは少ない。

---

## 9. Format choice / 形状の選択

Prices below are for quantity 1, flame-retardant with certification label, tax included, shipping excluded. **Surveyed 24-AUG-2026** — treat them as a snapshot
of the decision, not as current pricing.

> 以下は1枚・防炎ラベル付き・税込・送料別の価格。**2026年8月24日時点**の調査結果で、判断時のスナップショット。現在価格ではない点に注意。

| Format / 形状 | Vendor / 業者 | Unit price / 1枚価格 | Chosen / 採用 |
| --- | --- | --- | --- |
| Front only / 前面のみ | Shiropri しろプリ | ¥10,340 | ✅ |
| Front only / 前面のみ | Signmall サインモール | ¥12,980 | |
| Three sides, flat / 3面フラット | Signmall サインモール | ¥18,480 | |
| Three sides, flat / 3面フラット | Nobori King のぼりキング | approx. ¥24,000 / 約24,000円 | |
| Box, four sides / ボックス4面 | Signmall サインモール | ¥28,380 | |

Three-sided coverage costs roughly ¥8,000 more. For a two-day event that difference was not judged worth it.

One-colour artwork does **not** reduce the price at any of these vendors. They all print full-colour inkjet or dye-sublimation, so cost is driven by size and format only.

> 3面にすると約8,000円高くなる。2日間のイベントとしては、その差額に見合わないと判断した。
>
> 1色刷りにしても、ここに挙げたどの業者でも価格は下がらない。各社ともフルカラーのインクジェットまたは昇華転写で刷るため、価格を決めるのはサイズと形状だけ。

---

## 10. Others / その他

- **Navy colour value / ネイビーの色値.**
  - The navy must be specified in CMYK. The value from [5050_navy.ai](https://github.com/TokyoHackerspace/THS_Promotional_Material/blob/master/Printable%20Assets/Stickers/Square%2050mm%20X%2050mm/5050_navy.ai), which is a CMYK document, sticker design.
  - ネイビーはCMYKで指定すること。ステッカーのデザインかつCMYKドキュメントである [5050_navy.ai](https://github.com/TokyoHackerspace/THS_Promotional_Material/blob/master/Printable%20Assets/Stickers/Square%2050mm%20X%2050mm/5050_navy.ai), の色値を
  そのまま引き継ぐ。

- **Shipping fee / 送料**
  - Shipping fees are sometimes waived for orders exceeding a certain amount. For this project, it was cheaper to add a 50-pack of business cards (monochrome, single-sided printing) for 770 yen than to pay for shipping, so I also had business-card-sized THS cards printed.
  - 送料は一定額以上の注文で無料になる場合がある。今回の制作では、送料を払うよりも770円の名刺50枚パック（モノクロ片面印刷）を追加したほうが、安上がりだったので、併せてビジネスカードサイズのTHSのカードを印刷した。
