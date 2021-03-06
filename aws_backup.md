---
layout: default
title: AWS Backup
---

# AWS Backup

## 特徴
* https://docs.aws.amazon.com/ja_jp/aws-backup/latest/devguide/whatisbackup.html
* 対象は AMI, EBS, RDS など。
* 費用はこのサービス自体は無料でバックアップファイルが S3 の費用に準じる。
* このサービスで取得したスナップショットをこのサービス以外の画面から削除できない（削除防止に役立つ）。
* 実行日時は特定の時間帯をスケジュールするとその時間内のどこかのタイミングで実行される。指定時間きっかりに行われない（手動であれば可能）。
* 一定期間後に自動的に削除することが可能。

## 注意点
* 特定のポイントからの復旧が可能。通常の復旧と異なる部分があるという報告がある。
* AMI と EBS を同時刻に同じサーバーを対象にバックアップしたところ、片方が失敗した後に再度バックアップを取得して成功した。エラー時に再取得を試みている可能性がある。


[TOPページへ戻る](./index.html)

