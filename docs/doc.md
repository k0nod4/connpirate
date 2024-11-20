# connpirate

## Architecture

### AWS Resources
- Amazon VPC (パブリックサブネット / プライベートサブネット)
- Internet Gateway
- NAT Gateway + Elastic IP
- AWS Lambda
- AWS Systems Manager Parameter Store

| Resource | Description |
|----------|-------------|
| Amazon VPC | 仮想ネットワークを構築 (パブリックサブネット / プライベートサブネット) |
| Internet Gateway | VPC内のリソースがインターネットに接続するための出入口 (IPを持たない) |
| NAT Gateway + Elastic IP | プライベートサブネットに固定IPを振り、Internet Gatewayに通信を送信する |
| AWS Lambda | Serverless Compute Service、API通信を行う |
| AWS Systems Manager Parameter Store | Lambdaから読み込むAPIキーなどを保管する |

### Development Tools
- GitHub
- GitHub Actions