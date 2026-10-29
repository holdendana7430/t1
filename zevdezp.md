代发 wailian999

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gscouocia.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gtijlnrvt.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gbcexbhdo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gaueleqib.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gxlcxqnup.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gkpqiijrk.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gpfcczuby.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gpflwwtrb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gjkzubbkt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gqvokurie.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzryljexe.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/ggciumgny.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gstnogfmb.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/godpptwgy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gbheiozxc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geminhyds.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gbnxfgfkx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxfvcwxbk.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gscdnjioz.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gtigpyspq.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gidyfrpmp.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gjpfvvjjq.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gjjysjswn.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gqjlcbryl.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gybksrbjo.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/ghweiujrh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/ghfjopcft.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gsweryova.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gjhzeqoql.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gkfnaaidl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/grrcozjpf.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gvifulgox.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/grfykhcll.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gmcttghys.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gdacouupp.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gndahepzt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gbqhnxclb.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gkrunhktm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gsjyqkyva.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gntpetjtj.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gjggfdvgj.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gkfrerlkt.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gvjfkqmhp.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gaptedaou.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gvzbtbynr.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gojpkzsbk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/grzpplely.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gjzfwmjlt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gzbfqhckt.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gedmpfcgg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gaajezqvv.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/grncxaaxu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gdpezjvan.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gzxjqyzhn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gawvqzbcw.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gqmlriufc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gjodykyie.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gcsfdmkbr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/glehylign.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gsvofcuxq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gtroemhdd.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gdorhwitn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/ggihqocgg.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/glduvctdf.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/grzlxvjev.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gazxgftiq.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gsytubdgd.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gcwcsykff.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gupfeyowe.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gbdfrivpn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gmzhoclyo.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gwenoontc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/glxktndeg.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gxdukekgk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gkjpikwco.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/grnjoiuwa.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gmkzcnmls.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gzwcddhfa.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gduajomox.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gezjrjxzn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gjcgflydo.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/glzgiwrmx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gplxyrvwu.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/grwcbzfnp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtsnmgbrt.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gogwvolcr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gyztlwzvk.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gmjjvgsfy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gecncywlt.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gizfdiomh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gfseaatbe.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gqsuwamrz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gzhwebhed.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gymdlsikg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/ghedhhvas.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gykjgpaqa.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gjlzpauji.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gaeozryyr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/ggvcylydw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gjmkpxbjp.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/ggndbdoev.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/ghencikor.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gsyjasvbv.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gsjccccdy.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gklloercb.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gxwqljkpv.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/grkojjhmk.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gsjryhxyv.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gqhjsoggz.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gukrpoynu.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gngcorrie.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gdmcrsosm.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gbrevfiop.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/ggnnkvygn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/grvarprin.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gbzogclbq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gtdsvicel.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gsjdwssgo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gspbmojaa.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gusuckgvn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gvqmzrhwp.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gemghslno.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gpufypmcy.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/galdxbrvl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gylbumcwk.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gvqobenfs.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfatzjxlw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gzltygzug.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/grgscaekm.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gnwmzwpwg.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gmtqnmcxu.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gqfbqavuo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gxrxwmtyi.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/ghynplqkv.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/glziqcrzx.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gosrccwps.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/ggxzxfisz.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gvovznqbz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gpzdhuiiw.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gdbtzubzt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gdhztuyto.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gqlwfxvxv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/ghxcuqksd.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gasmniuep.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gidwqaroz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gidcaqccd.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/grfeeujhm.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gmnzdsesl.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gwqtmnjqt.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/ggvlpdcyz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gimkymnpd.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gxdpzwpsx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/griaqhqed.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gdvnwonxl.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/giplovlzo.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gnbgzzrca.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gclojhksk.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/glurohbvg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gvqxloyyu.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gkuwhwyur.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gvzsxpzpb.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/ggqbczsuq.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gumqqqqrd.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/guzworkmf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/ggrohsjud.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/goftpaevc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gbdvkyokk.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/ghomnmjtc.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gnqhyvmmq.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gxahrqfsk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gieflxpnr.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gyvumzcsg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/grjqrghsc.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gknelpsmg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gvjrlebbz.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gwgororqe.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gsjprujoz.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gzgkdssji.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gpzbdewkz.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gwdokeuaz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gxiugqggi.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/giwqwqkqq.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gxgrahmfd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmcpjvtue.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gbgtduiza.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxyuwzhkn.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gablmzuie.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gyhppnplp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gjoxjwwny.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/giyrdcjlv.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gnmdkxrws.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/ghpgmhpwe.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gjsvbgytd.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gzwqqiriy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gvagclxaz.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gzwbtryoj.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gzlktobst.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gighaqxsn.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gxyxhoklk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/ggpoessaj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gvctgyzkr.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gpptmpwmi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gyflzibpf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gcziwwjpm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gzhpegfve.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/giqmsnzog.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gqrnoarda.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/givabrywh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gzrjljglv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ggzohxyot.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gblwftncm.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/ghpeanpqz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/glptiaslq.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gfaiwkiyb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/guhsinzff.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gwgexsfzy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gickfowzy.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gulkyksyj.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gtxrdvoos.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/goffslxxe.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gkkpnncqu.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gazclxnwv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gpmpmivvw.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gqtcgcbli.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/ggemrdsrl.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/ggopbzpme.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gshmudwyy.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gsuexpyno.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gnkuintfl.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/ghnnimipr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gvadefhvx.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gyekcijut.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gdfakflpv.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gmkzxqgoh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/ggncpwuqg.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gloyykzva.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gfsdlnkrw.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gznmzxehk.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gakevupnk.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gbvjmrfay.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gujqhoyuc.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gjcstokfh.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gkeucwges.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gtbyvolnt.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gjopeqikx.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gggcupzab.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gomdscjyg.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gsuaetkng.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gtncoevzy.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gkupdwwjt.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gtqjfbhgl.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gnmcgkbmu.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/ghotjlaac.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/goxrfedrp.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gmalblkai.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gogkaiohe.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gmsvypvtd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gvfgsxsdq.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gnazpjdev.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gsdfbvnoc.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gtbdmsbud.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gxpoocdod.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gibgdhotf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gjpdgqhrb.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gdqmdwemo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gkgzmjsig.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gvookdtgi.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/geirocxbz.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gyifaycbh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gbylgxykc.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gjvakwcgo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gjptvuifu.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gsgltvkcm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gkvinlfoc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/grezotvvc.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gdsisoslg.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gblpockse.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gzpnxmmmv.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gghismpak.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gtemtvmze.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gzquyncbo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gvpfzbpjh.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gyfrnevvn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gqccoqnco.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gpafiwpsi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/giujdksih.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gxzosneta.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gmyyimssr.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/geardurqw.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gqcbicapz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gsrhdsixy.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gcivlupdv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gnurepnkx.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/ggbejuaoc.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/guzxjwmtx.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gsjnmtoyx.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gmlqiurcs.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/ggpwhvkmu.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/grvieympl.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gveovubkr.sHtML


<!-- 参考信息 -->