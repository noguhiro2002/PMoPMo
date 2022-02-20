# PMoPMo: Python Movie Process Modules
## Pythonを用いて動画を編集する、おそらくよく使われると思われるModuleを公開する
## 方針
ほぼ永久的に開発中。出来たらその分追加して公開。

## 現在のModules (Python Functions), 2022/02/20現在

1. inputExcelToProcessList
  - 役割：処理内容を書き込んだ定形Excelファイルを読み込み、rawMovieEditモジュールに読み込ませるための配列に変換。 
  - 使用Library: 
    - pandas
    - numpy
    - pprint
2. rawMovieEdit
  - 役割：入力動画（現時点ではGoProの1080p, 60fpsを想定。ファイル内のパラメーターを適当にセットすることで何でも応用可能）に、TimeStampとWaterMarkを書き込み、出力する。
  - 使用Library：
    - cv2
    - ffmpeg
    - datetime
    - tqdm
    - numpy
4. movieMerge
  - 役割：複数の動画をエンコードなしで、単純に結合（故に、結合する動画のエンコード・サイズなどは同じである必要あり）。
  - 使用Library：
    - ffmpeg
5. videoEncode
  - 役割：入力動画をエンコードする。
  - 資料Library：
    - ffmpeg

## License
Copyright 2022 noguhiro2002

Licensed under the Apache License, Version 2.0 (the “License”);
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an “AS IS” BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

