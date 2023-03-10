---
title: Cosmos DB 基本情報採取
date: 2023-03-10 15:00:00
categories: [Cosmos DB,情報採取]
tags:   
-情報採取
---

こんにちは。Cosmos DB サポートチームです。

本記事では Cosmos DB データベースアカウント、もしくは、データベース、コンテナの復元リクエストを弊社サポートに依頼いただく際に必要となる情報を案内します。

なお、意図せずデータベースアカウントやコンテナを削除、もしくはデータの削除がなされた場合に備え、[継続的バックアップ](https://learn.microsoft.com/ja-jp/azure/cosmos-db/continuous-backup-restore-introduction) (ポイントインタイムリストア機能) を利用することで、弊サポートに依頼することなくご自身で復旧が可能となります。ぜひご検討ください。

なお本記事は継続的バックアップを有効にしているアカウントは対象外となります。継続的バックアップを有効にしている場合はご自身で復元作業を実施ください。

# 復元リクエストに必要な情報

1.Subscription Id:  サブスクリプション ID

2.Cosmos DB Account 名

3.Database 名

4.Container 名

5. データ削除もしくはリソース (アカウントやコンテナ等) がなされた日時。できる限り正確な日時 (UTC)をお知らせください。

6. データベースアカウントの復元かもしくはデータベース・コンテナ単位の復元か。データベースアカウント単位でない場合、復元対象のリソース名 (データベースおよびコンテナ名) をお知らせください。

７. 復元先のデータベースアカウント名。なお、指定がない場合、復元対象のデータベースアカウント名-r1 となります。

# 注意事項バックアップ保持バックアップ保持期間を過ぎると復元ができなくなるため、データ復元のために弊社サポートに依頼いただく前にアカウントのバックアップ保有期間を 7 日以上に増やしてください。

# 参考 https://learn.microsoft.com/ja-jp/azure/cosmos-db/configure-periodic-backup-restore#configure-backup-interval-retention

復元先のデータベースアカウントは対象のデータベースアカウントと同一名含め既に存在するデータベースアカウント名の指定はできません。

他注意事項は [FAQ](https://learn.microsoft.com/ja-jp/azure/cosmos-db/online-backup-and-restore#frequently-asked-questions) を参照ください。

#NoSQL #MongoDB #Cassandra #Gremlin #Table#情報採取