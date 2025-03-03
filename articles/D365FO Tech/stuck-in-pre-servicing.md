---
title: パッケージ適用時にサービス提供前 (Pre-Servicing) という環境のステータスが数時間続く場合について
date: 2022-10-24
tags:
  - D365FO
  - Tech
  - LCS
  - Information
disableDisclaimer: false
---

こんにちは、Dynamics ERP サポートチームの福原です。

この記事では、Dynamics 365 Finance and Operations のサンドボックス環境・本番環境に対してパッケージ適用を開始した際に、LCS 上でサービス提供前 (Pre-Servicing) という環境のステータスが数時間続く場合がございますことをご案内いたします。
<!-- more -->
---

まず、Dynamics 365 Finance and Operations のサンドボックス環境、本番環境に対して LCS よりパッケージ適用を開始した際に、始めに環境のステータスはサービス提供前 (Pre-Servicing) [*1](#link1) というものに変化いたします。  
サービス提供前 (Pre-Servicing) 中では、環境自体にアクセスすることが可能なまま、システムのバックグラウンドにてパッケージ適用に問題が発生しないか等の事前チェックが実施されます。  
注意事項と致しまして、サービス提供前 (Pre-Servicing) を含めたパッケージ適用全体で、 1, 2 時間で完了する場合もございますが、システム側の負荷状況や適用されるパッケージによりましては、サービス提供前 (Pre-Servicing) だけでそれ以上の時間がかかることがございます。  
<a id='link1'></a> (*1) : [サービス提供前およびサービス提供後](https://learn.microsoft.com/ja-jp/dynamics365/fin-ops-core/dev-itpro/lifecycle-services/pre-post-servicing)

サービス提供前 (Pre-Servicing) にどれだけの時間がかかるかを事前に予想することは難しいため、パッケージ適用の際には余裕をもってスケジュールして頂きますようお願いいたします。  
なお、以下の公開資料に記載がございます通り、パッケージ適用全体の平均の処理時間は約 5 時間となります。
もしそれ以上の時間が経ってもパッケージ適用が完了せず、お客様の業務に支障が出る場合には弊社までお問い合わせ頂けますと幸いです。  
[クラウド環境へ更新プログラムを適用](https://learn.microsoft.com/ja-jp/dynamics365/fin-ops-core/dev-itpro/deployment/apply-deployable-package-system)  
> 平均環境で単一パッケージのアプリケーションは、約 5 時間のダウンタイムが必要です。  
  
基本的にはサービス提供前 (Pre-Servicing) を含みまして、パッケージ適用が開始されましたら、弊社でもお客様でもパッケージ適用をキャンセルすることはできないためお待ちいただく必要がございますが、何故処理に時間がかかっているのかを調査をすることが可能な場合がございます。  
その際には処理に時間がかかっている要因の調査となりますので、緊急度 B として弊社窓口時間内 (月曜 - 金曜 9:00 - 17:30 (祝日、弊社指定休業日を除く)) でのご対応となりますことをご了承頂けますと幸いです。  
  
  
---
## おわりに  
以上、Dynamics 365 Finance and Operations のサンドボックス環境・本番環境に対してパッケージ適用を開始した際に、LCS 上でサービス提供前 (Pre-Servicing) という環境のステータスが数時間続く場合がございますことを紹介いたしました。
より詳細な情報が必要な場合、弊社テクニカルサポート, Customer Success Account Manager (CSAM), Customer Engineer (CE) までお問い合わせください。
