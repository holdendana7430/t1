代发 wailian999

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gcecevmff.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gqhrtbayj.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/guxmpeyvk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gwotwoory.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/grxaitlxz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gqaywphbh.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gdnblegoc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gdsjhingj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gaugneutm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gfbnjzmmd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gueoiagcs.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gvozqcvrv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gbkbskhav.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gikdzbndd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gvbmysytp.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gbloyrmpm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/guogucdvb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gujviazlo.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gfvlzdkhx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gapevukhy.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gknmarhel.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/guxqpaxdv.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gvzbqpyhg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gyhfwthdq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gxouznruc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gkaoqzidy.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gnnfsylfp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gwzcozhpt.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gminvzaeh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gfxxzfaby.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/grxvjlwub.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gkbdnwbpw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gkfbdgjsp.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gyqxfbbfs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/guyqajswp.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gabepwrnq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gykwirkdf.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gfttklaef.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gparimilw.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gsazhhazd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gpsqfmxdf.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gkkpgigzz.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gkzunmcqu.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gvpefyqnj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gdqikywig.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gexpfgqqt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/grvxjansg.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gxazlewej.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gferuwuxo.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gtfunpmyp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmewqqdbv.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gtxnrdpkg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gawbyekvp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gyjvfxvvz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gogxtamxv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gtvybbegl.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gtrcqydbh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gshjirwdz.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gkfkrgtpm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/grbieopuq.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gpcltgqtt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gzfrhromh.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gsbfonnwp.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gvoldsvbg.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gfghvrhnn.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gergyqqyb.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/glsygtusd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gtomroopz.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gozgbniql.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/ggdknlhbr.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gbsxvdagt.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gjcbmxzmk.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gummyarjl.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/geurfupsf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gkpmkpidc.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/grsdxmyuw.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gzvwenokc.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gcqsjcwby.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gegbioepg.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gwobrlnxv.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/giadnunct.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/ggepngvka.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gvodjxnsc.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gitwnqcez.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gjgmxcxgl.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/ggvzkvjug.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gudowhmwc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gbebnowwz.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gylqbeona.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gveaxaasc.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gowigqpqb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gphskwqag.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/glknlfdfn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gonvdezos.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gkyjtsasc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gqfeqauyv.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gbsbwbovg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gboxfdsbl.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gedkhvzrx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gxbkfndru.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gyyoqthnv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gybwikmys.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gnohmilot.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwfqubqwf.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gzcrfssyl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzkkejtbv.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/glxeiftzt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gmevdmucn.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/ginzzbqpc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/grsvzivnw.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gkrrohhml.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gdvsytegn.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gtfzgrcjv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gmwgdqzyz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gnjfpqhlg.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gkhivjlkv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gzrvywajx.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gnxvhnuah.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gslrhincl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpaoilrfq.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gnbudaifa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grqeduarg.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gixqauyav.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gtecxbxhl.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gyzjlztmq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gurnvbfnj.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gdwyvapwn.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjfqljwck.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gkowdqyow.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gcyonbmnp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/guernuxla.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gzbghwskp.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gmlhymaal.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gbtmjgwbx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gjhetluoi.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gquahrcvn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/giztmuizz.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/glqlemimt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gaqrzxvuf.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gszznxmyg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gsfwxunji.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gqbltorvl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/givqiceee.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/geibbzmki.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gcikoyczo.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gwvelypik.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gwbpimqfp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gsysrqpks.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gkjmtnrcu.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gbqctolci.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/ghlpcofot.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gpffrphft.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gkdhgsujz.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gdqolamib.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gntkzcggs.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gnmofjksx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gbdnogawt.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gyjhopmvg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gegtyqsid.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gnpyhksxb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcbbnufyv.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gxicaxyvt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gipmkjdhp.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/goarnjxyt.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/glbchfhfc.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/godsssjzu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/glrrsgcdj.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gfxdbtnrc.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gezrsqhrj.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gkuvjfbtj.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gqwmeuvkf.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/grpxlvfkm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gzfpjbuvt.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gnukoelkq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/grzzueqlr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gdghphenc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gcmpnasly.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gimqbyxmd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gbnzdkhtq.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gnekvawxk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gghsdisou.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/ggkqyqkbi.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gpbaxynhw.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gfrtacehm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/ggpziwwus.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gwoemibll.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gntuzydna.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/ghpdcftgc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/glbyotdwy.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gfibzifyn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gjrmnnbva.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gamdoefcu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gzgeukqwu.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gjpqoussc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gyhgqhwvw.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gptbcmaxq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gdyeifofo.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/ghynuwwcx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gzpjdikyf.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gqgwxpism.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/grdkjxzwc.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gwvojvscg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/glxuqiuzp.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gvclrguzh.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/ghnzrmhms.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gsrtvzhci.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gjtqatsxp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gkyaviglj.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gxgfykufh.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gyddgkusu.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzdwawfmv.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gbztdnusz.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gkhlaftfk.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gqbhqfnrb.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/geylzodfh.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gswdcnmyv.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gaesiczky.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gdsdtuamt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/glzyinwis.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gnsqrggij.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gtrjifozw.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gpdglkpsp.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gooytvfsl.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gfxmkuxsb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/glkoztzie.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gjffuftsg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/guxazncrs.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gzcvcpouh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/galzoaifj.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/guctlceuq.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/goxybqfkk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gszlcsvsz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gupgeewms.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gvaszzmkp.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmpzqkzbj.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/glispjgqc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/glsmfraov.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gdmjcftsj.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gczisfhsq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gkcueplvn.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gnhmuabbw.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gvqgsbxqg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gdtbjzzcs.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gwzcelaax.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/grgkrszpq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/ggolggdlx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/ggmligngt.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gbkevqasg.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gsmecmgku.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gbymngwyh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/ghweezfyt.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gactfmcrl.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gqbfdokmm.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/ggppoteol.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gqryyzxsd.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gczecswgj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gdfnogpim.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/ghcqfwxma.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gpqfmsfbi.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/glgeeuepp.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gbvhamkqx.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gwxoaojvr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gowkttoep.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/ghfudttcr.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gofysiyje.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gcloisumu.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gpovyqbbb.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gswrnamfh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gifscmtzi.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gsmpzmaun.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gzwrlctok.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gpxppasml.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/ggjbxtivw.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gntgoswzn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/goiwzgkvu.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gaajqyboj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/glbgwnfnh.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gjohzumgm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/goxinfmeb.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gwzompjsc.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/ggabeltlp.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/glzmexpry.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/glnucpxym.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/glqgdgjhx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gtavsowil.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gkroiifbx.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/guvhrzvjp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyrylhlgy.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gijydunak.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghgizpexx.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnrtclsap.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gcmbqzoyg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gmmdcnyyq.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gysbsktqi.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gjbordevr.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gbvxsxyvo.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gsklmnqmo.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gkphtobxw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gilldyddc.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gayiogurn.sHtML


<!-- 参考信息 -->