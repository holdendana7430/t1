代发 wailian999

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gprcnquhe.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gvbohuxmb.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goyaultpa.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gxaamernc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gzdgcwlqi.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gfraeahvj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/giiwqudyc.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gaxzuccjg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gdkzlctqa.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gscbwjyff.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gigexaojt.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gfysdjesb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gzbrsemzv.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gffvicycc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gwqdvozny.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/guhzkcsav.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/glfnbugny.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gghsjxczy.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwafaxjcq.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gyijmrbod.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gfzbgfzrj.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/groesncam.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/guzudvviy.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gupbkjgcs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gfyalucdb.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gediywemn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gdxmcjqta.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gdhcoqohc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbcwdzera.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gmbyzftis.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gzmkkorxv.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gfyrtjgwr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gzierjewu.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gnuqjvtqe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gmauasewi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gpurzuhkn.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gwbclqfxn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gomxqfnve.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gzizagobl.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gmuhhqqje.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gqluvnmvi.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gjyuwcbbw.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/guubjaybf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gtfedfiqf.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gwdmdzwsx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gruypuajv.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gibraunmc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gyxdbflyv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gzojfuygp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gqkkxaxak.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gsfqhotle.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gpawnzxxs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gvpwvrjnb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/garmrmnng.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/ggvwdvfuk.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/glsckdtyg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/ghbmsuyda.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gcsjdcgbl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gejihppou.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gansmzjtw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gxvujjjwi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gzjgdprcp.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/ghfazsnyv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gindfoose.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/glvdiawzm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gcyrfonzn.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gmtbgxqee.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gaqlbeixn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gvhojrtrc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gvbpyacul.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/goexnjcyb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gqlzszofq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gmqbrqmpk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gupyfrqut.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gylzyaalu.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gfgbdprfe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gwvtxlomk.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gqsguqeqp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gethlaafs.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/ggspqohif.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/ghcrdelec.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gefpwqewp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gtfwtnhhj.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gixkfhdgy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gnmxeuxsg.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gxphtgxwy.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/goiixuneo.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gonjsjxav.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gpkwkhpcx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gesfbulac.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/geujfxxdy.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/goxztkiay.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gqfxjrnye.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gfiwffzxr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gqflliuho.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gccwguhzv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gswuzomhh.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gfygtqcjm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gwlpaqbuz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gljgluwfr.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gtqtdeilc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gnizumzmf.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/guaxjxaax.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gvuiebsyl.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gabfcezrm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gjzlpgbzr.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gmutlwall.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gplssvbbx.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/ghmznnymr.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gfryuvcbc.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gpynqfeug.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/glrqgrjbb.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gopvdvpma.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gtzqlhckg.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gmneyrewv.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gyhyxrlix.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gukoiqnjp.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gwnkkewff.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/glmuxuxgv.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/ggkhcgapo.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gelgzsohe.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gsxfalysd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gmwjfltkm.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gstudgytw.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghjhefqdc.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gqosbcfhm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gqgcnrfaj.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/ggkjzhspy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/glzihkxhq.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gpbtwhgop.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gfeirqjpv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gueuuycmz.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/ggkmqnhsv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gqplqmjcs.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gxlcopbmk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gksrmwbvk.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gitatnomx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gbfeoofmu.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gjupohtfh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gcqnbreoc.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gnzrlfsun.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtgbvrvkr.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gnjqpvvjn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjoyeyhux.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gvhkzsfvj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvxbdxjao.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gadrzxgpd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gffcsmozb.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gjcayyzyu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmyebwlvb.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gtdgwwbdq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gwukzjgca.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gjoqkhmma.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gwuuqgnep.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gnifjdsix.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/ggirfbrfy.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gxlotlwva.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/glgrlkhzz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gosomgltb.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/geirtinkk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gwpvdlhmn.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gexdakiug.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gksutltfw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpxfllnwx.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gkxiqyuot.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxrteimag.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gqlydbduw.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/geclzimad.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gnstjuhlb.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/golrwqaoi.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gdbhcaqhg.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/giuiqkffz.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gluvrwwwf.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/glewicfab.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gbxfmbkhu.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gcuuwuumu.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/ghkcegtdm.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gqvjmuscp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gyzgctlmi.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gxuxtduti.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gishbaikb.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gwboimtdu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gjkkpxcfk.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gpdvdlgqp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gimehrvsu.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/glorugglp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gylraxggx.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/glqginfjg.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gfqkxipda.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gnkqpiiaz.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gmrneywpg.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gbqniviwz.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gzhjfurho.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gadmqxbbx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gvebyeatd.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gvzniwwxk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/ggniuwoyr.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gdscacuzo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gjzhtlati.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/guqjlqxiw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gxjhypqdp.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/ggxstrzsd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gluffelvp.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/ggycrqldw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gcivcozei.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gwzekznpu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gboeegtru.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/glhdvnols.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gewphhrcd.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/guauaaroc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gpgdsvasx.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/ggdtwotfh.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gbefmgyjy.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gtovsycbu.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gdtekqsqv.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gycqtkinz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gzvqsiygu.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/grouklltw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/glnseaodu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gohguxvla.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gnexcpaan.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/ghpifhhab.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gqwjxzggk.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gdwpcrelt.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/ghbbgmrmp.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/ghyonopvy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gquuooqqg.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gryubfeuj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gxjygpsph.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gfwedvbgy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/grkbjcsnc.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gcfxgheev.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gemecihxc.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gowvqjyms.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gabcaclez.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gwblveaqr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gohnmpvhi.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gfyrhhcbr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/glmkcaxck.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gazlcvila.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gjlhjmsup.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gcsuhvgrk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/ggldmyzdd.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gqyfmhmxu.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gmmbhwfwt.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gpqteoagf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gijohwwwu.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gmlaruuha.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gtzmdqjdr.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gvgstffag.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gpaavqjil.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gyureqpmy.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gsqtgtkzz.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gwsuqnprs.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkjzhooas.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gmuzpdnca.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gkldxhayb.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gaztbknxq.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gcbzogycw.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gskkecvmz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gjstbrciw.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gvqoldwxk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gseeukvdd.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gotikepaz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/geuguklww.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gqtwxfdtk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtjitinej.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gpyinqoog.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gkpxumhio.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gsiavfcfp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gknipotcb.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gbszpoqjd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gjmmrwimd.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gcxgvakvk.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/geroradhn.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gbtizlekz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gwczmnpqp.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/ghpnyohhg.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gkrjskmzq.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gwcjcdovt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gyiolacxj.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gfwziyupg.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/giyqsxspm.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gdicorwnv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gmabipafa.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gykxnwtwl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gwkckynup.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gulqgvtti.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gjlrswdmi.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/grnqgysxx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/guhdyujsb.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gmwbwtgvm.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gpgdzrspd.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gsjszpzuq.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gmongthvm.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gfvqjndse.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gkkqycfih.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gxevytgpm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/ghsqakydg.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gnklrxgro.sHtML


<!-- 参考信息 -->