## S3 Upload API

AWS Lambda Python 3.6で動作します。
API Gateway経由でS3にファイルをアップロードします。

API Gatewayのマッピングテンプレートとバイナリサポートに、以下を設定。
テンプレートはメソッドリクエストのパススルーを設定。

* application/octet-stream
* image/png
* image/jpg

UploadしたついでにRekognitionで顔分析した結果をリターンします。
