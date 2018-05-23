# AWS_serverless_Chapter5_spa-backend 写真投稿サイトをシングルページアプリケーションで作ろう、のバックエンド側lambda関数とCloudFormationスタック作成SAM(template.yaml)


パッケージ作成コマンド
$ aws cloudformation package --template-file template.yaml --output-template-file template-output.yaml --s3-bucket serverless-app-photos-yah

パッケージデプロイコマンド
$ aws cloudformation deploy --template-file template-output-yaml --stack-name serverless-app-yah --capabilities CAPABILITY_IAM --region ap-northeast-1
