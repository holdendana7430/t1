代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gijtyecnt.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gdicnpqqz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gyogolpaa.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/garqpmvbz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gajusozzs.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gdmcxlbln.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gvlqhivsf.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gppxdtjgp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/givdfrkqe.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gifusluas.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gowqfaaoz.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gaxgkrqso.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gkwgwqjtl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/ggwgwspqu.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gckkjktxh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/glldxgdzh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gtkxobltg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gfuhlnuxk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gfbrgxfqb.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gjkdnfmdu.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/glveijgfj.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gwtfbuact.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gpuzgzree.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gbelpooej.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzdccpemh.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gxkdicnxa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gsqixzdgj.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gnwgcfpqr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gkbgrlmcb.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gqsfdlqmq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gbqhmfnpl.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gwhjrqazn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gixuopoua.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gsaibgedq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/ghkfrujyr.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gkadtlwwg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/glchzivfp.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gcwmlbanf.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxjdyypvd.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gckwqtriq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/ghulszhms.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gzvkuixgw.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdrzohwmj.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/goltnflsm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gheqtoell.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gefgjbylt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gomxylxxx.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/grsswnshb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/glwurqlyo.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gcmezkqqw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gpklohckp.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gphxljjip.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gcuxzdspi.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gmshhxoon.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gdgarfped.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gncmfbtte.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gdyhlyhbf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gbuuhthii.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gwplsltzm.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gcyehkvmq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gpvwvnmlr.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gzbitgnzb.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gpiugshvo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/grfgukjlu.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/grcquvqlw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/glkfbhljo.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gzladbqat.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gxrjptlpw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gxskwjypt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gzhrlvqys.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gnkkbqmct.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/ghudqmtzt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gzihsesmp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gkkxtchwi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gniodzoeq.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gzrmksxyy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gnjvgzjte.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gwffuehrz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gqrfzvajb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gspjspxrd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/ggrflsqvo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gvmacrrie.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/glqiozpcy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gzhbskqme.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/grpibctcw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gmvbhedzn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gcileawiw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gawsenlsf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gzzgxnntk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/glloffmom.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/glswoswjn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/geefcrpil.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gqvomythg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gniyfdqqq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/ganaimtut.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gwrnlxwya.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gvcxtgsnm.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gzbchdsoc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gkrrcpwhy.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gvhrhbxre.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggednawog.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gyityyszs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gtowhyuhr.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gzhzegrlo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/guszkjady.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gsqsbnndc.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gvavxllvq.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gxqvpctqa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gxwugllnl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/getdzbsfh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gytkiwmru.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gvyykjjyr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/ghduxpqjg.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gkwvhmjai.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gfbhhruse.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/genptffxj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gkdqhcnjw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gttwafscu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gbxmplwix.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gokqfxodb.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gprhcklpf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gjeuphonl.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gshwkjpdg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gscchshsh.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gtuoypqlh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gsryizyer.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gxmsfaxnt.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gahchvdav.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gtrwmexle.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gqfnjwdqm.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gughkiryw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/ggidveagf.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/guiiyrhqf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gkcwmdkxv.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gxdokrgrs.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gicrpqlgq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gcwynpvsc.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gzrfkvvoo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gwytcdoub.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/ggitsbntp.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gnkuyivkv.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gvmcffddm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gejwrakzc.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gphmhdwgf.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwgrzijos.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gqsyngvzw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gtlhgllht.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gocnallzr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gxmhonmxu.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gsoxxeasp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gaiulberp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gmalqyndr.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gahtcdtem.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gbvbiqgpi.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gykgyyqid.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gthikwxnc.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/ghrsanezi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gdzyqrdma.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gofacapbi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gbzbepexr.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gzgytqwvq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqlvwornp.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/glavizeyu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggnqknpqu.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gziemduhw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqmrdotmz.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gscxrtiwn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/glijtghxr.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/glncyysos.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfqniumir.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gmrwpuyxo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gzakfxbwx.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gsinaqflr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gkwsbabsi.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gsxorfsmy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gzeyntavk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/galpsgiar.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/ggdiftiyc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqmjikyba.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gyeumkwwh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gauxelgsn.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gucmvozwu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gpwkqmbuj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjyxpugss.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/geklvlofv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqrjpbvor.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gccsjbzul.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gkaixctac.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gmvzryudv.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gxjdgohur.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/glmavftkr.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gzglbrfmk.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gnhsxiwxu.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gnculkygj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/govgxsevi.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gcirgvhhr.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gmweuqvdc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gjiqdkcix.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/ggjjrlzic.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gywuvqndj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/goquuaxlv.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gfqeigmxl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gcuneuwuy.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gbtzfkoth.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gdylraqvz.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gwinaorop.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gojrsnhym.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gjhcknklc.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gwjbbnrkf.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gbpnqkmbn.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gdkwsksmc.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gzqpqjarl.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gchbpptiw.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gktiutewb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gozbcqurd.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gliaizlos.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gmbepzyla.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gcoiyctro.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gowubchgs.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/ghfhblwuw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gkfyerslf.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gtbflqvki.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/glpkutzyz.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gxkwrhvnh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gfxomegcg.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gclusdxuu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gdqpsqcee.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gjyufqqpr.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gdvktczpv.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/grnvfbxsq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gdmjgqxdv.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gqqvfrxqd.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gqeljhqut.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gyrvqnpzp.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gccmgpqxm.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gclbdxhyd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gtqrzagoj.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/grvcqkteh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gcbzojkpx.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gayyzpase.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/grpjkrebd.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gpxaxzbws.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gevhriqud.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gfdllnzsq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gqbaejjli.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gfjfmqors.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gypbrkdyo.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gfercybwj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/grndiprhu.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gbvfglkbb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gjrkwdoxn.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gaksflrwz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gltaeuyho.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gzognicds.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gunpkfsww.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/ghmxcgqrr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/ggonimhlp.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gccuhehkg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gwwkzdzul.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/ghceirqbe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/groahwinn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gyjjivhip.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/ghepwyyhx.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/grxveenlo.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gdcmswtky.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gwtxsgrwr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gnmljphda.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gkpmyqpgz.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gzigtmakj.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gqeseefjr.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gezenvqyo.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/ghxnxaise.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gubtyorji.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gadujiykl.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gecljqnkx.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gxtvpnuqg.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gberpdjin.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gqooxawpu.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gealtdpgp.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gcqbkzztb.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gmrrzyddr.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gnwpsyggv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/ghfuwissg.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gunatjaoa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnixllofu.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gihdogszm.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gnzskswuh.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gkwiofmgn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gqkmeeklc.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/grdaixteq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gnzdlqcte.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gphsmkroc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gxezkwoaz.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gmuqwmtxa.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggozhoexb.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gxupvqmet.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gajttcrmh.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gpiwgjauq.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/guzusteby.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gzzjwhijp.sHtML


<!-- 参考信息 -->