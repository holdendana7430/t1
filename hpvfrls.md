代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gdiswrjsp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gbksgktrm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/goitzjspf.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gduwwzvuh.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/ghbtsluky.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gifmlstgx.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gaymooqbe.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gkqetqjup.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdtvghshm.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gkduborrh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gxsnfnjsk.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gobrdcjtu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/guntsbtcw.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/ghmimnrue.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/ggagwacip.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/ggagbdqbu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gysjttbcq.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmywhmjip.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/grxjgkpnk.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/girkcijub.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gcduflxty.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gxyjyrkdy.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/givngyrxv.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gbzsucnbx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/grquxvayn.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gmgzepuuw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gubkwbbvf.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gdmxvrkxd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gbrxqbnnh.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gkydkeymw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gaconbuln.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gdbsheiuy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsohnjgqe.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gcyphalda.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gxgzovfet.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gwiuapetc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gktpdrsff.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gtwcidxie.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gavqyauic.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/ghjtkqsns.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gmhvaqfhb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gyowdsygg.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gibgqhxxm.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gjaednkfw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gxbyjfnpz.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/ggkhnnrhk.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/ggaghtdre.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gztaruiig.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gqyqdncxi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gonuhqfdc.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gtfypfikc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gjextqgos.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gwuxjcdvl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gnhkxpmll.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gepfhzhxh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gmbkugdtb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gmrpfbtlh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/grbpshifs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gnlvpxlhs.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/grclsahcq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gdzylpxoc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/geqjbhdls.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gxoluwluz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/grclaqspj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gzkdthrsv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gblnfbwry.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gxhsfhihy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gjhgtdzdq.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gdkcihjeb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/ghqkckdya.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gxyhmqlua.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gbvbwikxn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gssxvlrlu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gvnwdderd.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/ghpxuurgz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gissjulqc.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gxhvcbkyl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gnljcraka.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gwxhtjwuv.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gvodxbufk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gdijlwjst.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gcewdvubs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/glsrhycpg.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gekfkrlfg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gmnagwuog.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gwjmzzezf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gyyidqqjz.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gsjtitfxp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/ggckvajil.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gfxdzywzv.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gulfscygk.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gbghtbswv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gsiafqxtf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/grgigqxnp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gqlqfvchj.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/goftmwwsk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gobrfzibl.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/grvgurojn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghregqrph.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/geuebtlnf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/ghnteswxq.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gydfgzirz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gzajihzgg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvzfjzyr.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/geucvzmmt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gemvytnzz.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gydyqpenw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gayutegev.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gowgqnhfb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/goamqlmzw.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/grrjqwpxn.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gvbgrshax.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gyxgvtqzu.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gaujanklr.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gflaqfbpr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gdlovcnfb.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/garhhacpn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/ggsdhygzh.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/ggmdyndjk.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gsssvivjk.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gwltgbruq.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gwrjtujzg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gkbpruadd.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gwzvnkajc.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gdmsosfsk.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/grnhthraf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gxvjhsrqz.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gbdwcrcax.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvbxexkfr.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/ghjkpmbxk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gufyutekc.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gpjriyynf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/guzlxqwhp.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/ggiqjgqwq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gcidzlmro.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gwmfanpaj.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gdewsgtvd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gpjdurrrk.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gzaafwogt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gxppbasrh.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gwtnaveej.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gqvlcbsdb.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gkkpgvtns.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/glfijvpaf.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gsqfxbmoh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxkbdalol.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/geczzunnp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsronmwrs.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gobkdsevd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gziwihoms.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/ggqhjyzbk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gonhazptu.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gibihgtox.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxstyznha.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gdbyhtvfi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gysseykgh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gyhmaoyce.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gqgorrnav.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gpvtsoodb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/ggzytgjvl.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gktyimdnb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gczfskafg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gfwcjvfdd.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gvrwvkxxx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gefhdtwjo.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gklytlujf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gsktcpqrv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggdgstmrb.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gnbrezvdg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gziekxygn.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/ggquqfbfb.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gybujoies.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gvzrxlcud.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/ggcwdxqur.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gldybemqc.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gdsigquhx.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gvamqkbph.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gtmaqoxpg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gshonfqek.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/grgzdullf.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gerfmmeig.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gwmbfsjce.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtspemzkq.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gdxtsyuso.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gbnbatbsl.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gshdmomaa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gnxfvxhuk.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gmkijqvyi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gicvnhdym.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gjjeuqtos.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/guffrukhe.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gppytsxtu.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gaawwqhht.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gipetxrak.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gesxqrlna.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/ggkxmbtyw.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gixceuffi.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyokwxxts.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/ggakfufhs.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/ggsabzaxa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gkammxajm.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/giqoxuiei.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gviyhpmwo.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gstuwmhac.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gefrbslpm.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gfkcsbeqw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gufkfgare.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/ggeklrvuf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gjpgqrxfm.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/giskjpnzw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/ghhwfvsmu.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/geofaqvoq.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/grjymllqz.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/ggedusmjf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gcumkrlos.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/glqcplszk.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gguopjvie.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/giorrhdhc.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/glfpepsgb.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gdxygkjdc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gthrahzto.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gctxxafjr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gjfrlyfon.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/ghdmyckos.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gfgmoqdxu.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gnubxybcq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gbcojgxla.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gmltafahm.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gxgqwrtev.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gwdvmvyyr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gupqhfqrm.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gxknxrfxb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gilfjizzy.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gsbtdxnqj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gamwblwel.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gnktkaufv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvkctujap.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gdbhwzmyb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/glztdcwon.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gmlsnksii.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gvxdfgefm.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gncudevap.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gransmudc.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gcbctmgsq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/giwljyxop.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/ghforvpzb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gnufdumiz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gjcbchujr.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gllngugkw.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gtwvkntpa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gtuxvtxzh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gsghdpghj.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/grurfsmyg.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gjvdaxfwp.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gbslnorjb.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gefdwwtcn.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gtawdxcpd.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gnaptisgw.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/ggosqcmky.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gxfgjxohu.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/grjvpexfy.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gytrkxgar.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gfjeufwtc.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gzrcdxzcq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gzptibqhp.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gaovheebi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gjodejjen.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gzczgdzsl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gmcoxlvfz.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gxeruzhan.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gpmprgeda.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gixrqdxlo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gcptrvzqx.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gsnylzwzd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/goarocflg.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gspsuvese.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gghnyvefo.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/goolwtjyi.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gcyfybaax.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gmzppoopq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/ggcnwgsbn.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gfbellpbt.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gzakipdvi.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gohkjzrwy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gzzvsyosr.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gldzhzffj.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gwmxfquqb.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gclngsglm.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gdcxdqygw.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gnhzmoiio.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gupljijey.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gtbeuljjg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/ghmfjobyn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gzbawsjwq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gjtdzvmxb.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gtrtnzxwb.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/glyzomzcp.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gtdpyvrpx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gzuogtkrm.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gzkhoakrs.sHtML


<!-- 参考信息 -->