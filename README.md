# 左右反転画像 生成プログラム file.py

## 1.概要

引数で指定した画像の左右反転画像を作成するpython 3 で動作するプログラムです。

## 2.ソースコード

```python
# このプログラムは python 3 用です。
# あらかじめ pip- install pillow で pillow をインストールしておきます。
from PIL import Image
import sys

# コマンドライン引数から入力画面と出力画面のファイル名を取得
input_image = sys.argv[1]
output_image = sys.argv[2]

# 画像の読み込み
img = Image.open(input_image)

# 画像の左右反転
img_file = img/transpose(Image.FLIP_LEFT_RIGHT)

# 画像の保存
img_flip.save(output_image)
```

## 3.使い方
### 3.1.実行例
- コマンドインフォーマット
  ```python
  python3 file.py <input_image_path><output_image_path>
  ```
- 利用例
  ```python
  python3 file.py input.jpg output.jpg
  ```

### 3.2.出力結果

- 以下のように入力画像の左右反転画像が出力されます。

  |入力画像(imput.jpg)|出力画面(output.jpg)|
  |---|---|
  |![入力画像](input.jpg)|![出力画面](output.jpg)|

以上
