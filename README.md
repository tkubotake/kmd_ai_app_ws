# kmd_ai_app_ws
# 動作確認環境
`Python 3.6.1 :: Anaconda 4.4.0 (x86_64)`

# 環境設定

`$ pip install opencv-python`
Fashion MNISTのデータをダウンロードする。

# ファイルの種類
- 01_check_data.ipynb ：　Fashion MNIST でデータセットの雰囲気を掴む
- 02_run_fashion_mnist.ipynb ： Fashion MNIST で画像分類を実施してみる
- 03_run_dnn_from_folder.ipynb ： 自身で用意したデータセットで（ディレクトリ内の画像ファイルを元に）ディープラーニング

## Get the Data from Fashion MNIST
- Fashion MNIST（ https://github.com/zalandoresearch/fashion-mnist ）

You can use direct links to download the dataset. The data is stored in the **same** format as the original [MNIST data](http://yann.lecun.com/exdb/mnist/).

| Name  | Content | Examples | Size | Link | MD5 Checksum|
| --- | --- |--- | --- |--- |--- |
| `train-images-idx3-ubyte.gz`  | training set images  | 60,000|26 MBytes | [Download](http://fashion-mnist.s3-website.eu-central-1.amazonaws.com/train-images-idx3-ubyte.gz)|`8d4fb7e6c68d591d4c3dfef9ec88bf0d`|
| `train-labels-idx1-ubyte.gz`  | training set labels  |60,000|29 KBytes | [Download](http://fashion-mnist.s3-website.eu-central-1.amazonaws.com/train-labels-idx1-ubyte.gz)|`25c81989df183df01b3e8a0aad5dffbe`|
| `t10k-images-idx3-ubyte.gz`  | test set images  | 10,000|4.3 MBytes | [Download](http://fashion-mnist.s3-website.eu-central-1.amazonaws.com/t10k-images-idx3-ubyte.gz)|`bef4ecab320f06d8554ea6380940ec79`|
| `t10k-labels-idx1-ubyte.gz`  | test set labels  | 10,000| 5.1 KBytes | [Download](http://fashion-mnist.s3-website.eu-central-1.amazonaws.com/t10k-labels-idx1-ubyte.gz)|`bb300cfdad3c16e7a12a480ee83cd310`|

### 画像収集系
- 大量の画像入手のため、「ImageSpider」（ http://www.vector.co.jp/soft/dl/winnt/net/se425690.html ）

### 画像分類のアイデア
- Tensorflowでロゴ画像を分類する（ http://stmind.hatenablog.com/entry/2016/08/21/174218 ）
    - GitHub - satojkovic/DeepLogo: A brand logo recognition system using deep convolutional neural networks.（ https://github.com/satojkovic/DeepLogo ）
- ねこと画像処理 part 3 – Deep Learningで猫の品種識別（ http://www.robots.ox.ac.uk/~vgg/data/pets/ ）
    - cat classifier - wellflat/cat-fancier（ https://github.com/wellflat/cat-fancier/tree/master/classifier ）
- TensorFlowでキルミーアイコン686枚によるキルミー的アニメ絵分類 | 独自のデータセット読み込み（ https://qiita.com/domkade/items/fc9903c2119fdfa9a234 ）
