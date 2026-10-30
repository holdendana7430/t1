代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gewfkgprs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/glxmpmwir.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdmgujssy.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfxecmfn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gvklozcig.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/grihqghxe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpsivhug.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmnaxgao.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gnyfdsmmz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkskynbyu.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/glqotusxw.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gueaanuzz.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gwevgxxdd.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/glehtrxpo.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gdyfbofob.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glfxfzdju.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gxlhhdkfj.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagykzvjb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqojnpui.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/garrugqbw.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gosflmmnn.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gskzgxyqu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glxhtgadc.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkxhavygi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/guqiqlokb.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrnnpvfs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmratyie.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gircjgueo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gmstuaenr.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnlhxskq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gvywhemxh.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/glcrvhxsq.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gdirgoiaf.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtbkvynl.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gshnafauy.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gpdyvwlvl.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/ggolhprvw.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcxpyvjwo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzognwsoi.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gaghgaamo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grvxdhujl.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/ghvivkzbx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxjtoxrtv.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gogutzeam.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gswjsegkk.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gxzgimhtg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtkdijkez.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkkxpflz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glpfkasdb.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrbmnffo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvtprgzh.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjoognero.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbojcrefx.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gmfrjpxdz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhxlgwka.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gshhcfdce.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gecaapmaj.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gecsxaibk.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsulwlhmk.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gixwaabcj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfefjipk.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gokausrsv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goizunqtk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewetvtbm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/geihjvzxf.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gyavgrpor.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gwpzmvkaa.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gqejgwpck.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gufvibcde.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gmahsdvkx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqrkwwzc.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkmaxzcm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gcxtxirce.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gufifqkli.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnmgidwk.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtahrhihd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/greprvzpg.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gbcdstmit.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gllolpofd.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gcwveijuj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gfjdydfnh.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gozhscehn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gdtkntylp.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gvcitugae.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gzefacuqv.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/guzqyshmb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gkgssuvvw.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqlwhfnlc.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghedqggii.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/ghttxvhha.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvpusoue.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gpykoimwn.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gtwbsrahb.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxekspixf.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheqaojai.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrdjabns.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsfkjbfo.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpcmmnrt.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsycdhjm.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghatpfdfm.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgckvvun.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/giubjxmqo.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdaggiue.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynwotfni.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghslfdrzd.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gcymeczpf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gueshidrq.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwyuyyip.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrssnmkc.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gquedttzz.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggxqmudes.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbhuvpho.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gikdfilqh.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsbysewk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glbelryuo.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gifbcowht.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/goxbezgtr.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjopjljrj.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmvjfzhg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpidpcrza.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gdvtygdvz.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgqkqrjm.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsisetwwp.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhdixdca.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxkbvuza.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyhwdzqd.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkljpkkg.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gtqvbbclf.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gawumxeah.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsicdpjpi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkzvcsqc.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gyimqaxwb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gnotucvnl.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ghsrvfqnx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/goziawypd.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gygjmgjbl.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gpsrffpcc.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gonkuntkx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdpkidcr.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwgwtkoy.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gprtkptkd.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gidxuhgxn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ghyvkutcc.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/glnmtpxik.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goffqhhsa.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gjecckxrw.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/goyfolvdk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gaacwtrvn.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gmctieasr.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzpgkwbu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqeavdwz.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gcimefijw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gufuvedsu.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gyzrejklj.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gxogrccva.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/ggoukggqj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/govibmyfd.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gbmlhapzl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdhojlidv.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gmwfxiejm.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnstwxltm.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gkxmluwkj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpcrpina.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghjxbhrpq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcccubecj.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpqkmozi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvjbwuep.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gfarzoksn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/genfqypbh.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqeogdqj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gastycmse.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfpwgjnr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/goswzoygg.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gtdjidxps.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gqaijnvlb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gowkvoaaf.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gsrlmmzkd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbmxnhitd.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gitppxril.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gkigegpks.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaakwmxlk.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmjxdxsl.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gtqiepbmy.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/ggzotaqmg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/grlegrzsh.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gabmxydzu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyalfxag.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gyewiznnl.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gufisvwtu.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gohmspbhz.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/geuikpjnw.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/geimxawez.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gprpkltks.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxgurxlk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gxccglald.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gwzlualmh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gvqdqerpt.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gqusubqep.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtuvnodi.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvapwktwq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gjxmoapah.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gbjbtfxsr.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gvzafwbrz.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glroxzwok.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gipbemkid.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbeibhzc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gowpyqphn.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gqebcthai.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gejjcvaav.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gneijiqkc.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtkvygdq.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gmsaqumbi.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrxoskht.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsgoepxt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/grbvnalbw.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxipmiesn.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gxndczgtb.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/geloxncjr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gcuxxyoid.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysthbntl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhglwdcb.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkklnubd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gidesjesf.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gevfhekhv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gnexrpaqe.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gqneborod.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gfhpafmbz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgcvplre.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/ghrkahpbh.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknghhexy.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjasxnwb.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gpvpfjrrz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpjjenpd.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/ggbinzbhf.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gorzngzph.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpkxyhzyv.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlmmoylu.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkzwxrntg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmfivpqd.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gwcheeacs.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gheaibugh.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gpodlymsg.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/grpfobpvu.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geszwlhds.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwarefiqi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfckkeots.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdgqfzsu.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/grvqggoax.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gvmitrrjz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkwwajyl.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtnlhoxx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqpzfveeh.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/govptcvtb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrkfnlyi.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgppjjxc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdytfnsf.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvjnuxva.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqtctgdr.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbnegxxj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbwcwult.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuqejbra.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqifxlrt.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnppxntu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabqcqmix.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcjsxueo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/glwdmfwbz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxfdtiptu.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gaipbgubp.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gddlwdvpo.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyygvetcj.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxudcbez.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghxprgdt.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gidstajrl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/glyfkwqgj.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gijjlnucs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyviirnxm.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gjqwagzok.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gurgtsjis.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gygompjiw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gasmqztmv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitjzibwe.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpifkgzic.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gsajhhvzu.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gqxildedk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/guoyqwfkw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gonrwvmpk.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gjdrfjwyc.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbzrxuzv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcalyjpxl.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/giheqktgy.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/glvoimuzr.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gxoucexnc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwomqfns.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gfyrmmeit.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gvciolalb.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gcvgerurv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gooavzyiq.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gufyzgcok.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ghrjdkxqj.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwxlxpkd.sHtML


<!-- 参考信息 -->