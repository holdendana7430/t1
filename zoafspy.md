代发 wailian999

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/grtghgpit.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gapslyyou.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gwtfqutjj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gqobuicqt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gtxlbfxrn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gzvnrgjls.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gcpbqgtbw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gjjadktof.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gngrhqwwu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gcflvhbha.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gaxafhjyy.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gffpllyeq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gkvsuseod.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gboawouvd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gbwultjru.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gjcjoihtw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gmixrquhe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gqpenugjm.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gcbbgsopv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gqfostloy.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/glsnsrdgi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gzgxkwaar.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gcrobgwsa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gorehwhpl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/grbgqekpk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/grnzkxaxq.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gmxrktoad.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gbwwudspl.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gunohqbrw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gklafdypx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gcsiqrkuf.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gvhejymyn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gegknrvmp.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gsbtpykzp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gtguwuxqq.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gqsdufjnp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gyjxoheyw.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gyjcwuujk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gagdispve.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gkdddanvi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/ghibcbbnd.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/ghnrwmrhw.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gmpjftuyh.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gxnnxxgjz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gegqjuksx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gmzgcmfeo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gwbvsopzi.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gicnnlskb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkmipaiqn.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gjvdoarqg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gpkpavtug.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gritqpmyw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdndxayby.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gdookynhr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/ghrllqzcj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gzftweurb.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gusieezlz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gemrjxmke.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gysmfllhh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gjvpmdkqf.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gsmhuuulu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gnjnkgwzj.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gpucabskn.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gbroskzcb.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gnqvuecig.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gwuihavja.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gfqknjekx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gzduhwjht.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gvuvdbsym.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gkkfzdxzu.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gkyqxrftv.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gfueileup.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/grwtqmclm.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gtlzlnimx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gjomydybw.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gwesopjqb.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gaummwfoj.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gmcpskqql.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gljugwpdc.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gujtrmdsq.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyhjiyjoi.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gnnykyfik.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/ghuzglvln.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gaaukxvlk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/glbaqjywe.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gvhhdzhfx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/guvikfeor.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gpkxwnvsp.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/ggdmnhmcw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gbwqacqxb.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gkrbdlyqz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gbmkrcvex.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gowmqeunl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gbjvvfyqe.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/grmtcbcik.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gtopufmhd.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gjezrstio.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gazogzkfr.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/grlwtakdn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gicaymzwv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gmvqxnvkv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gypxnezbg.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gvespfqzb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkzrulgrc.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gsxpjyctn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwejkedgt.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gropesbrp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gsskltrnt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/geveegkde.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gejbfkred.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gmclrvyiv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gpvywgvpd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gkyabupuv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gilxizatx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gddwkpkgv.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gpuzwfuyl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gkulppmoq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gvywxjgts.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/ggrycjaha.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gndtueshi.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gjkbowonc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvxeyqbap.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gowiuudjk.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/ggzkxxjay.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gnrvkgwba.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/ghtcvghkr.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gzunehjrw.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/ggmxtusvv.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gnhnssjtx.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gjflgbkxb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gdnjmxmmr.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gnfkqqbab.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/govlfkdlx.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gvyvddbfl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gnjivdybl.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/guhattxdp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/ghbwxksrf.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gqyxmsour.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/grdglfssm.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gwdxzkiop.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gwkeugjbi.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gbmczznkg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gzdrwvkia.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gpdobrzca.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gvuqszthm.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gtiuofemh.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gqsplaljx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gjeojlujh.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/ghlkfbegj.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/ggwpuqnbt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/grhiijvlq.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gfgaxludn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gxcnumqcp.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/grztpprxu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/glmtbzqvl.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpxnfmxnv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gnxyhnpsp.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gmrjtznef.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gwpdnnhqd.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/genetfazi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gdmkaxerr.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gsxkwjqau.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gimclgruk.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gepmctbut.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gsdiarvjn.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/goehlcumz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gpihfmfie.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gzcpudbsn.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gutlsffnv.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gdxdhbqmw.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gaizehcdz.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gkvirltge.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gtguiwguq.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gcycrveln.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/ghrzqbkya.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gzegopmcu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/ghqjckswq.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gaaahaxmu.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/grfjigngg.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gahimpucs.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/goenxibbe.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gkeiqvicw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gevlwxipd.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gpaenfubz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/guphidgkv.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gwjfdpgkw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/ggqjsijjz.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gybmajbqo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gedixsxch.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gkyqngoyx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/ghnfryoes.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gzpwfuzhs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/grlenjalv.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/goapycvsb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gljpnsjaz.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gxfypvpun.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/ggpikasch.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gellbbuwy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gfiztczcd.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gxjycibhu.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gczcsulce.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gyvpbulcz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/ggasjinii.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gclriiadn.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gucabjqcw.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gifgjcnmc.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gheqtfihy.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gfdyhjncr.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gfpgcccko.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/grxzpxuby.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/grdilxuct.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/guirnonka.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gtraidrpi.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gfitcgscb.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gqzewzppp.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/ghkyfagsn.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/glhmepmmq.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gdjyuisti.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gjxaxsloj.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/ghsuskorj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/geowionjx.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gkhyzsnbq.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/ghwrtixpb.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gzmowhdya.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gemzfkgwc.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gzuoargvb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/ggwigharh.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gqvxdoght.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gnjytnzsu.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/grjwxsipj.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gglsxgxkh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/grwoyngou.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gqeljdnac.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/guhyhilsf.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gbiiluxmy.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gehddwjyo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gpcdibjzk.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gsueyicqs.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gexrdmnen.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gxujaugpv.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/geijuybag.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gszdwunkf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gpwfmbuvv.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gdgdxzkjb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gkrysfyxj.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gshtsgfim.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gvzqmcdcb.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gxtkvaycn.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gyqdcumej.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gugjzqomp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gisnbmncx.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gknuleyoz.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gnjlvwpzj.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gbcwbxjxz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gbtldzytt.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/genbjyvop.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gwqzrtzet.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/grjtrhklj.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gwszfddmp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gxroiaujg.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gazbmicfr.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gfwuslxkk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gbahrhrhq.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gwmgfkvnl.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/guoqjqrhr.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gwloyocei.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/ghsxnpatu.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gttrtuljl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gjvvxxgld.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gcyqekqkh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gjaqzowpe.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gwvpparlz.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gavrhohul.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gefufponx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gholpmrcx.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gkwedhvzi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gamewffat.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gxbeurunk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gwrfjxxna.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/ggpdoxypo.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gqhxwcmdf.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/guuhwctwz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gxwfyijzq.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gxhdjnmvm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gutextgne.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/ggcfslbmi.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gjwdjblwr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyfrkfxpr.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gngeirocg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gobjqiyye.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/ggqvaecpx.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gcqncgqmg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gyfqobkon.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gffrsdvdf.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gbhhkrgyg.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gqdrijjfb.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gpzydwjid.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gifksebfo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gwkmhvoza.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gsguzvpzz.sHtML


<!-- 参考信息 -->