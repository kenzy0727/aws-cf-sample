# CloudFormation sample

## 想定アーキテクチャ
SQSのメッセージキューをトリガーに非同期実行するバッチアプリケーション

### 事前準備
AMIとKeyPair作成

### スタック作成順
1. cf-template-network.yml (VPC,Subnet,SecurityGroup)
2. cf-template-service.yml (S3,SQS,DynamoDB,SNS)
3. cf-template-iam.yml (Policy,IAMRole,InstanceProfile)
4. cf-template-autoscaling.yml (AutoScaling)
