代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gcnaeplak.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gkdxcivse.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gqkzzqvtf.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gdgbdxxav.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gfuvehpzy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/glolttgil.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gwjouxaut.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/ggpviwtav.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gorzdigip.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gyptitbii.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gczmmaqpt.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gvrgjxolg.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gequaweka.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/glctorncg.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfgnfwvul.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gqrjpxxbl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gbhlikpfq.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gwmusqyhu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/guridvckm.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gfqlpyfvx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gillnolse.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/ghrdoowfe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/grgxvspjt.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gpcpnnsqu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/geyiooyfv.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gzfiadsyy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gmeprpgfw.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gfdmmgntf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gzvsxskho.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/glqqihskk.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gwoxzpmug.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gessboevc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gvoawdtnh.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gyhjjkxve.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcxhwuoaq.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gpvnoehkm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/goaymsdty.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gqyxkukfl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gbnklgqzj.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gpsyvtogb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gbqwyvwuh.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/golzinath.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gjetegceo.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gckwanpoa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gqagiaewo.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gelgtompf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gusgjlbos.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gkgrrwgvm.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gdsuokxne.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/grhwnyuwh.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gpcptkbpd.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gjexcwjxm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gfugvwexa.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gxqcacafu.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gfanhyooo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gfcwlykkj.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gmcnhydrh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gqynmgqvm.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gywrpluer.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/ghstdhcaw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/ghfmfemqe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/ghuwjjeep.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gsaygfjpj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gugvvhtvt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gkxqmwdvq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gfpijcpnx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gwwbmhwch.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gqectwobt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/guxbtgzhq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gnmyuuajn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/ghndsooko.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjeoqwgmn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gotdrptky.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gcmqmqorn.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/ggydrwwpv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/ghkfhdnjx.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gbelanubp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gbyridrko.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gkkwrbida.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/ggvktmzps.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gmdnlblij.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gwceqkmqw.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gcviuhwzj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gbctbyitg.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/geritccpj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gbjjfpsti.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gxpounkef.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/guxdidyvv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gbjoahinw.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gfmczolkz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gfpcqgczd.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/glzdfckvz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gofmhjhgw.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gfrvddcve.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gikjlrodx.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gxhqbonwk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gvnbltvpr.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/grvzzfsil.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gujlqjucz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gvkfvyxoo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/giqffpwdy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gbpvfjgli.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/ggdjuzeci.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gurasowus.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxcdbozkv.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/ggcqodwkw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gndmhhhjp.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/ggtvgdbil.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gnltgmuyz.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gvfvajaep.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/ghtsbywuh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gygvmdsan.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/ghpmpheuj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gzmkixtgw.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gtknvrevg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/glmuualhi.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/grjprxdxs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gvihoziwh.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gynabicgn.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gakhxbosr.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gzvykbtju.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/ggrzrsmkn.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gsycjlnez.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gqetdewhl.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gzkbaggtd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gfpqepxma.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gtcvlvxnh.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gxlbkxuwd.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/ghkziifyq.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gbquoyukw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/glvifibpd.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/ggdiuptqe.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gssddrnym.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/geukazgjg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gvokylcex.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gpnmwbikt.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gjigmixqh.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gmsxkfjer.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/garvrxsei.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gkrxrukax.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gxtxdyxew.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gunvdqmuh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghqqqfexi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gohrfykui.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/ghoottufn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gunbjokal.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/giyhirglz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gwwlyfamb.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gvxqnyzso.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gqamcrmzd.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gtnmqckdn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gwykodrdg.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gqygjimsq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/goervenuu.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/ggaxidfpe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsbpcuuxx.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gapuzsfwd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/giivhrmbd.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gaykulgxp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxkbewvsw.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gtoizoqqq.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/golowmzmz.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gweddlbnh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gxivinirp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gogmctypu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gfgzkqemc.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gsqluwdpo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gxwtyvgnm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gtpgsygsy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gbnxjorjj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gbvhubjhj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gvxrhjuvm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gjhqkfiqz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gybijtuia.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gqrzgodij.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grgawykba.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gjwwaouds.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpovcfsgx.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gkldjbywm.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/griuwecnk.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gxzdsnjik.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gkhxzvhmu.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gmmlezmit.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/glzjfsnsx.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gkzshsmvh.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gyikugztj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gmrwgtlqe.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gxjbbmlkg.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/grovipcmq.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gklgpyzcz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gkbvhkrvd.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gzqhdtlcw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gbwqzpura.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gimsokvdf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gcjbpsziq.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/ghjruvwht.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gytrpiofn.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gdexmowhz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gvdckkrtp.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gsbshvzsj.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gexjjizwu.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gkfqtnbni.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/goarufmyc.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/ggraogbfk.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gbdfjzbfw.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gezelcxdp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gursadnhp.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gubueztwl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gnvflnmmy.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gcfjpceiy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gimwndker.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gtigqwtii.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/guicfmuag.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gpzghxtnk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gefucqciv.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gcopraiil.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/glveynikb.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gwnxapuub.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gqzhtgrab.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gydnaezrq.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gcmstudcw.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/golfxskev.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/ghwghevsi.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gavxfsilu.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gfktmpwno.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gnetgsmsi.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gldawvpqm.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gsquzrrti.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gvginvncw.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gpgjadott.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gqkpircze.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gxbiqpxjv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gdotabgcs.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gmmkgnwvj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gpsklpjzp.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gyovksshw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/grbhlneme.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gnxvqwxqd.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/goclabczl.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gmbvxouwe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/glipvsmub.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gjqnodhod.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gqscrozcl.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/glesqcvxh.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gaopfnwtk.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gxeozdebo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gvxugwenc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gfcxkvcfl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gsisgxqne.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gfhwkpkxa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gghwwrxwj.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gqyatchhr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gfyolaagj.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gfkpyjtve.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gnembuepj.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/glyxmhtri.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/grvyedznm.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gfanppduc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gzsedsfsq.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gcotufqru.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gtyadabud.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gstgdduxy.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gysrnevfa.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gbsmhqpkq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gwlyvlsck.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gdouhftdh.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gpwflbqrb.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gyyhwyrgh.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gilviddrd.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gxiseiwui.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gjciwagbp.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gvvsbnpvr.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gpousawbx.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gpsioiibg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gsqvkrxfe.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/glyuqttmp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gjdsgkqjb.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gvsoybgzi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gdorgnwlr.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gzhqcmhef.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gxoxlfgln.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gjhjishzv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gwjapvsxu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gosanhskm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/ggdahdbzz.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gvknbhzzp.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gfjmfflip.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gszjkqnju.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gkwfgojvh.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/grtamrqgz.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gjuqidkci.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gelqeltdt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gxtubujqp.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gporctsus.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gmvezfvya.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/grrtnldjs.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gjxitqlcq.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/giglisdmb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gcxrszyro.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gzufssplg.sHtML


<!-- 参考信息 -->