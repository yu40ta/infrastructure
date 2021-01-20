### Zone Apex
Zone Apexは相対的なもの
- 例えば example.co.jp と www.example.co.jp がある場合、
  通常は example.co.jp が Zone Apex
- サブドメインの委任をすると www.example.co.jp がZone Apexとして扱われる
- Zone ApexにはCNAMEレコードが設定できない制約がある

### Domain Management
ドメイン管理のポイント
- ドメインをどこで取得するか（外部レジストラ/クラウド）
- ドメインをどこで管理するか（外部レジストラ/クラウド）
  - ネームサーバーの向き先
- FQDN/Zone Apex
  - Amazon RDS/ELB/CloudFrontはZone ApexをCNAMEレコードとして登録できない
