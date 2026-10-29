代发 wailian999

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gmevznjqy.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/geiwmkwev.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gkudvwrwr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/girnlkwrx.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gtrrvqmbc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gsmnpfyhd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/ghnltenbq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gzhqfmbir.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gswzanmit.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gopelidbp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gslmpbbix.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/giyffplmj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gtptbpyrw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gijfripob.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/ghibwepmi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvorlbrcc.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gijsiuono.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwejjosak.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gjwfyedim.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gfvwpvjin.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gjkmqpacu.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gmlivulcb.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gxwcdtnuv.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gnpxdfstt.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/goizdwjuf.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/giifxmzvk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gnxupsyyj.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/glwglhgvt.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gtiqafqrv.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/glvlgvbsj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gqnybalfe.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gxsciehld.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gltgjcecc.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gqldhoroy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gpkriqzwe.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gsnftblpo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/ghdodrdan.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/ghceyniqd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gpjvkqqpg.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/grwqxxutt.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gblbbrnol.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gxoftuwxl.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gbuuguphv.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gdvxtaqdz.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gbjslcxqe.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gseglwlpj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmvtiybcs.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gtovhebie.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmscrbtsc.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gpqstktsb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gromwfhlb.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/guhtbjseb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gmgfxhewu.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/ghwkkcizv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gkprofxhe.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/grnpxbybg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gelppgqgy.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gzymvlgpp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gejdfmbts.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/goydklmyz.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gzqynbggi.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gsmgqndjm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gqqjuhsuq.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/ggeejtujv.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/getzxuide.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gbzonrpnz.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/ghsudvkve.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gflkhgjnm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gxmmzlqtz.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/galpsjeif.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gjsuqqspk.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gedcbnzvv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gtvewqcwm.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gutnbpvxh.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gylpftngk.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gevwrwmip.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gryblsurq.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gpeqwgysg.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gxavtjyqq.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/glqxngsnl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gypsoizia.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gyrfmbcon.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/grsiuanhp.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gvnhkoraa.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gvqbkbtkt.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gbxflthul.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gpvduihpa.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gfzggulan.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gwzlqifuy.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gzuvrzsqz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gfmvkmwnp.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/goybqrbqf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gcvsnfyko.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gsvaruvoe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/giwobpizx.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gjtjoxbhv.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/guuhgmamu.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/goplpmslu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gagvrksfg.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gbnlcjntk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ganzoydzj.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gcmxkviwc.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/grlpwxnuh.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gjvrrhsxq.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/glmbqivwv.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gfcfintdz.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxonphpmp.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gmpatznfc.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/ggjlgqjin.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gabqhvkhp.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gcyafdnkl.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gsszkplbq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gmrvhcbps.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gtazmpazt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gxwbebknd.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gspyleyxh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfevqwuds.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gziyqbzjo.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gxhloqxfe.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gwsmydqnd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/ggvxnoemv.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/goimdjwwc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gmqvwmulg.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gcbjqhvkr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gbuvzszwi.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gblwowlcb.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/ghcpqefwd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gavqlzqeo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gcnvffmsk.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gfgtkikfb.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gotvdvrsl.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gsjmivgtc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gqayovvta.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gxlitwwco.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/ggxdmayje.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gzafwmsvk.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/glolztvfq.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gvilhnuok.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gmzykjoef.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gniwtxldz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gumrelmwl.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/getmstafy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/ghqnwcgwm.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gvcexjong.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gyubhkxsm.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gibhbrqta.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/ghcpfwkrg.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gzgalrfra.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gdigwzjsx.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gcrikpeps.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqxzxzgv.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gfapovtkr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/ggrfwbkgq.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/guvenqeqs.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/grpbfcuyc.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/giyvwtqsf.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gctdaescz.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gcrypnpto.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gejruwbte.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gspeboopv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gkzbssiiw.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gnroisflv.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gngiqgojf.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gzkocxtuu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gjuhafsrr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gycpruony.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gcobjrjtr.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gtawwjhtj.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gulyiuyjb.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gefkhkjtu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gsrghwmas.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gaopwhngs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gihthrinz.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gofaooerk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gtuvplmuj.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gkgezghdg.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gxdikaezb.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gppjfqfzp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gykmclubk.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gvkepwman.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/golrglwey.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gdkdmblvm.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gynoyencz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guaogjgce.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gblnoadsp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guqfqymsq.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gkdzicnot.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gxnnlijbr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gktidxprj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gyofoxaho.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gvymubnpu.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gsrtjkwqn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gesvdiiwr.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gydsynfkj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gmxhjlthh.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gbtjpmmju.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gafzggdub.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gmlwgubvk.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/ghmxdtvyh.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gofqxifpz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gvpdyegmd.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/ghbnvtujg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gmkyjdxjb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gulfwmhwz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/geprdwhhg.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/grrhholmi.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gxiwuktlg.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gfthsylrm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gfrodhgwc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gopmxvrft.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gvojalccf.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gzjlntord.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/ginsyvqmz.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gtgytdoom.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gvbfcyyzb.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gbizznhrv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gxgprwnah.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gwtkpryxg.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gitnmbtdg.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gvuutshlm.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gkofwwvtl.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gsazuvwyo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/grkadaign.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gdddcggqg.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gmajyukio.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/guobgtnwd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gblubgmie.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gfqqcbcrv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gfociganx.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/grcdskxkb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gteqrdfiu.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/geeyglpnm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gmptpsbge.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gzhemgwce.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gcipivcgv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gpxqqbqrb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gmufjnkbb.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gvrylpfyi.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gjsxzuppt.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/glxafpkgn.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gubkkfpzt.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/glxvijtfy.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gmfpqvyis.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gqqhvmhdk.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gxdswkdiv.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gjsdxbifv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gunjvkkgq.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gtclfdjad.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gsztmolwq.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gneaqlxim.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gmnruhqce.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gzquhrivv.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gpdzssikk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gfjltequb.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/goviveuhy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gglpemcle.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gjffcsimw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/genqrfeta.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gkzrfcuya.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gdcfrhvja.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gafluunyf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gupcksvbh.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gmfwwjiaa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnszqpqyu.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gsyxbwpjy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gkjbqbzrb.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gbxfyrybm.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gvgxeqcog.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gipdvrubc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gsxvddomw.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gbosvxhoe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gbniudvif.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/giyygxdfx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gchyoamub.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gjeujtinm.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gxxquwaxb.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/ggnitgyku.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gkqngjryh.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/glyzxekwz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/goesuwpfi.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gguyhlblx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gljspmyzi.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gxzogufbx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gdytvekrp.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gqmbjlroi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzwolkxo.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ghledrtye.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gvvrjuykp.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gbfnjtutu.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/ghybaehoe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gopgwxgbd.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gyazvyifk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gvcpchqgv.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/ggggijyqo.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gxysftldj.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gbyfgzhtl.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gqtnumacd.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gfpjpejun.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gkkibzooi.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gepskwhxh.sHtML


<!-- 参考信息 -->