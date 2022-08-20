# raisetech-live15
- CircleCIで下記のworkflowを実行するサンプルリポジトリです。

## Workflow
1. リポジトリにコードをpush
2. CircleCIがリポジトリにpushされたことをイベントトリガーとして、workflowを実行
3. 最初のworkflowとしてCloudformationを実行
4. 2番目のworkflowとしてCloudformationによって作成されたAWS環境に対して、ansibleを実行
5. 3番目のworkflowとしてServerspecで自動テストを実行する

## 実行環境
### ansible
```
$ ansible 2.10.3
```
