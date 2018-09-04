やること：タイタニック号の乗客データから生存者を予測する。

内容物：
・first.ipynb：
ウェブサイトのチュートリアルを実装してみたもの。
決定木を使って予測している。
https://www.codexa.net/kaggle-titanic-beginner/

・my_tree_one.csv：
上記ファイルから作った生存者予測その1。精度71%。

・my_tree_two.csv：
上記ファイルから作った生存者予測その2。精度76%。

方針：
データ数が「たかだか800」程度なので、ハンズオンでやったようなニューラルネットワークを使用するのは難しそう。
調べてみた限りでは、決定木もしくはSVMが多い。（原理から考えて予想時のカテゴリ数が少ないからこれらが一番楽なのでしょう。）
基本的な部分はウェブサイト見ればソースコードが書いてあるので、プロトタイプを実装したうえで一工夫しやすい方法をとりたい。
よって今回は決定木を採用することにした。（こっちの方が参考にできるサイトが多い）
英語なのはつらいが、時間があればKaggleのKernelも読んでみようと思う。
交差検証は今使っているsklearnにあるらしい。

使用ライブラリ：
・pandas
・sklearn

方法：
教師データの欠損を埋める。
決定木を作成。
教師データを使って交差検証。
返り値の数列の平均値を取る。

参考にしたサイト：
http://kefism.hatenablog.com/entry/2017/04/22/203740
https://mathwords.net/kousakakunin
http://aidiary.hatenablog.com/entry/20150826/1440596779
http://aidiary.hatenablog.com/entry/20150810/1439205637
http://blog.apitore.com/2016/07/05/kaggle-titanic-traial-and-error-2/
https://www.codexa.net/kaggle-titanic-beginner/
https://www.kaggle.com/c/titanic/leaderboard
http://scikit-learn.org/stable/modules/cross_validation.html
http://aiweeklynews.com/archives/50219779.html
https://blog.amedama.jp/entry/2017/09/05/221037


