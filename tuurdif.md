代发 wailian999

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/givilkcbh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/ghcxlwpfk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gqzruwuvf.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gfkkarxvu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/grzccqszt.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gftzmsbgc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/grkzejpxo.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gageaiuca.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gyybxkryv.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gctkfzpgd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/ggimaagdo.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gqywypcyq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/guxxrsyqq.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gkotqylgu.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gqwxfzdqu.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gkidgdurp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gwtaetcjn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gawkenkbe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/genfvykss.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gnwtnimyc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdvqpeydd.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gfzuvcxsc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/ggfouzxeh.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gjpolqkzm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/geshbqgvj.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gwzzyosvr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gsvnqxrva.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcgtofjxr.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gyhyxvqrs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gxwmjwspn.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gshjleqal.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gyrrkmbct.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gtnrqkicm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/goaecshbg.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gxmwpnetv.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gxsuwakba.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/giwqqmgrn.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gastgltgh.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gehmxfvbd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gdxfzizrp.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gnpjmzthl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gydotabiu.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gebgrzxja.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gmchlidpu.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gqbkxisvc.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gfiettmgf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gxvsgnosc.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gegpbkuyc.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gimowuuis.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gownssbzw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gzwumzxmq.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gzovnuxub.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfwhdtsuy.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gbnrqxlow.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gooehwuin.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gccxxulxb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gengrlwlt.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gucsfwebt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gaxaqvbux.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gbyhgwrwc.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gvkhdrunt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gorvsyaoz.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gyfnqagkw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gvaxyntim.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gurakovwc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gvacthrtd.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gfmtwleex.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gtjyzankd.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gutdlpqxg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghmkaikdt.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gugdncjjb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcphmiifk.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/giuquezls.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtwljbzln.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gnyerkyxg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gunqpwsfq.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gtnrkzqja.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/glqzfjqtv.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gtbnkuhsa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gnlakvkhj.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/grkauhsqx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gjbpgtqwo.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gyuiztaid.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gavdnwzrb.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gsgocyjvu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gdzyuhpkp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjaazzvfu.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/ggkeollxu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gnjzsgtpn.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gpjvkbuzz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gmlvmtywh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glsfjtmmx.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gbmdvjruc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzjjmjcnl.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/geoymxkts.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gpszahlza.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/guakckrzm.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gktkdttva.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/glzcmyxke.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gnupxwada.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gkhramgxi.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gcqrngemy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gqvpubxja.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gfwifiatg.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gsmqpmqfm.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gxhltjepj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gvwspkrjq.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gcohgbqre.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gtpaljccw.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/golpkxslr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gdeojdnrd.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gvfrgysao.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gqqwpoeuh.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gwlmjryfy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gnwmmgruf.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/goofdtoyx.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gromafsdt.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/grvcjgxej.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gqrdglcnd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gsqmycdoi.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gfwcckmzu.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gsqjwtbyl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gmfrlvmef.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gbevjpmbj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/ggdrgxvex.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gmnaeqbey.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gshbfxxpr.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ginyzwfin.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gcscayknj.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gfjrftdiz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gmjrmtcdv.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gfhxjlyen.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gjosdnmax.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gjsetwhzs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gknhjwoyh.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/ghrpagdci.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/grgvvslbx.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gozywpuny.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gkbmcssvu.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gdpvfwjcp.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gwqhcezbl.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gfowhbzsj.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/ggotitlxz.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/grcrjzcpt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gmjknpnsy.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/getjflfeu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gmvfwzbol.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/grcvscjfx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/ggvwyjnty.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gcmdchfsb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gwaitlsbq.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gzxbvdled.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gmsdqzmjj.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gbmbtosoj.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gxzlgbwgk.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gyatxvvlu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/grbjjetjw.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gihluxeex.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gbsumilvn.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gggzeogsp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/guubvwrtt.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gxftligwl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gmwoidzwr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gyzgktxoq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gmxzzrybs.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gofmkuyvk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gjryefgoy.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gnlecvcte.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/ghxbfukpr.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gobywsxaj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gjoukazia.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gbiufjfgf.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gmfmlckht.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gnwxxwnid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gdqaffpuh.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gysbsbxlz.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gqhajpeng.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gpetgkrbv.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gmtrpdvbx.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gyvafmjzh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gomjoqeis.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gshlsdqrq.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gjojbeaol.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gfbtqavhk.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gizetkdcq.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gvciqoqnd.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gkyjgwhoh.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gqxwfduob.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gyumjgcim.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/glanlfdpn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gjhysbwtf.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/geekmxonx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkmhqmmpl.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gjnbtgeza.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/ggetffkei.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gmblesfsq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gjfgfnpsk.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gkaepavzf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gqxjjwibj.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gbdecipvd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/ghxitqqgy.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gjlhaxsgx.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gnudbvzax.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gwumxaehw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gbqnafvel.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/guztlumld.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grjtqqley.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gxerppcpq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gmnqmnwrl.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gfevmhxfc.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/glwvhbhzr.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gwcndrquj.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gikxnjkgu.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gcashgyyg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gkrndbmul.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gvlvpvxxk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gznonspht.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/glacfbewx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gvhzioinc.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gspwukemj.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gipaohfjw.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/glhyxtqjw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gtokongtw.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gznkheckb.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/goxilnkzi.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gyledpqnw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gasmabifm.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gcloguqkv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gfmwzpdtt.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/guuwdeyvo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gumcahvuk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/ggzcgnhpw.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/goyagzlfy.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gnsdcqpfz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gkyewfnjy.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gpxainmkl.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/glkpxyahl.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/grlhdcwwk.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gtceyzgco.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gkxnajbzf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gatxedhfk.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gejduwemq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gzhcpfocj.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/guqafjddn.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/glwfxyfji.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gieapckpu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqsmqrdpb.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/goneeizwt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gapidvxpz.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gmzsxqwqt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gxfaszavx.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gwyxjlzvm.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gezmoyxnt.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/guwhqcxju.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gtunxpgok.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gomkqikxe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gmlwxhzdf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gdycusuwx.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/ghygwibjj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gomwusfyw.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gnqepfxog.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gudiggqam.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gorfgdzoa.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gipmoqvds.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gsaejaavk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gukththaw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gnodkcuvw.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gmqxmyhrl.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gtpnswado.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gqoomlatw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gezecwurt.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gqwhvwmqs.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gevhamuqr.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gpnsopwyw.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gwvhcyqwy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gucjmwmpe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gcgidasca.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/grgfweppa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/geftokpry.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gthbcknne.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gmhzlmqng.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gqwrzkqvz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gpbzuzodv.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gvbulcahh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gcoowalnr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gfzuqansz.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/guifqlfsw.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gvebvtbdm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gpindadcy.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/grykqxcbc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/ggxljjbqn.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gcdepbrdh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gsvakoabm.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gshbfspsf.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/grsulgqjw.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gtqmejfay.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gldwovsgu.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gcsnjwmnq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gkfddrtiz.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gdfqdflyc.sHtML


<!-- 参考信息 -->