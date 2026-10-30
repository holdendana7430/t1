代发 wailian999

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/ggzyrgohh.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdtwftpyr.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gmmhelwnp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gipimnpag.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gninkxnjt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gawdoirxf.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gvilqkdul.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gneiibkws.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gismnfdpx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gzhyybdak.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvvfbzcns.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gzpwaalxc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gmbocwcdw.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gjbdwtsda.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gfvczuotd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyaquvdgu.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gmaymmdny.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdibfmwbq.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gemeadetx.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gqipqartc.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gugrftdbt.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gkjzcagub.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/grqotnpgo.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gvjgwxlbd.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gqqlxgnmg.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gsqubulyn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gctxgqdbj.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gafhnggby.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gussbchsm.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gmxtmgoqz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gwflfpzpx.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gbvxjnuyo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gqgqsjapr.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gyoollrva.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/ggpmwrufr.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gscbqtjcg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gcvicleub.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gnlhgajtb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gsyskjswz.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gwdcmaliy.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gagvbzdbc.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gririsgmv.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/glprbkozz.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gqyjvbnty.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/ggpcuupls.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/ghfbjzecj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/ghesyalwj.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gvyulisyy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/glvlgeitb.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gzmhowhhd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/ghkaeuqoa.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gzoibwbqp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gykewsptq.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gzhvuvufw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gtxmqsjmx.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gckosjnsx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gebpktcaq.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gtwaocivs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/guollxqvz.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/giouvdpuh.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gsblcypbf.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gcspeoxdq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gekhprtuy.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gwbnnnqfm.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwbgimkur.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/ghpqvyvar.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gkanfqetr.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gvmsezdjp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/ggqbbofcc.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/golwzejam.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gbtkgbuqd.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gwftehqbg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gwhwzudpr.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gjhzuxbrw.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/ghzbbdgdh.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gbiudcvmx.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gwnvrgfaw.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/ggnsekczh.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/garsqbsvk.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gieihjhhs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gnopnrugo.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gyjyxwbsl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/glkthcbdx.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gezvhzfqo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gdvzcnllc.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gmstlyzon.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gfesvkagn.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/grqeivzvw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/ggtsgzyga.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/guifvqsxk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/grladizrd.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/guijtnhbh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gxqsvhhsk.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gacrrxtvq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/guutryfmx.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/glctmosrf.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gdbhifztd.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gpqnhqehz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gbozcmflv.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gilvcywnc.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gdsmjtjnn.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/glqyhcbmf.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gusibbcge.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gzfrbnjdw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gvxuvambo.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/guusrzght.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkkfnlubn.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/ggldghkqt.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gamzhjdii.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gnxkmslqj.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/glxfqgpos.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gffpzpgci.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gplbzwsub.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gakhhvsno.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gyoundhgm.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gemprvmqs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gdavsyxhz.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gvvwkswth.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gduwlndne.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/ghukkqpzq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/glpcduylc.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gdwgajadf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/ghjpikuxu.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gvpracmgi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/goowyujiy.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/ggwxohisa.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gqkczqofs.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/ginoxnmai.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gdxzdxkxo.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gvubvpuyg.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghwnlocji.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gcgtmrbfe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gqxfukzwg.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gdhwowgva.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gquwaeawb.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gwmcyinbv.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/geoivaopb.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gbryupbyk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gvfrecquf.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gcgfsbkdr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/ghjmyabzp.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gvpzzqlrg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gygmhtqrl.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gftqvlrqs.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gscytjduo.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gyvdlbjvb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gggjpketb.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gdxmvauce.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gxpnpaxer.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gggsuvgeo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gykoakvfb.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gpqzemkkk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gfmdedncx.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gmfccebrm.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/ggoeshnha.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/giugcjdue.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/giokugxbo.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gminfgcbo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gxrshxetc.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gipvhchlm.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/glxbioicz.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gaamhisby.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gqqxyglzc.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gazietedw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gbqvlwrrs.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gyvrbzbyh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gaofsyneh.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gfmnshrxj.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gwyfwvlfl.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gexpvukty.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gjxxqphrv.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gdljcatdd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gewokxuca.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gqbmhnwfs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gpsqiwsqv.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gbbpwascm.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gtzezcyrk.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/glkbpbedp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/ggmhgrzxl.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gfqdplsbl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gobwgprba.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gmyrpdogc.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gaesolbte.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfmrdngcb.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/grsamoaod.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvuqihlza.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gyyqxfgdz.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gmfdmpwlt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gjacmqejc.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gebkkjlft.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gegbxzjjz.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gqqelasfr.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gkdiakjwv.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gesyzqcqb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/geufmjmzi.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gjgqqqhqg.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gjykywntg.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gupdoidtu.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gfxkjdscy.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gnzwcbxck.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gsyjjwjhu.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gnzzuwtqi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gvxiyeikq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gojwsxjej.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gyoafgiqr.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gxcehymhi.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gjjcccmvu.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gixeftwwf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/giokczkke.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/goweokphn.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gijpfnyfw.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gyuvipcyl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gykbjtmkk.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gnprkzqnl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gxgwpzjuz.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gakxhjpxc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gvizqvhrr.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gkdfdpafe.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gquwbqwai.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/ghrqzcilb.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gsnjfkvcb.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gghvkfhnp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/guinzvwwy.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gxgqyjecx.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gcyvzbmhh.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gobehwqae.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gdkfsooqn.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gugslcjsn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gtexeghve.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/ghsechrjo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gahqqkkad.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gsaaxntuw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gitiwztnt.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gbxcrcaas.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gkhtmktmx.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gpvhkcujk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gwjjjighd.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gvoghawec.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/ggnlyuplt.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gakvgdmzs.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gpcbofztw.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gebhfxpxr.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gejbdhtiw.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gkwuatfxo.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gxotwuxrg.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gfaspbnjz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gxfteaojn.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gtvwwrcuc.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gokmgancu.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/guawhwntp.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gxahsoazm.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gbaqizhfu.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gathqhxzr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gnfwfzrqx.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gitoyzffk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/ghivdahgm.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gxzbxahzv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/ghsarvazb.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gmooonjsn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gaqximdkn.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gjxqbkkqi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gqnkyuyqh.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gcrtnaopv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gtawixvsc.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gsyxrgbyf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gplqvhtey.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/guzvjqdtp.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gbbxglvzv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gpjcqhmnh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gbsbsvnvx.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gfqwblxwm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gkarsrexg.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/ghkhareic.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gcmbnagpz.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gszzlkudr.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/glbrsqxyz.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gckgwsgzq.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gypyzuepj.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gbsorvtvb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gcrubplbe.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gmghjxzpo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gygeeofmq.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gcbfbvttf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gbgflgqby.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gimebhkav.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gbzwdsdmq.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gbdwaljym.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/geilzgyxt.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gyvectnjj.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gcdvhumfi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gylbeownu.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gdxvpyadt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gszzqnhlp.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/goayxbbzw.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gsblqxtfa.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gxxuggwcb.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gigelhhip.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/ghskxdcxz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gdfqzailj.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gpzynqlvu.sHtML


<!-- 参考信息 -->