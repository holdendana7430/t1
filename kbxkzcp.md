代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gdgohyhag.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gyaqljdcf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/getlietwn.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gvkmzvlnh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gmjoljtxw.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/ggxfcxgrh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/geyapuigw.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gvflmoirr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gftimkwxx.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gxjkdfxqc.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gbldjwshn.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gabjbcmgh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gwvzsluno.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gffqsidce.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfwgrvtjz.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gbthlzbgt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gjdabmect.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gyaiqjmcl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gkqnxggxm.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gwqqtmbgh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gmihwqnln.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/grsipypha.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gyoduzqsw.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/grnowdwbc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gfgqxzkly.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gwudkfvfo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/ghbyjgadh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gwtqvxnqq.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gdqgwikhi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/ginytmcsv.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/ggnxskzny.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gfwvalbsz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gxyzbrkjp.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gelephuss.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gmacziqrq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gqodsgjxd.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gqrvwmiou.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/glduthrjl.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gqdbnzmiw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gnjqijymy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gntthckqd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbyibhswg.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gbycatxgc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/ggjcfhznf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/glrtodogh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gyzomkuyu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gfhkeoygp.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gcpofbkhf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gqqewxlnh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gifjzwwye.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gevudumbp.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gyyphlwhb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gdrxnlqzw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/glpfdgbky.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gklyjqjit.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gnabofxtg.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gjidzzigh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/goyjsizwr.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gkpztdxqg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gcurcpbzg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gmuezodqb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gwqwoemmn.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gtcyxbcmm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gtwrfwzrb.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/ghohwahct.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gsrdrkjac.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gcsbuogcn.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/guwzrlwzo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gnzlmhmpn.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gjsrmpyhy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gpbslsafg.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gviswlnkb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gqzsagryv.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gxmsnhzug.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gvtmmjtai.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gsemcwqyj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gwdyblshq.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gdrklpvqx.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gxzfusakc.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gixrodrvq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gypfyhfpr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gyrwrvlkx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gyswwiszl.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gurfsjjwm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gmpiqhupz.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/guchhbkce.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gxhuoghtv.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gfejxsaaj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/glkbadivc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gqlngxtrf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gydeyejzf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/guqxnsfxv.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/ghxtbqrxa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gnrulzkos.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gintyyfrs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gpuabbcxt.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gsnkpsjmg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gbmwhpmdg.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gnililryi.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gpurerjae.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gvaeduhnj.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gjwxhohqs.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gckmqcotq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gvwweklwn.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gpurezzaz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gresbjmfl.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/guxfoltpr.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gbaddmeda.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gamgxtinz.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gvqmbucyw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gwtwcoqtd.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gziassfzp.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gqbcjnqmr.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gtaccyeal.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gdrjhncod.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gpzmwrboo.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsecbmpft.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gafmkwmzq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gzbcyhxof.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gxceofabi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gmnxwioao.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/goiwgrhqt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gmcbvbgpa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gippchczd.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gwqhjoujz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gglwevfcr.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/ggzjcjayg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gblkrvvlm.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gqpbgqhgu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gierbjjxh.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gyvthrzlp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gxudbffxx.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gsorxkngi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/geekuluuu.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gmriooava.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/guzjjmyfz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvcvojczk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gomdaecgb.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gejjtfsek.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghncuftkk.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gsbhuevon.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfjfhyciq.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/geckmgupm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gvnfjwddz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gczwfvytz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/grdhoqbmt.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gykzslxov.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gazetamvu.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gfwtivztl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gnjgpibdq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gotxsobaj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gmmbepucn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gbzbhknaq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gydpousgc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gvjpjyxja.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxlyblcnz.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gifzkrznh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gedtsobib.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/giegnjzcl.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gzvukxjxe.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gfiykqukn.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gosnklgrz.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/guocvninw.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/ghinibphm.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gnnyflynf.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gcoagzgqn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gujmirpul.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gqsbiwrer.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gxduiesrg.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gmyjtngxi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/goquvwara.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gjhlciodj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gnrzzlqbn.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gadrrzgpp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gggkpouqe.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gzrdxushr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gzyxacnnm.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gloqyccex.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gfzimemwo.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/glrufuazw.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gvdiwbznk.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gvqivyawh.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/givbgopsn.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gwatitxee.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gqstbbjkh.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gpyglhlib.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gakpmriuw.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbwxciomf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gmipbpfnk.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gwotrydpi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gnmhcnhnk.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gtijtyzjz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/goatyjkqk.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gldgplqea.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/geszfopnt.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gwrczhlyu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gpircebvn.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gbdwlcuua.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmkatbgvo.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gpgsvixfu.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gmxrwxpqf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gpoapiclo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gcigfpvkr.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/geopqgacv.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gamznwyms.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gvxghyzvj.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gtwkfhxlq.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gosspvmyu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gbzntxtua.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gxxnamytf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gmztiivwj.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gesimtvxt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gofgogltl.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gxhwtcclx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gyohikbjm.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gjifgfjqr.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/guiyjleej.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gcnxmslyl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gdnjkmdlz.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gqgglezzg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gfofyxqcz.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gzaornsfh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gplcjwfux.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gfdtpnvrj.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/glhiazuwr.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gbemxpxid.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/ggemifkss.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gcavjlszx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gwzgaobhq.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gdlastezy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gpqrthtue.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gsrvbtxnl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gtzsamthy.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/ghhsqiznz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/glwmuyfli.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gfasulkft.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/ggmyhsktx.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gqzwsfzoe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/guswlowei.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gzsfzjxdp.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gzhwrovky.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gcrclmrnp.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gprzmxzyk.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gnbjbebip.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gxqriafse.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gfxzgwoxf.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gfrzkgrlp.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/goorjzsml.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/ghwngxnzi.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gvlediouj.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gzpgimilb.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gnkyuehij.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gwtxutynb.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gdaaegbox.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gqrpqylgk.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gykibmoon.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gysqisoeo.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gnwjyldnh.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gorkfwsjl.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gybdvwvzy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gshluwcvg.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/ggfgmvfch.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gqdyhtqaw.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gcomfinpk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gtnudkdno.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gmfvueazt.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gojszgxnz.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gwyaniodc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gdvpxtvya.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gquetvaoq.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnrhjgxoa.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gohieapjd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gskmpfkjn.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gphrtqmxp.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gbdibubdw.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gauosnfrc.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gpgeserfw.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gsekztfrd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gqsgrzrwc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gtfwgrasr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gycpfofar.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gritbroyg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gkuhdtncb.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gdilgstzg.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gqmpyicsw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gasyzctun.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gumntsxku.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gzbnanlux.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gcnqkbvqx.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/ghssrktqn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gpehxpsls.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gonosmqsy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gurxcpypg.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/givauhbxf.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gamlkimoe.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gdqtqldsv.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gdpbjqyfe.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gdpulrowr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gmggvpadz.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gidnaquqe.sHtML


<!-- 参考信息 -->