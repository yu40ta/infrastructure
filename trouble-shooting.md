## Amazon Web Services
### EC2
- メトリクス確認
  - アラーム: AutoRecoveryが走っているか -> false -> 復旧優先
  - データ欠落
  - 回復済み
- サイト表示チェック
  - ヘルスチェック検知していなくても
    - OKなら対応不要
    - NGなら復旧対応
- 症状例
  - つながらない(SSH接続できない、サイト表示されない)
　  - OutOfMemory→httpd kill (メモリ不足)
    - プロセスApache(httpd)が落ちた可能性
      -> OSまたはプロセス(例:httpd)の再起動
  - rebootでも復旧しない
    -> Stop&Start(ホスト移行)

