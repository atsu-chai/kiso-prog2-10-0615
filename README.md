# 基礎プログラミングII — 第10回 演習

**日付:** 2026-06-15  
**テーマ:** テキストファイルを行単位で読む + サイエンスアート

---

## 今日の流れ

1. このリポジトリを **Fork** する（右上の Fork ボタン）
2. クローンして step ファイルを **番号順に** 動かす
3. `step5` まで完成したら `color.csv` を自由に書き換えてみる
4. ボーナス問題（`bonus_odd_divisible.c`）を解く
5. 変更を commit → push → **Pull Request** を送る

---

## ファイル構成（実行順）

| ファイル | 内容 |
|---------|------|
| `color.csv` | 色データ（名前・HSB・座標・半径） |
| `step1_fgets_line.c` | ① fgets で1行読む |
| `step2_fgets_loop.c` | ② fgets ループで全行読む |
| `step3_sscanf_parse.c` | ③ sscanf で文字列を分解する |
| `step4_color_csv.c` | ④ color.csv を読んでテキスト表示（完成版） |
| `step5_color_draw.c` | ⑤ color.csv を読んで raylib で描画（完成版） |
| `bonus_odd_divisible.c` | ★ ボーナス問題（発展） |

---

## コンパイル方法

```bash
# step1 〜 step4
gcc step1_fgets_line.c    -o step1
gcc step2_fgets_loop.c    -o step2
gcc step3_sscanf_parse.c  -o step3
gcc step4_color_csv.c     -o step4

# step5（raylib が必要）
gcc step5_color_draw.c -o step5 -lraylib -lm

# bonus
gcc bonus_odd_divisible.c -o bonus
```

---

## Pull Request の送り方

```bash
# 1. Fork したリポジトリをクローン
git clone https://github.com/あなたのID/kiso-prog2-09-0615.git
cd kiso-prog2-09-0615

# 2. ブランチを作る（名前は自分の名前で）
git checkout -b yamada-taro

# 3. ファイルを編集・追加したら
git add .
git commit -m "yamada-taro: 第10回提出"
git push origin yamada-taro

# 4. GitHub で Pull Request を作成する
```
