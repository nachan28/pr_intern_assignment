# pr_intern_assignment

行った改善

1. MySQLのcommentsテーブルに新しいインデックスpost-id-idxを追加した
score: 0 → 5986

2. /home/isucon/private_isu/webapp/ruby/unicorn_config.rbのworker_processesを4に変更した
score: 5986 → 8404

3. /etc/nginx/sites-available/isucon.confに以下を追記した
        location ~ ^/(favicon\.ico|css/|js/|img/) {
            root /home/isucon/private_isu/webapp/public/;
            expires 1d;
        }
score: 8404 → 10098

最終スコア: 10098
感想: alpを使ったアクセスログの集計やtopを用いたモニタリングなど、パフォーマンスチューニングに必要なツールの数々を知ることができて勉強になった。
また、ボトルネックを見つけてからの具体的な対処法をごく一部ではあるが学ぶことができた。ぜひisucon本を最後まで読んで更に理解を深めたい。
