代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsjplots.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gcxtoamgv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/grgwznbfj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gspsqgeiq.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gzunnishm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/golwredeo.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmswugfp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gixasgunh.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gqohxtpqy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gehagrjub.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmgeegcv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgnbfpky.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnwujmcd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyycjarbf.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gkjmvcagh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcdswzzcb.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpubiezww.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzonxlytr.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwsiwydh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvjaeyvdn.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gyaxoyhpb.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqcmsercc.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgdxzpvm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcberjagr.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdbjxuah.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbmwzrvx.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgqrgkec.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gztrelvpi.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gwcmgftma.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcxgjtgx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxitmrsz.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/glmqufaqb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoymjwmb.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gezkyczaf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/glkifkyec.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgrzdwvf.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmowtrnm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gesweafrx.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdikdwld.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gddsgboel.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gphrlgncm.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gwbpqmngl.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/georrtgzo.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/geiftsvqd.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuagrbec.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcsquxxz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gjglqvnrt.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpjwchth.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvlgkzxhg.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ghgknigzd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzanrolhw.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkklmnfbm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqnaexhv.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwmtcdal.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/goqqaqsyt.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/guamqwoir.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzokwhuta.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gegayxsmu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlnwmnfy.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllmgmrnt.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoymogdh.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gcahgeqac.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/glitkkymr.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbkoxkft.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gzuvlvmrw.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gksxdgtdj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gppetijqr.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbgyqxes.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gemjelaws.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gtorevdqt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gttpsctux.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqvoiibko.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/guvehhgyl.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbpqbbka.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpcxcjmy.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giswdcfud.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvgkbkpbb.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjouqeyv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuapryci.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/giohqoaqn.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkyrfkfw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjjvnxtw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcqkajfhw.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyaqzqxq.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gevgjtvdk.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofykdukr.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsorugdb.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfymnouac.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxyshvpw.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbmpqfev.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gscjbatkw.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gavtnxghu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gutzcvxgj.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdxwlmgt.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gftfpnoig.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnkrcukf.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gwjirhexc.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfsylolf.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpbsnvdl.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicrezahu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsutcfam.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gvfcexqaa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gnctfdlcp.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/getbnxnfz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaikgpmdp.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtygycnih.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsukbbuxm.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gtihiudyq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrxloqxr.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gufcnhvkj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyquueba.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gipnoeuio.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpxotrem.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxuzhhvv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/ggqvptvhv.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gugtsaxtu.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gsowjhrsf.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gcnnqpmig.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlacmcgh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjworfkf.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhrkcgkk.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gazupgbml.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/guighldpr.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gygipohiz.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxsgtbrb.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gryrgjlkk.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavdqxudf.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghmrqllpt.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gfpirdaxi.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjswywbv.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbazwdyi.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gusobqdju.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/glrfaiogk.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuhcviqr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/garndivyx.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvtjazpt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaknknar.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/ggdnopigc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glpwfkkaw.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gpnhshexj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnkhrwsz.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavghuyff.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giridpvev.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfivntmzt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmzgwpzy.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzxwmknw.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gveaszsba.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gjfwonpso.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmxafigv.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsvjjwehj.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grbeuyvqg.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/geyvwdmdo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gvcquprpr.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzqboqkj.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuwnierp.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmurtzvu.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gigdohjun.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpwphcfw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grntcfkcm.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gzamqohuy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpwpvtwm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gfgdjkqlz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysmuzibi.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjygghpu.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gdepahsbu.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvkymzta.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gtgcsahxc.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gytmxvicy.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gammxpaxv.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbrztnvq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gvdflcfhz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmldemjwf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlxpgboz.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gizaaydtr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxztgekh.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyozvtber.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgyplqvh.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdckgawdb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gscjonyrk.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gfjcbxwwg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwfnfzrn.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwirlubq.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfhhixoc.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gciashdso.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gapykjvls.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/guwthywme.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/grrmqsbhp.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/glgtkznzt.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/ghnyijbqt.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gjpjeqkhh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gohpmclcf.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeufwqci.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gusfojfbr.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyefsvqrf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gtxojdbrc.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/guhrwjauy.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gjtyapbpk.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gkojvlrkr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gygjopwpi.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gtemnpqlt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoecqbga.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gfcjsjlqq.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gfvkeobjo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvshowbcf.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gnsevmrwl.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkpqxidg.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmomwzjd.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gwczhkmby.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjjgahyec.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gvdkfkpyf.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gelrwzwzu.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gauincbog.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaihpbau.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/ggkcwrbst.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkekbabk.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcwaqtny.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghhhnocfa.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwctrvnqc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihsivxtk.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gwzeilwha.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrhrauos.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gymanbdkx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhrhbgyx.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gflbnlvgj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gajqjrrbq.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbhzgbhb.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmozitppj.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gguazillp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwuvcaiz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfciivgz.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfubsyau.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gztekglkq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvcznxwp.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwayahak.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gfzabkzfr.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ggbemhykz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gelxdfqmt.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbzijgrk.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gpfboziza.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbykcdxg.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjilnxalw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/glupqjyci.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gahmgupyg.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvsprrfu.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gckpssube.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyujqogq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gitriuvyk.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gaidvoejj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gebugmmpk.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypawideg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gyfutahzl.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gcwwijgjf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmguwgpsk.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gegrcxokf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gtvxlyptr.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gecgoahnf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gavudeawj.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckfxlnfv.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbhdcnmo.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gklmfifly.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/grcvuyjpb.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gpztgjkvn.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwickudu.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosuyllve.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxjikcto.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwfjmqmio.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gdebukglp.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gnsxpxucx.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gntbjldjd.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gjbfzhnmo.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gyfeeglbi.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gruhidbgh.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gerysdaxk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxyhdmjdb.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedrztumj.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmmhqyei.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjqosbyf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdciuscr.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/grcolqfvp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmjaowul.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gqouboaxr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghrzrrkzl.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabzfkmmh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/grvvepmxo.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/grtlggfem.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvcpcqev.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwmbfikl.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxfbozpx.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/glsmgvjom.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/geotnhpuq.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/grcbwyqbo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/geyiioxfg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gygeiyxxh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gwqfhhjis.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzvibskym.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcanwtrok.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gapbysram.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gtjykrcrw.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjjsgine.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznbqoakb.sHtML


<!-- 参考信息 -->