代发 wailian999

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gdcoakgsw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gfffktjwo.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcicrmtko.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gnusgfbmm.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gyqrzblwh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gibqzqcke.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gabwxoeyx.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gbgsnicpt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gckflwbeu.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gynqtbkcq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/grzgubcax.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvykkejli.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gpkqkenxd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafvntrwa.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatnpfnds.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gozczbwjc.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqfrzfap.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gfzygjlzh.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gyqgmreps.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grpfyshwr.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gdimevsgv.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gzvxtekpb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gfbipmpdg.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gcyjktwau.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gijccnzlo.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/goduqleks.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrvxkuup.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxvefkuto.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggewuufrq.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizfykkxh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxumuiqu.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gyzljqcrn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gprnrfwnp.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/grfowhigq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgnoxkpn.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzqlpaky.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gdijldkgc.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoywsljp.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goemekhxo.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimudryih.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/ggswpxwfx.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnigyzwii.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grfovgwzh.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsfprhph.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqyqeywr.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/ghnfkvayn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnxqnitt.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtagscsos.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdascrkgn.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgoyvrlo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gydewljub.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdubjndgj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqozbmfb.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/ghlijxpgc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsptncidi.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmbtcbnpp.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyjhdaek.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlphydup.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gplhymbck.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkgawusy.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlowlokf.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/grqdlkpud.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gddlggpdc.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkybjokks.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpegurkd.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/glielehlc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaapurvdo.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlyhhpfc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gitgsibvk.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrbekfek.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyatcihrl.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvlxsgcr.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcezuupif.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gzbeeecly.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaylyrlja.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbjdpdar.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gmyxbfghx.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/glkxjkncf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/glxiecrrs.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvndyndw.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtgxkmpr.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gclniqitf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gavnrikkh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/glrabrzjl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gjimftpmb.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gwvegjrcp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgrwstbh.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhjpzdbh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gituxhhof.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gqxgeitwk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gswrismdz.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdigqniga.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydmpdgrz.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gcsqqldur.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjldqvij.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbpybbqz.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gcegdpslx.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gfluthate.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gsnwyjbxp.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/guogtuifa.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gqavrjtim.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gndslqanr.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/guhdatsls.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghnrqhywt.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhmihdvy.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/grjckfgex.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gvtmmdonc.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzazpuop.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuahspla.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gzymlxsux.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuxuxavb.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/guohfmsfd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzficzpir.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzbgjzcd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvxotdwe.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzejcjdn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gnvzjktvc.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gbtyiesln.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gavjktpfu.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/ghswtyabe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gytgxlbpc.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnythudvz.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghxeuihbn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdwkhtyj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsbnoitz.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghqixczhu.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxubmugft.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/geskxcupv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjtxyfnv.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gojavnoez.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gzptogaij.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysaazfms.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqczevuo.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gutfwcake.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeybzejw.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgzkbaso.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gehiftwqk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjemmdalq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchmtkcrp.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguxiixvl.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gnyoiufho.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsrtlvmb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gcagrgtqu.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gccizqrhl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgnurdtj.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gogtkmfwl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdzidsew.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgbruptk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gubohdadw.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gqjasdrsa.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gmfdleekl.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gomkbtfri.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrajqvap.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeafzpcn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjlxbyoo.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfaannjl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwfmrfyq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykksgjbf.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcpzddtt.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gohckndnw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gttwchudo.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggflqsojm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyschdpzh.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gbtobkxmu.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/ghhmecoqg.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gydpjunnb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazsatgms.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpjccnxe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gevdfgunu.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvweerwy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwqcocwe.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graatczvp.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvnoqelq.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gkhhsbsol.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggjycfdbe.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtovsstq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvtdervq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywnaywrj.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gwvcagiqf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guugaihbw.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/glnuraexl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtgfyatcx.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gsflinxpe.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajvmubco.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrvxsatb.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gyzmahdjg.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gukynxjao.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gmmbvqhnu.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gisaytxwb.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/ghluunkjh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqckdofej.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gomouqzjg.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsessbzz.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvireosvr.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gjxleigwx.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfkmgxoq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/glsucogjx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gqqrtscuf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gonvqlxef.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gwihsxdci.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gbqbbtpyf.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gagsydusb.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshexsypm.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyoezzsp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngeoyncf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gbxeyrkeg.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gqjqhdepz.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorqqwdyp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoaqhrwt.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmvjpelx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/grzjjjvhf.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/grxmtlgin.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/guszwtowz.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gexbkyuot.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuhzjqnh.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gamfimwlg.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzcptvoe.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gxqtyyqyv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdkqxyum.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gmornervr.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsobfjccu.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/ghfxlewib.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgbkkbgb.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gfqqpmljb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcytxpdg.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/grwoccbfh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseaacuyf.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gklrtxfhp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqzzcbdv.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnswcdkut.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gazubrgli.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/glwsfeqdh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gzhiclqcs.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gaeznxfbz.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhuuvsxf.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/guockclzx.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgoncabd.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjjhpmss.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsnethcx.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcdcivjcz.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gcgscrdjd.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/grweqskup.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gpbfnngys.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gplhsmjip.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gdfzydqht.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzbqxosi.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhtsnkoo.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyjipgnk.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gvmxnbugz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdeyrjeb.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbixxsdju.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/govoapgvs.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gemeiular.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjztezzqw.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gacwnhnii.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghalkuvno.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gwvlbhdwr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeshrodk.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/glgelfeqa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtchocti.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxwebbtt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gutgbzvyh.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjxjzwei.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gsjgihebu.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/geozcdyxw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gnjxcxgtg.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gzwxoxqfw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsehkfrvm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxplsieh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfclxouq.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gagaorgah.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gzrutwykp.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfalcncfa.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gwtcxaksr.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgnbigsj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gstvamgiw.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gtunlzyrj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gegbnwepl.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gpogpufwc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/grsygirfo.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/glwucjjyx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzxhpxvr.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtbuvdib.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzozbeku.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfgkaybj.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaaecmql.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gxzoqhrek.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gndrymbro.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqefzxjyx.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gnpmwfgug.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/ggextlzwr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsnunbjf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvyusimbg.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/geefdhpfs.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjercxpqo.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goivjzwax.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnoxyjes.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/guatitgyx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gicoaqiuj.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmqowceh.sHtML


<!-- 参考信息 -->