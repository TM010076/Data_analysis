# ウィスコンシン州の乳がん診断データを解析する

## データ解析の目的
  * ウィスコンシン州の乳がん診断データにおいて、良性と悪性の場合でそれぞれの腫瘍半径（radius_mean）に有意差があることを検証する。
  * 尚、有意水準は5％とします。

## 仮説立案
   * 帰無仮説（H0）：良性の腫瘍半径　=　悪性の腫瘍半径
   * 対立仮説（H1）：良性の腫瘍半径　<　悪性の腫瘍半径
    　
## 学習に使うデータセット
  * UC Irvine Machine Learning Repository から Diagnostic Wisconsin Breast Cancer Database をダウンロードします。
  * 属性情報（主要な列のみ、以下に概要を記載します。）
   1. id：連番
   2. diagnosis："B"か"M"の文字が格納されている（"B"：良性、"M"：悪性）
   3. radius_mean：腫瘍半径（中心から外周までの平均距離）
   4. texture_mean：グレースケール（色の濃さ）の平均値
   5. perimeter_mean：外周の平均の長さ
        
## 結果
  * p値が0.05を下回っているので、"有意差あり"とみなすことができ、「良性の腫瘍半径は悪性の腫瘍半径より小さい」と判断できました。
