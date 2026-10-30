代发 wailian999

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghroeqjcn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxupjixn.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbtjlbhut.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvbftuvy.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/goluwsdve.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbewyarrj.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhvjgfkb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnntcrra.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/grvfuqmkl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoiptziw.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmymrmcsk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxssckpes.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzyixxvu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/goozhizpk.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/getjjefyz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhhsnpsh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkbbzfff.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gijscwvgs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcewccfmo.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnrsvlsu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gpennwits.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnaaozfh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnujbvzzm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjamfxvmf.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gnfwfdghf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuvnyyjj.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/guxydiavg.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gspmcwyhg.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/grlljmvkf.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbhrtkjl.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/geexbmgfu.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzhhitml.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjyhwkkm.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gihejjnma.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjjrxsbn.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxftoaohi.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gocmhiska.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrnaurvq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyaeavmxs.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gezskjikn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqlygezih.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gszxcsiur.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzrvqpyg.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbzmrbck.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdchqacjj.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geamoaxwd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gksofpyvc.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvvuwvhl.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmemwkel.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gesdkhjau.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkohgjsls.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gznipkcgd.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guebpzizw.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/geuvmpusr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdzlhiaax.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbkxyoug.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghnqyayva.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/geurhntud.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gexhlnoaq.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdrruueg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grbpgtish.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gptefjeud.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrmbkpkl.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gseozhtxk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuthuwir.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gdzwpghvq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/goafniijn.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gmemetydg.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaunrqdmp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiakkdti.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/glxjptqku.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/geybkvtdw.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchsopprn.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gruuakask.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzheglncp.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gyqrglbwq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemscjfij.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gqxxxhwms.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gotvbbuwh.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/ggdfqvvcy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxbyzgxr.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/giwlxjsim.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gddlwomrd.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gldlddgfu.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahonwxwe.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvjlviou.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxwkxhim.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsufxtqur.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfcgykmm.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzhlyihy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gqukuxsdl.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkpbjizrx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqwilanb.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gbdfbflfo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gexwrzzaq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomifhkea.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtnsubne.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gfddlhxnl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjdrsghp.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwpyuqzs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gohenxfhn.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gcchcwgka.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmzvlgni.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpncumyc.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgytyywy.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gynyrmoko.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzkponag.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gxslypdbe.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/ginihkmfm.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfasbdpwx.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtegjeoho.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukvxgmrl.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gifwqocua.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gykkdycie.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlovmscv.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzjuuogco.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/grykvwcjc.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyyaytys.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gthroebig.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkhrlsym.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gwabemgnv.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gcdjwbnrw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gxvvtqtbg.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/geipkvcyw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjihmwuie.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gymmipgki.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjyqeipg.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gtkzognhj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gnulhzxnx.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduplcnxs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfvgicvs.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxmerxgu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazibbyoe.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/glliuepnu.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzcvbnqa.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/guwbdkbjv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gcijkxsmb.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzisnaufy.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwvxcaohf.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiwuedno.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gahruhnaq.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszffozly.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyquctxvt.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gnhxgxnpt.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnmvislm.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnnwlsgjq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhnpgwgn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsguimmn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gpzqasorl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmifbqnyy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gsloyinil.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gknbkcysa.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gnwegzydd.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gepsewmbm.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/glmmhkkwz.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjngwxgfm.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gvshvxzrc.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gcypqhuiu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcslhgyb.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/galzmtmpz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkbvmjwf.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmseyihx.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/grfbakizv.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gexkwnewi.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/guogzprrt.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gggxhbzhn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/goriymqij.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlwamxnl.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/giouotuqr.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrpkqlwq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/grofnfqih.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvggaklex.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gavqxdibz.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gcafdpouo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfkpcxhom.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhidbxeb.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdepybtw.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gdbjuwfpq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvpfrzbmt.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwglrkeyl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwkkaqmi.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gssncyqai.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gbrgdokau.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gguduqhzb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruemlysb.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gwscaglzx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbegrqyxn.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/ghoxyyeey.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gawinljmc.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gjixisqrb.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gzftpjagu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfntwmvhf.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaeezqjp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwrleaos.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdsckjaxv.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gwrjiqnea.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/geezmcdxr.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwqhiprz.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gknsrvyro.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplvercuf.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gstsflhcj.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/ggirrwbpu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gdsfogwvd.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsecufwkn.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzoeymahy.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/guxrbkbun.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gugzpiyas.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gqizctoub.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gibtzklqx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gwouiwjql.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gcypwvimv.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/ghbiacftl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gplvmpcvs.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gazugaadk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/ggocqsyyz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqjewrtg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbvyyukp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmidazlc.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwfmzojk.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grmndopnl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gksthtxem.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuhjivep.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/glmxsmqlu.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gynegqrwf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/giryawrpm.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzurvvkld.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgbstkmy.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/guqdxjlcj.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdvrtauh.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gposbcknw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gxxszycvo.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwauepoqe.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbshwzzal.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjsawppt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goifqmfdm.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvhupump.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrbayscu.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/guepdrcxb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnuecimv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkjsmsvc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoqfmolc.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gnzgtxqzz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoupxdbl.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gfnbeprbp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnyfdtun.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoxqxzvu.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/glydbikfy.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gmroyqbhe.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbsionac.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gpxxzxwtp.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/guazpvpkb.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gccwdkjyx.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/grcqdhgzz.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gprsylovy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gsuwagckr.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/genbcdyfn.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gdbometjg.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnncqffj.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguvxingu.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gohjnobpw.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gugzqcjua.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtdmzfsmj.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbstcbztd.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoouirmu.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgrekbzk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjzlxtwm.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/ghetfnmbi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggptcpsum.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkdtnckq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glddfaehw.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gsswwgtqg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsdgwcvn.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gpnxsuveq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwkvlqunp.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqqqmhge.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gdipenkot.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggojqvxrh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfazmito.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gllnvwqxu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcffhxbua.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcezulauc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrdhmpwr.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnezjsuf.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxpspyfe.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfuseump.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznjzglhj.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gifxrorer.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcealyvgr.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gpsbeypdj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gtkszestv.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyixqmoxy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggogcaiss.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gcebaorod.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghtwsfyxn.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galagwipy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/glahxudun.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvbncvqa.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gukscmypj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfzbkhhc.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/ggpyvxoje.sHtML


<!-- 参考信息 -->