代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gdxmmypeb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrkuhwsj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvyuizpds.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/ghjralylw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbxikclm.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gpxszpcls.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gthwtbldg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnlshycc.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleyxjemh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxohrbypg.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gpeybvoya.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxkqtnnl.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gzzubfdxy.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/grorgdpsi.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpewouxe.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhapmqqi.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/guypyahmz.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gweownojp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrdqewkr.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgjcdxgu.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpmgfbgs.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjgcgzti.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsqctzcx.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmjfiojex.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gmcjgicjv.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gddvkbevn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeqbfmzu.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gicvdqpfe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrqsyowk.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gtzzixfgf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzcgmedf.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpzoigmj.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowwshczr.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckpidsih.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukvyzcsd.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbckyica.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqmvgdyr.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gttmbnlux.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyqjgtif.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/grzrfzgzj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvitfcbpl.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gscquarug.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsokpleh.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gilrzxpch.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfrsigvu.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxuzxgcs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/glppasboh.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gijqvlqbp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgddftfc.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gamapxvjt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhnuyrlg.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpzsnfal.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqxvvcol.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gxrlydmbc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grqpspffq.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gcarypntq.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpedsswv.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwytsevd.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/geoqdnhqh.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmmwsmtta.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/grqtrxoak.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gjjurwlwt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjgvaazn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gemwqsyxw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyklrics.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gevavswyo.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/grnzsqvoq.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/grejsqqxc.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gexgzcdga.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfbdkjvv.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/glrxdxggc.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/giqgkaeyn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gufseygxr.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpmctuwk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gcjuzrhag.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtdpaztxt.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gimslrpxu.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gmvguykiy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlcoagiw.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/galagsejk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gmisokofe.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gyzdwopgu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gebemeykh.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gvshtevss.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyvnsdfd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgjnevce.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gippmcnbu.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydpgovzg.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gdhhwsedj.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghauqbzeo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gckladqxj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gyekanems.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/grcpfollo.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqqvultb.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuxhbqrq.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gjleohjiy.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gfmclqzwl.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gegdmqett.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpguedyta.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuueuntr.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ghhajqecz.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxlvgxbp.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqattckn.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gcedtfkin.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/ggsxuliyc.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkctngnaz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/giauxoiht.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/guhwleqvq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqurelyyw.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/geshnaaxy.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gckldeqgc.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/guavyeyss.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gglmdahhk.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gsvhjawkr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvhpikjrz.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gfghbgkcl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/glkfyohid.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqppoouvi.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcqazhgl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjelrbpj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/glbeufjxa.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gthvnodjw.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvtekpeq.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gimqxkywm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmjavzmt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbefuopqf.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gjdvuutzb.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gorrxvqww.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gdxurhwek.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/groaylbft.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gzkzigohd.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gsoyunbrs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/giefthunf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrlpesxe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsfzarwk.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gqwraufwh.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gadsytgft.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/ganzlzvkw.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gpjvywvtp.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhhegizn.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gvmktnwbv.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gqikntiew.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gutxfrxfy.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhppqaqr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/ggopnqoxw.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjazkaxg.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuuctgls.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzviteda.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gukbaswup.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtmtfxbf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmyljdydr.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzhycodz.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gagaardzb.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gqqbugqif.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gzfyaszba.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwovnwiv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gsodzgolg.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gukksskis.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuymbyxw.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gtjpcntvz.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/geekurisn.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdtomidw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbvktcpe.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvqsmeip.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gnienrtef.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrybtpxw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqjtqxui.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gbofxkxjn.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gceacbeqy.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gwnzqdjrg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gceyfepyc.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gmtfuvagc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/geqtxmxer.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqreihnu.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdytipnot.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiuebroo.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtmtqryz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxdwbqlt.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gavgksfaq.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gyhhecrlo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasuizsbh.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfvkdcfv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gheopcjey.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gtctineql.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/ggjiuwihz.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gimpcgzwm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/guxffcmva.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvqicels.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzbjpkuo.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/grrdjbvno.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gntiglver.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfjigzzl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gbstyncej.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gyirdhbwu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goptxhfbg.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gaujhvvlv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gyivqnwxe.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexsbbksz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gajlkqhdk.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqmgstyqv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntzvtwrg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/graxgwwjm.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqebumjxz.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giezdyvkh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwflvspzj.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/giwyrpqzz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gviezhhvs.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuyuwsnt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gwuqvuxxt.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoqdudyl.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/goqsczdpm.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfyciaec.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gppwoaoqq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqhjanyi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuvyosud.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcrascwr.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gprbjxqci.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gygaffwto.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gqkgswuyi.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gmwerudef.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbszmgvvr.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gccsdowkr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gtwwgnrqg.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/guhjrojcq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gqcaastqa.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlwhjlqe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgapmvhu.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gtxxzfjap.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gatnuvxfm.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsuqfxap.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnzykvdp.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/guwugthlh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gagyorzmd.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gkxilqqcq.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/grsyucgvw.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjwsvitu.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gawvyebee.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkzhgvwlg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwcmepma.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkojqzhbu.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gzameywqu.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gujatqekj.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzylmrqao.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtixuccl.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gziekwdkk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjfvkehf.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwtlwjtz.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/ggpieefcu.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/glmcvtils.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxqlzdic.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gillmtsow.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtzoqmldm.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuqnzdvm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gnytlxxxo.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/ghvobcedl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gywqnsrwm.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gpcslttlt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gmugzcebb.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/grfnocjue.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiycffra.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/ghcnmlgmj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdehsxqp.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwihzyady.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/guplfcuye.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gexftdzco.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/goudyriwn.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gupczgpyf.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gwzcigzps.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gejwmsars.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwhidsws.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/grqltrhrg.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gslssqyff.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabcuufjz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvykgnst.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvrzghnm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gudafdivc.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrqxmhut.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvsoifksm.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/grwtbxntw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmdqckjp.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuuyyqkw.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpakuslr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gyouswxag.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gjjchrnkr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzifvnmh.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/grbepppjt.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngvzyemd.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gwvrsyobo.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gprmvfbcc.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gonzlwyht.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/glujhhraw.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gqqljhiiq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gffspbkir.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjysnrzf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gylwclcmo.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqetozdaa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtmxaoyq.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/ggyrhjzvl.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gcdvbmgtr.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtrcbriz.sHtML


<!-- 参考信息 -->