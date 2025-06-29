## 自作問題
p766
- BCCとbpftraceの違いは何か(p774)
- memleak
p770
- offcputime
- runqlat
- tcplife
- tcpretrans
p771
- argdist
- funccount
- stackcount
- trace
p776
- bpf-perf-tools-bookリポジトリ
p781
- bpftrace -e
p782
- bpftrace プログラミング
    - probes /filter/ {actions}
    - BEGIN, END
    - bpftrace -l
    - 組み込み変数
    - スクラッチ変数
    - マップ変数
    - `@z=count();`と`@x++`の違いは何か
    - sum(), hist()
    - あるカーネル関数の実行時間の分布を調べたい場合どうすればいいか
    - interval プローブ
    - bpftrace -lv