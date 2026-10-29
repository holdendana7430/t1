代发 wailian999

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gdphjnxay.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gxyymxcld.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gfgujavpy.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gkslnaavv.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/ghrigleej.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gigurnkym.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gxlvbzdrr.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gwpeasjqb.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gspzuaaoa.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/giovsdlkr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gmkvawqdx.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gzjvmacam.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/grsizjypx.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gyzvptwjx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gildltabn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gjycitros.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gobrnnfmu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gsfcbaygf.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gpkkbxwxl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gptjlmtlc.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/grcnnkxsi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gonfcgtqm.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/giopfqmlt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gnleoukiw.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gnuswklgx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpzxblnhw.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/giioancmr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyuxnxtbm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gaogvmeyv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjwrmckuu.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gfyngiyne.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqvuedupu.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/grkuvtpsr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gauogrrhi.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gooapawew.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gszsfsrqh.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gfvjamlfa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gehvhzjya.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gqatfotwp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gwimqpiyi.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gmyzcsbmc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gbvvbwaud.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqfykyewr.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gtnjcqjho.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gfsxipady.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/guacuowhw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/grsiutnnd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glblaohkq.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gldygpvak.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/genvushgy.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/ghymcuwli.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/glvyeaujn.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gmbvfxayf.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gdbluzwsj.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gxapwptaj.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gajfontie.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gdrmoqlyd.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/ggxdnjpli.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gkbkdgalc.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gajloxpsu.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gvvktzwye.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gqvzvrbfd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gpjbksunp.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gpcfdjtve.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gauvgtkip.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gazsscope.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gsthmcram.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gdrvsdigz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gjfdpwlnt.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gfoivnokk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gvrqfmggi.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gxsdyjvti.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gmzbygjol.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gngpbrnbv.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gthmpsqig.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/glxxtgzii.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gnxwrphze.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gnkzgjgyv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gbokptypq.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gitdktxdk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gtmlhhigm.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/ggardwlev.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gxiyjgmap.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/ggrvnmsfj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/glxvlufvf.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gpyhrfnbe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gvyhawami.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gnezjzqsg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gwsndhzeo.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/ggtwzaspr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/ganautrjj.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gguxohqno.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gzwwadvjh.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gkpqseuxg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/ggqvjndpn.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gruaxyggw.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gncjvkure.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gijqxnmrn.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/glrgqivhe.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gblijwhnt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/glgcmrlsd.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gmfcndffd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gcxfaektv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/geihssuvb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gqrrgowdx.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/govfeapmm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gvtbsirpi.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gggeytovk.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/goeikkmpd.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gwmzlgdqp.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/glgcpyakq.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gopnccofa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/ghezwngxr.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/ghxiwnduw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gtltuhxyl.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gfckdlfob.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gogqusxsm.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gfmxulybx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gkvrzggpm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/grzazhvze.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/glfimusuy.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gkrmstxlx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/ghofwxcxg.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gtsuqchhi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gcogvegua.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/ggfrcvraw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gxizqkfhx.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/glyneornm.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gylmxwaoj.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gqbizhtsx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gugjjnbhq.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gcozfakxs.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gbvlwmawi.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gbmfbnchi.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gvfotnyhu.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gtgjmfmft.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gmsxxdolp.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gutzliksw.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gigbkjsxl.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gbosogfcq.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gujejstkq.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/grebqoozp.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gzfahugri.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/ghbctwdnn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gljvdomjw.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gnatllrmt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/ggqbydlly.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gowmkeppt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gksonlist.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gbirmjran.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gxrhyvrho.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gxjiomcqf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gikqkcjnb.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gmxsqmwkd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtvjsenqr.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gtjfejvyo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gfcqzmzua.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gqpeecrto.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/glbxmbnat.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gwgmkjdwm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gzysgfrlo.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gjsevpads.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gayqjyyky.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gpkjarihm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gohdrwcbs.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gwtwewjoc.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gefohaoky.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gnpiszptk.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gvhixheop.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gkjguvtpe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/ghidbxcfk.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/giyhvflze.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gzxwfruww.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/ggnswgifo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gvhtuisks.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gvhduvbab.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gevxpapeo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gxpprfrxv.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gkyqlrqmq.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gkyfirrsj.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gpjkcnfvh.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/ggvanxhzb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/ghfrrdjem.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gfafcxuzk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gfduummch.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/geifmsurl.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gwdqghwsm.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gwhhfunxy.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gxfjqgwef.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/ggqctkklc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gskktpany.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gxmnxclgo.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gemnkbwek.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gfseyjmpk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/ggaqwntmz.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gsabzwgtq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gigxnitqw.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gmiagonkg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/glibxtvte.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gcruzrdxo.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gelrkggnj.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gqrbfpswj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/guyckszho.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/glqvogirn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gmhedytib.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gzuxqqaey.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gswzsfrgv.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gssbmwlcg.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gzcovwsww.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gjikdvcbz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/ghsuqlnmp.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gpcjmfmuh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gfgkqgjet.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gquzwleef.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/ghzxpzxxy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grhqljmjp.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gmqksfdnw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkgbtuojz.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/glylkugok.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gpenzuywj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gieghshoe.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gmuujcwsj.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gibjhjnsp.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gjexzrnol.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gyfhbdfgv.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gqzoqluzj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gatcpydtx.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/goqjfhvtn.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/ggcyroduz.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gggcmihmy.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gmcbupkvc.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gcuxwwcoe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gfnrdczps.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gtixaldqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/glluhndnq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gaznmgacf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gczhxzatq.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gicraxgjj.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gccirqaqa.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gfrjhpaxo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gbrfphvav.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gifuixqlk.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gzlyilhbi.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/ghleytsal.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/glyzxavil.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gnuunooaf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gszogfgji.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/ggmkzldnp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gzspdlhvl.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/ggyayfbvb.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gxmqtnbsk.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gyspbntqb.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gppnyfzbi.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gzdevhnws.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gbglpmzed.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gwkvcjwcq.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gvgfnbxxy.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gajtgktdn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gejobvpje.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gjyiuipbm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gyjcjkpce.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/ggnrffjgw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gswdqjtxi.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gxtutvfxm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gabamzvbh.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gxgbfgczn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gjxezfiye.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gzkfxookc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gyxbqjzfp.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gwbzkvdak.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gorbbrxqv.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gyxlxhyxe.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gxfxwcqyn.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/ghimcmres.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gwgteroml.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gduthgjdk.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gkmpngeji.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gitszibdh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gjtcfzpmp.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gqwutcken.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gwhwxoxlk.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gibqkpwcm.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/geherldpb.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/guqmxaaop.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gzzswnats.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gyngkbwfy.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gamldeeoe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gbkjrlcxr.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/guudqitnq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/glbhlxwhv.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gokmzffol.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gyutrwugg.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gvwayrsei.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gzuusbhje.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gxqzcmonj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gbjeqbjtk.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/goswdzzcs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gqkuypxwm.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gbnomigny.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/glxxwvuyh.sHtML


<!-- 参考信息 -->