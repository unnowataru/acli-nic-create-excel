# ACLI-NIC-CREATE-EXCEL
ACLIでNIC追加自動化くん

## なんだこれ - What's This?
Excelファイルです。ダウンロードしてご利用ください。
Nutanix AHV上におけるCitrix MCS/PVS環境でNICを追加するためのACLIコマンド文を自動生成します。

## どう使うんだ - How to use this
Excel内の黄色で網掛けされたセルに各環境ごとの設定値を入力してください。
CONCATENATE関数で文字列を連結して必要なACLIコマンド文にしてくれます。
仮想マシン名はacliの [ vm.list ] 、ネットワーク名は [ net.list ] で確認可能です。

## なんでこれがいるんだ - Why this excel file
Nutanix AHV環境でMCS/PVSを展開すると、仮想マシンに接続されているNICが1つに強制されます。
仮にマスターイメージにNICが複数あったとしても！
ちなみにこのAHVの挙動は"By design"と聞いております。(2019年12月1日現在)

手で数えられるぐらいのVDIならそれこそ手作業でNICを追加してもいいと思いますが、
それなりのボリュームになってくると大変ですよね。
ですので、このExcelを使ってACLIを連続的に生成してしまおうというものです。

## では、よいCitrix on AHVライフを - Enjoy your enterprise cloud !!
このGitHubリポジトリはNutanix Advent Calendar 2019 (3枚目) の12月1日分として作成されました。
