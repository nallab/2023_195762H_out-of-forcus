# レビュー文における的外れ文抽出の試み
この研究はYouTubeより収集したコメントから的外れ文抽出に取り組んだ研究である．
以下に実行環境，手順を示す．

# 実行環境
google colaboratory
# 手順

### データ収集
YouTube Data APIを用いてYouTubeより実験に利用する動画のコメントを収集し，csvファイルに保存する．
ソースコードは**YouTubeComment1.ipynb**である．
APIキーと動画IDは各自で用意する必要がある．

### 収集したコメントのアノテーション付与
スクレイピングなどで収集したデータセットは公開できないとのことなのでnal研teemsにアップした．

### bertモデルを上記で用意したデータセットを用いてファインチューニングを行う．
ソースコードは**CommLearn.ipynb**である．
