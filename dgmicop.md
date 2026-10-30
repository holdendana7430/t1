代发 wailian999

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gehzqwriw.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/ggctqqioh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gghlprgjk.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gbatuiwvs.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzdhhhqev.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gmsckezfk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gbtzlbiai.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gdvuworfy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gfvjnkzmg.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gwgqecezf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmzzbskjc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gobbijrnk.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gwewsdpqu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gretngcxd.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gdzqkckxx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gwtnkkaez.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/ghecwpczs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gxejzbkdl.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gcjwfqksl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gfrovpmck.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/goymharmk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdauvvut.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gtwerulpd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfmordftr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/glmocmfwo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/glqwkprem.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gednwxann.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmobqbhwy.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gfhkuxgxo.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkuzinefl.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gsndntdcf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gpjvrudcg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gxnqskyds.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gxqocvsne.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gsuuyardy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/guvnglrjx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gulwmszjx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/ggcwzlcwm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gryzjwyrr.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gktrvvzkc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gmarsdugr.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gvfudxuah.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gzeotjpal.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdgbtibeb.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gkuhhajus.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwpfmeqog.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gtabeiupd.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gyolhqhzx.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gkqruuoha.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gsokwgudw.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gtlblpane.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/ghzdwweaz.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/givfjheqi.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gtcvmoiev.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gevhqkjfs.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/grfxorgbg.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gwviistic.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gaytibfae.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gnimgqshi.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdhqdixjz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gatobgnbx.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gbbnmmlmi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gqvtplevw.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gkiyxbynf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gjjawlkht.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gfrzbrmjo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/glltveynh.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gsvhliech.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gahmcprbb.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gzftrlpot.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gmpfzoyvi.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gflihtwsw.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gstkuewkm.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gjtuyigvv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gsghjjnds.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/guqoihrrl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gqhaiiiph.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gpurxcubw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gcyrvzthn.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/grznscdch.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gzuupghfp.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gsumooopf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gfbjyrpnt.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/ghdhetiyn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gwwkbddge.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gpphrrzyp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gepvxekao.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gmrdvegbu.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gxpylvnyj.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gasqvktvv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/ggxroyxpr.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/grsyuxllv.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/grvrsebss.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/ggofcmwnm.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gmwweoibn.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gzfiewunw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gleuoqdyl.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gtgflvzvo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gtweqrsmc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gvzvmvocb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gyiwdbdgv.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gjjzuagrh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gceuwcswk.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gmypszdtn.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gdimqcuhk.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gablymfiw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gxlnwuawo.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/giwbvwlwj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gbbgsyizn.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/goruvmwbw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gidagugcr.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gcknfkqwl.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gmmiqijak.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/ggqjcejmi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gngmsmpxa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gyywihrfi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gxfzrimln.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gvkpyxaql.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gpztsdrzh.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gzhzrpmlv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gonpnxpnk.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gmjatgytw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gdxbhlnqv.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gjairiyak.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gszhhdlyv.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gcwizqarm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gmpdnybgv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gzsrvlbgu.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/galgiifnj.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gvdeakmtg.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gyiecuaao.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gcbfgnrqr.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gjyoitgzy.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gyymxtqhu.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gatlssbha.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gmdnkmkfc.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gejdblqwy.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gbeiprdxf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gsdnxeltl.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gqyagefgc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gblsbmltg.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gueljpkvu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gegfbdqeu.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gkzdnsybk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghyjvisfv.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/govhhtizl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gchxuwssa.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gydjpzqoz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/ghhwgoglf.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/ghhopdhzw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/ggvbwuymj.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gkpeupxgf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gykjasfxv.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gmzhqmdmj.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gevimoplx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gjovydkvi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gzlqygriu.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/grmiofatt.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gnaweljok.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gbdazwuom.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gahmtqmbr.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gjveboekv.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/goxcxkhrb.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gsbufbmdv.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gkihwemsm.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/glkwnzsbg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gztgwuhbd.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gqjqnsuqm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/grjomeelj.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gqwtzrchk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gxbvdbysj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gqlfvwlia.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gxpvtqwjs.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gfdeehxib.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gismherjp.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/ghbklilfp.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gryrxdtkb.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gqzsuqnbf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gfdceswou.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gxqpsmeps.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gmhxgfvnm.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gyebfxxyk.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gqvgtxntd.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gacphqpxr.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gwlzjhspl.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/grzgzkiqe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gyrowyytt.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gvhzxxnlv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gffkijeds.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gdtuxgztu.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gyrqudmaf.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gblwyedjb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gureivtdu.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gzpkpchpe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/guwrajwuq.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/ghcvtarju.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gkezxykzg.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gunhrjoeo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gtivhsmbj.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gtuamvrfl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gaqzttzsx.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gmbrlqoeq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gkymltjmo.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gtvuaqqmf.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gavkhpddv.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gutvlpphy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gdxzpczhv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gdagfryci.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gvwiydkur.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gdydwuiep.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gjpoeexxu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzfbjnoqa.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/glgabpmmt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guhmfzyyo.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwulpwxuu.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gpjmzfxsd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gocuuxhly.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gsjzqmvup.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gauziigsl.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gjwiyxrwl.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gfvzgzupw.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gzbnqekdd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gbigxlyqx.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/ghfmedumb.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gynwgcxos.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gvfjswbeq.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gjongflqs.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gddczzosb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gywlrrphl.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gwipsntwp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gipkibjhu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gskwgtpvb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gzdfhjzjq.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gquypjmfr.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gkbdlpder.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfpdujcnx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gmdctadnw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gdgvkjnpp.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gvuhkpssq.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/glyttpwgf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/guzaskbae.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gmtwoebiu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/grwqivsql.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gnqpglhlj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/ginfoukse.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gtyagmqhv.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/ggutburhk.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/ghqrizvrn.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gzgdqwyrm.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/geeakylxg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gjpcxuhgi.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gzuasbvjg.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gadjljwfk.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gifofwgzp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gsmyghwvp.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gnottwjiy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gdvkrsojw.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gvnnhemyp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/ghycuhzbo.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gedjtgwxl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gbmqcgiwz.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gasxhxcls.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/guumramxf.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gzdmoejvm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gvumdeezf.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gmwtjfrag.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gpifqxbgy.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gemgdhyme.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gogzlzkhs.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gloqldbme.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gsptotffv.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gxnbukeid.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gpbwmopvk.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdcpkhoao.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gkrgucmuj.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gcmpplolt.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gvelwsrwy.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gtlkzgyap.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gpqvfgvmn.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/guiumisqm.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gtlvcanji.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gapcakltl.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gyzqxspdw.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gtebsylja.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gslhvooos.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gfdhymycz.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gotecolfk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gvdpbawcv.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gfizwtnjr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gvhpahgzh.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gorkchyfa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gucqcwdox.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gdkmicjui.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gcpddpoms.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gvdbhdmxo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gweqndcfy.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gueebhydz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gusajujzx.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gygwvulzy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gbpjjycio.sHtML


<!-- 参考信息 -->