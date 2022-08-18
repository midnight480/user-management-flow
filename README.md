# ユーザ制御処理を整理

## 処理フロー

```mermaid
graph TD;
    GWS-->GAS;
    GAS-->SpreadSheet;
    SpreadSheet-->Lambda1;
    Lambda1-->DynamoDB;
    DynamoDB-->Lambda2;
    Lambda2-->AWS-SSO;
    Lambda1-->End;
    Lambda2-->End;
 ```
