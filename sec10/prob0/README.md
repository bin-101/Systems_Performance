## 自作問題
p514
- インターフェイス
    - インターフェイスポート
    - リンク
- パケット
- フレーム
- ソケット
- レイテンシ
    - ネットワークレイテンシ
- RFC
p515
- NIC
    - ネットワークコントローラ
p516
- TCP/IPスタック
    - セグメント
    - データグラム
    - パケット
    - フレーム
p517
- ルーティング
- ネットワークスイッチ
- ユニキャスト
- マルチキャスト
- ファイアウォール
p518
- カプセル化
- MTU
- ジャンボフレーム
    - ICMP
- TCPオフロード
- ラージセグメントオフロード
p521
- TTFB
- RTT(ラウンドトリップ時間)
- バッファブロート
p522
- オートネゴシエーション
    - 二重化モード
p523
- ポーズフレーム
- loopback
- IPソケットによるプロセス間通信とUDSによる通信の違いは何か。
p524
- IP
    - DSCP
    - ECN
- TCP
    - スライディングウィンドウ
    - スロースタート
    - SACK
    - 高速再送
    - 高速回復
    - TFO
    - TCPタイムスタンプ
    - TCP SYNクッキー
    - 3ウェイハンドシェイク
    - TIME_WAIT状態
    - 重複ACK検出
    - TLP
p528
- Nagle
- 遅延ACK
- FACK
- RACK
p529
- 初期ウィンドウ
- QUIC
    - HTTP/3
p530
- インターフェイス
    - フレーム
- コントローラ
p531
- スイッチ
- ルーター
    - ルーティングテーブル
- 速度転移
p532
- ファイアウォールはどこで実装されているか
p533
- ネットワークのIPスタックの画像
- Linuxのネットワークスタックの画像
p534
- LinuxのTCPのバックログキューを2つ答えよ
p535
- ソケットのバッファ
p536
- GSO
- MSS
- qdisc
p537
- 割り込み一体化
    - NAPI
        - SO_BUSY_POLLソケットオプション
- NICはDMAを使い、どのようにカーネルと通信するかを答えなさい
p538
- RSS
- RPS
- RFS
- ARFS
- XPS
p539
- DPDK
- UIO
- カーネルをバイパスするデメリットはなにか。
- MSG_ZEROCPY
p540
- ペーシング
- TSQ
- BQL
p542
- ネットワークのインタフェースの使用率はどのように求めればよいか。(下の文章に書いてある)
- ネットワークにおいて計測すべき基本指標を3つ答えなさい
p543
- 高度なワークロードのチェックリスト5つを答えなさい
p544
- 割り込みレイテンシ
- インタースタックレイテンシ
- SO_TIMESTAMP, SO_TIMESTAMPING
p545
- ネットワークモニタリングの主要な指標を5つ答えなさい
- パケットスニッフィング
    - アウトオブバンドパケットフィルタ
p548
- QoS
    - ToSビッド
p550
- iproute2パッケージ
- ss
    - -t,-i,-e,-p,-m
    - limitedフラグを3つ答えよ
    - 平均スループットを計算するためにはどうすればいいか答えよ
    - ssは情報をどこから読み取っているか答えよ
    - netstat(非推奨)はどこから読み取っているか答えよ
p552
- ip - -s link - route - monitor
p553
- ifconfig
p554
- nstat
  - -s, -rs
  - -d
- netstat - -a,-s,-i,-r,-c - forwarded
    - 統計の元となっているディレクトリ 2 つを答えよ
    - 統計の意味が書かれているドキュメントはどこにあるか答えよ
    - SNMP(p834)
p558
- sar - -n DEV,-n EDEV,-n IP,-n EIP,-n TCP,-n ETCP,-n SOCK - 数字
p560
- nicstat - -z,-t
p561
- ethtool - -i,-k,-S
p562
- tcplife - -t,-w,-p PID,-L PORT,-D PORT - オーバーヘッドが高いか低いかを理由とともに述べなさい
p563
- tcptop - -C,-p PID
p564
- tcpretrans
p565
- bpftrace - ユーザースタック,プロセス名別に connect したソケットを数えるコマンドを作成してください - ソケットのトレースポイントを列挙するコマンドを作成してください - bt ファイルでコマンドを作成するメリットを述べなさい - soketio.bt - tcpsynbl.bt - 「キューイング規則とドライバキュー」をインストルメンテーションするイベントソースを答えてください
p573
- tcpdump - -i,-w,-i any,-n,-v,-e,-x,-ttt
p576
- strace
- lsof
p577
- ping
  - どのようなパケットで計測しているか、どのような計算をして計測しているかを答えなさい。
- traceroute
  - -T
- pathchar - traceroute と比べた利点を述べなさい
p579
- iperf - -l,-c,-P,-i,-t,--reportstyle
p580
- netperf
- tc qdisc
p581
- tcpreply
p582
- sysctl
  - -a
  - sysctl が設定を書き込むファイルは？
  - TCP 読み出しバッファの自動チューニングパラメータの設定の仕方を答えなさい
p586
- tuned プロジェクト
p587
- SO_REUSEPORT
- SO_LINGER
- TCP_NODELAY が無効にするアルゴリズムの名前を答えよ
- MSG_ZEROCOPY
p588
- イーサネットジャンボフレーム
- リンクアグリゲーション