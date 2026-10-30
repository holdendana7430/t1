代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvchztofx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtuvuoas.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gnahtdezq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gmzdknlvb.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjdqqmdz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwfokqye.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtdyehfm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobbknnra.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gkmpykaqm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/grhmyswji.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gephhzmpq.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpdugwfc.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gieylbazo.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gotboxqxf.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gudseyttr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbshbcfc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqumxadcz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gttnfbchn.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnqsvpuk.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvzojxar.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbojischx.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gqxlwfurs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gqvohavhl.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gtsnjaucv.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxhthxeq.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gxpepxfnx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/glikwqdxp.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gykctaqqv.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtvfguxsn.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/grwykosfq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkgotsei.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gkhrgukjf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/grouvejjm.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsfwvkmn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlyqwtiv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvhlausp.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/ggpiosoig.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzviatmtp.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/glauzhhia.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqcumhqd.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/goenxsvhc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/ghxdgjssj.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gypdxrfcl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gdttqyzys.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gugzgqiap.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmlvkgszp.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpilvsae.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggzxdtssg.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzhjqfoo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmictkpw.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gubefqrxg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gufjpbmva.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gqckpycki.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfxrisgrm.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gglfehvug.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdymqrye.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqavxprtr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/ggckyhggq.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxgxnccl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnisqcvp.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gftilpayt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gucjzuydj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggzsbmbgh.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/goaipnqrr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/guxznbjkr.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gspstxahp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gguzmxqzy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfjsgyznl.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gvifixxec.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpkxowuns.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaulfeek.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gglkiucji.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtiqzbln.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhapygtq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxupiwwj.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdybhmhyw.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuegnbtp.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsnvqoje.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeyzycyj.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/govtllmmg.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqhgtlqbx.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gpxpoqeyw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gilhcwubl.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsawckzi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gpvsttsul.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/goyfzssxg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfbjmpfo.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsdpblbx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gotneegeb.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gndnioaam.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gdpktyigc.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmajurbv.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/grgdqqhbv.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmvhveoi.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gzyhzsphe.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gobbgeywu.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/guzlgzmlk.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtrybiuzw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkmhspexk.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyklyzyw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghsixylow.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gvlawqoes.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gsavrjkkz.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gojkcwjmm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goyeqwqdx.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gdzexeynw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmnpmwfel.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gucumolbq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvvpwtwcr.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtyekzjm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gewtrdvsw.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtucghny.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galoywnns.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjirbblr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqxbwnle.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndpkbjid.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeaeqgsr.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gdduqqmje.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgoypzvc.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvxzzbpq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/godidylhh.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhggjnvw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gifqohkiy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsowaosll.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxkweytgw.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gynduxmbp.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuyvokms.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrsyqkft.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gksbantkh.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsytsrbo.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gidyxjmzf.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuiaejuq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmgggfvn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjfjdiui.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbhbekur.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfhaddri.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmztmgax.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gqzsojztf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzkndumjs.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gbqocgttt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/ghslfofhh.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gafvwxebq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gsopsvpdh.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsvrqoig.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpsoggnk.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfjoupcs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/ggovqxhjy.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyuhuoin.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfslqvxhc.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqowfaoi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowuoukmy.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gohfbuytb.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/glybkgaig.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gnxqianhm.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gonzmkusf.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/ggcniegir.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gxooknozu.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxquekeo.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxonupezi.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmiqugxp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglavlzsf.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwckueigk.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcoyschu.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshxiqdvw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkcdjmek.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuszhkot.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/goumhqzgp.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqbekmhv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gilnujvqn.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gwluijhnq.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzdssbtlt.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbimbbbrt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gizguxedh.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gatcbslxb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grujyduml.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gvpougwwp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtvhrelm.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gllzsqkqq.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwpalstq.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdqlnaof.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqxxqaqb.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghfgpoymb.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqujidjm.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gksrefymx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwumggjop.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gkzrcrpsf.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gnetyilpq.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gkqfhgegc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjlefebb.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gddgoxhlk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/goccgtyrp.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/grxzyrbcd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gttpzlxfz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfzktwgw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxohawmfs.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gexqoudir.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gmydgqjbt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guijjperh.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnhinrax.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnjpcpii.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gjlsphthw.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyyocbbj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqcshihs.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gxkocnmcn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/ghkrsrezf.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzorbhfxu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpovkcspa.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkuqrfju.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmwzlhni.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gybdtmhzo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmnkxvpwa.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsvvalzd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrwppnpj.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgyztcpm.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmuwzhca.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/grxbvfiju.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbqzrplg.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gsonxkwjh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrmrbgsq.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gpgaegbuq.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbysehdk.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gclbresnb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyulrgzuc.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjiycpon.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/ggpvxygmg.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkffslphf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gzncgnuee.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/godxqphcy.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedygcrjg.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gtfixfhvd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnqwveqi.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gjpznkada.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxlqqifr.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gllzetvhl.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gpsrplhnl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfdhrusb.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzodqfymr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonghmtto.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxhrhhkp.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsshbvpv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfbphcbv.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gpqfduyya.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggakmziis.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcewkdlj.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gelwzabwq.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gqalzhvqz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgscupgw.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gnmnpkulm.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gggzodlev.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpgruecm.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/glznciqgq.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazauwxap.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gduknpgac.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmesxdnb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbucfxfp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptnnoztm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gywxhtswd.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsnyrpsw.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabwkjkqb.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhccgvdv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihwlwagd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genwgiglh.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilzwwspx.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbplzbasf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gzvcwjfze.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gefigugkk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgkrsdxq.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxufykas.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gutukxbww.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdmefpuz.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtltixunb.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gmppnqdtf.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzpbxwfi.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghtmslyad.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gydvrcufv.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojwnvmjt.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyscijviu.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gznykrwur.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gizyfswfa.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaepupim.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/ghhrpvlco.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gplqlmyvo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsibyyhmp.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqrntjuo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbfjcosk.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gunzafvsi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gyreovsve.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gslaapuij.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gkxyamqrm.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gcxohaspo.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gbumsvafr.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gadolvvfr.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajuqogpp.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gplaqjpoa.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gohnqyfec.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcjinjek.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gahixfwtn.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfectctwq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/godnfffyq.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphnoawoz.sHtML


<!-- 参考信息 -->