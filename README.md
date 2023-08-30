# ウィスコンシン州の乳がん診断データを解析する

## データ解析の目的
  * ウィスコンシン州の乳がん診断データにおいて、良性と悪性の場合でそれぞれの腫瘍半径（radius_mean）に有意差があることを検証する。
  * 尚、有意水準は5％とします。

## 仮説立案
   * 帰無仮説（H0）：良性の腫瘍半径　=　悪性の腫瘍半径
   * 対立仮説（H1）：良性の腫瘍半径　<　悪性の腫瘍半径
    　
## 学習に使うデータセット
  * UC Irvine Machine Learning RepositoryからDiagnostic Wisconsin Breast Cancer Databaseをダウンロードします。
  * 属性情報（主要な列のみ、以下に概要を記載します。）
   1) ID number
    2) Diagnosis (M = malignant, B = benign)
    3-32) Ten real-valued features are computed for each cell nucleus:
       a) radius (mean of distances from center to points on the perimeter)
       b) texture (standard deviation of gray-scale values)
       c) perimeter
       d) area
       e) smoothness (local variation in radius lengths)
       f) compactness (perimeter^2 / area - 1.0)
       g) concavity (severity of concave portions of the contour)
       h) concave points (number of concave portions of the contour)
       i) symmetry
       j) fractal dimension ("coastline approximation" - 1)
    
## 結果
  * p値が0.05を下回っているので、"有意差あり"とみなすことができ、「良性の腫瘍半径は悪性の腫瘍半径より小さい」と判断できました。
