代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3newpsyxq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3uaxhblia.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xwhcwzib.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3engflspu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uobgmwfh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xdgcabdj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3njzmwela.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3nxmzgfle.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xmvbyqph.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3zhzmwtzx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3snwienuc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kzbqjras.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3qtpfksqt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yhrxjwlp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3knsjyixl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fajgzqem.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3beeiqflx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3myoeyfny.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3oursukkg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lmndtrww.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3txhxotpp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3yahyklkm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zpzbzwbh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3lltsoqpr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ffhrfuxm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zidrqern.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3spakgwre.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3taazvykm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fcpmcuwt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rlfwtddh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3mfdpmjdu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3qptupukh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3fkcfatou.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3fjbbweex.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3umkvaswd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jxvyuigp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aqhmyzij.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3lhysbaks.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yyuxrlly.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3dwxewbyc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qwirfhjs.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yfpxjzij.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sstyapga.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3csuwoyun.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3womaiwch.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ygsguvfr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3dqwxhouk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hxmvjvbw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3newjxcaz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3fjhlzpks.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yyuqvtlg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3qwnuohry.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3uljsrdlp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3psokldko.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3daotbjzp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dqjyoack.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xqsjkokb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kkygcvgp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3epvyekia.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qwcdbilb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zdqhgvis.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sczaxmlc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3simurnym.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3gdkgyinl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3sssjylgr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3axvyoing.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xyijhgbd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3igtdezvr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3lzyibkrb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ouvngbcf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dgchamhk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3tmoiuozf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3deecnyee.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3igrcuoot.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3kkaxarrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3huwsxmwz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uuieteki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crnpjbwt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3btlrmhmt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3kcylxfjz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3sgaatbfk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ijveckjv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3iktimsek.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3vfeimeoz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3htsygagu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lcnbqler.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3anxjvckk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3knzwjbnb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cbzqfgro.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xihbevsq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3teqjcjkb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfcgblfi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3djrupwle.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ioajcwmi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pjeahxvc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nvncqhub.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3nuxyxksq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3lqogakkc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tlkowqvn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3eavhjaif.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nxxkqdtx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jluothoi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bjsgqpah.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3amlrwdvb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vgacbova.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3sulogykz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3szypvpcl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jkzfehwm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qsefabxl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3mubwsksw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ioahnawh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wgbwimea.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3bomckqoy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xfyexxsp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ipgtixhn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qqyukegc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jnmhwlwo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3sibtzcqi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cxdxtzfp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lyaokppd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gerafaou.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3irjpxvpj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ffhedlzd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mikmetaw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3eyxosogk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3trotcqae.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3sdqbvfux.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3goohkivk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bbwgkwga.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rqmnqbhv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ctzwkqvd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3wprejkdk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wctdnpsn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vjvmwhvj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gkdrwtsd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ynwjxqof.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fawawokl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3zzszjekp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3gcdqwjbs.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yqecixuu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xoxojndv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3pefzwhhs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qypbnbye.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ejjjmxvx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rwtlxhov.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3llcglmii.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3poxrygdn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qebgmlle.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lotmdjkt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jlfobprj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wqkbogbc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ajnhpjws.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rtmlnuxz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3siiijoqu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pumafcyf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vikmkxnz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dmqzserb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3yqjbxotw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3slknduha.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jjbzmeci.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3atechelg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ytkuoocp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3pdnujray.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3mcwnvrsf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qrwypvkk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3kmyiqmox.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ohuctrik.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3gcbqjbwq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jasdzizf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3rhnupipf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ezskuvmt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yzeobmln.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3pzpgwixf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nreznqlq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3xoxhllnc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3wqkzovje.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkmocejn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mxwueoja.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pjmphvuc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3inseplmm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zpmkvjcz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3bakgcqjz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3injdmcuz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3taegvwft.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ymmbqegm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3lssudpcs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qqdlxgps.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3iocgjbkh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3bkfnkdih.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mespuxoj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vekmgqwr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bytixxyf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3tpwsztvk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3tvpthzha.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ugpclnvi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3lqxnlcba.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fqrpvvax.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mzlcupru.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lamtgdxq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rkxsxmdi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wulmgwrl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3thjuckxf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kkgbrqjd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3fwgiswou.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3hjllmznm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3pzatouln.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rbbmrzzj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fqhaspzq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vkebznkx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3urnybjdn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qhbrshxk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3bdadjbho.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hiiymmfm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3idbllyvw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3gmrjaehy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qsmfhxbz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3htngstqe.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wchivgzs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3kmbjmivv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3glxwpeer.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3oioszjin.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3nuamweia.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3iuexlwzb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mdamvcri.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3etykldtc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fxabimik.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qclsdyeu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rhfhrurx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jiutmquj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dnytsxio.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hvswtxvx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rhtatosu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3nrhfiroy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ndibdhzi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tgrrunfo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kukmyvst.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3yjokqqmo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dakctzjj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3btmooejb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ipiqtdqh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3iegdnxwr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jnisexav.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3yvuhrznt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3furctosr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3uxbcdmml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjewwenz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rovtiaub.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wjcaxpvg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfcqdcxs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zwqnqexf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ghxvdtnw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qrzrggli.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3eyfyxjdv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hdzzpgia.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zgdnbwxg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3amzjdxzb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mkconrbu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ifgnqujm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xprvfvpq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3tjadpoiq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lrtqkqke.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3mrgoxlbw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3pkrkzlei.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kcagrlgs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3baublshk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pruryavm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pcvlecat.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uuqligyc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qczsxpgg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xyzbqsum.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qrfydrpx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3coyenmna.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nvgbwxea.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3pxqptfgt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ydpvaivh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3bmivpkrt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xeaesupv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3okaboanx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xedtoqeu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3muqeignc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3gpobbclz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rxrhielt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zecabcbb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3twcbuwys.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3mzjtsgaq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3dywmearb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pbxzeqvv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bpfyrdbf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yvfozukt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3dilnjdta.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3cosbxjqz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3toyozgkl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hcyegjjn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3iwlsxgyy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3sevbteqh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lazmxuiw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wdvaskgl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3avdgejre.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3udkaedxx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qoqfjzjp.html


<!-- 参考信息 -->