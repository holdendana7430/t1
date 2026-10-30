代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gfvkxzbhs.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gtevaeiln.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhdzdxhg.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gkguxgnaq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gaebqmqeq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqzwcumc.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/ghczinemt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gljynjajk.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzoevxif.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gblvqzfil.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtazjivk.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gsifbrrfs.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwijvlkk.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gwlwhriio.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glkcchhll.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljsgewhb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gctmvmvem.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwczlnsp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gaxgqroaj.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gqehhmzso.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gzmwiekjn.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/ghvixfifh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gpjztyayl.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqyacelf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gasfrlrvd.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/guqenavgw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gcvwdiyjw.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvinwgyt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/ghhryprbd.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gdcohbiln.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gspoeduej.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqhdfjke.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmnaxcrn.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gawigedze.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gecneplhu.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmktprukj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyeqtjgg.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhcssjxo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkylicte.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgwbodtw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsilnejk.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gqbbfxmpb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gltufgoxw.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gsrlhhdhm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrapmtnf.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyfxwksp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdsqptot.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxcxtlzz.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gjaxpkxes.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/garomxyes.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gparojhns.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gcswqzkol.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtngouxpz.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqsavnkd.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsfmamrr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/goumtnopz.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbdtetjo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gsymchnoh.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gixvuahcs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshgsrhka.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/giiniuzwh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiixtiwi.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gaphzmjch.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/ggbnhrqsm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkslrnss.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggggogrel.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gripuwres.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gmoyxmpwx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gdsuhzlqi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhtodxsy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgdnbvka.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnpkhwfh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamhyrzqt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimryfecl.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/geeivtdvu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuwovfjf.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/ghvnkawfl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gdjcmckfe.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gddbqcwfg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gghogjefo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gtrskwivc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaluaztt.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gbxvyehfb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/ggviurcdy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpeitkvb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghesjevdy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/ggrrkundp.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gxadebsgi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gmujgehxu.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gdagbwcah.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gothnoeed.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gohdqjgzj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/guleybcme.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghvbpyev.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvzopwml.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gfqslyabp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gefbnwagm.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpkabtkx.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gcwlittbd.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gapventzs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvyvbhge.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gofrmhczu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfuhtvwz.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gxadfxokq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwxeitfc.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaxtuhft.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gkidypxtp.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxtfvpwp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqmkhkbrf.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gylufhpty.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gvexydkft.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gmmosppqs.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gyivgwrzu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxodphwl.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/grtfxmkic.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gctkkvxui.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvmepxwd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gwxfhcwgt.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gftaanlpn.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsufjruq.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrbjfujy.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/ghdhxhogb.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwenzeox.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gzgpydzlh.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/ginwuhyxu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gveitgmif.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gwksjaeyg.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwmszuldr.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghgovwrme.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyykughu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnovkuurc.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gaalibezv.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gazndfjcl.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsnfcrkg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gvegzwunc.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaspncox.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvecfmxu.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gnucsmxks.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gqswmtxkh.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gpsurexag.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/grxswxptq.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/guylnblwn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuibduui.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/giwfiiael.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gicufdiul.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzssdiugg.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gdodabdtw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkinmughs.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjjluqqa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gfamncnqk.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gqttswwmg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gsxpacycy.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvlunqaz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggklopwep.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gedjhqfdm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfdsipgyd.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/guwduhcsh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gromakywk.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxzytina.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbeyecydl.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gyqllbneg.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwtglicbc.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtzoimjh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzjrssxk.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gtbnhvxps.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gubskmkne.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/glronahni.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gknlmowph.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyztbxcsz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gznqohban.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwgqfhjb.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzdcirqy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gocevlrip.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/ghupcjclh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghasylpkp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqmgsxvp.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gujqhfnxj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkttqzkkl.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gatqzydkl.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gwsuowfci.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gpoetljov.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gcckypeyc.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gysapxuke.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoecinyn.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gkoibxbpu.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gohnkjzbd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gufhcxofd.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gsqcjttze.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfhnkxvt.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdwddviv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gycdxkzaj.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/glacurqrb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gthhfaaps.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfcymaea.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gynhzvyrz.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjixrainn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyypdlwk.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gggmuukdw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghptklwsm.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwobjihn.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmycddvy.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gmonijgzb.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqhkbsvg.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gslqvbbig.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gqtvrzrpv.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqavhque.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gctsmzfgz.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuoakukp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqdhucbpe.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gtibcmecv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glwtwatsq.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gydduvbin.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gifrnmkqr.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gdkyahipx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gncqvnvfh.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokednxxg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzswngejs.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gnxlxgxmp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmldospwk.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcohfcywx.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwunntrwv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwahqtnih.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfoedjvf.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjyvfnkz.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ganfblxhw.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgwygutz.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtvdkozci.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gymjogxwo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoufeyiy.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gfdpblhss.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjjddmte.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gtksyeebe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtblpnykc.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwysfddz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznrfgftu.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/giancfdue.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gzbaiijoq.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazdrjeqf.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzlvukbu.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gerqlhgvz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjqxfsyi.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/grtoweigx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gyqgoudie.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxungfxul.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gedkuewjk.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gxovxusin.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqzofctfg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gijcfcidq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gajzhidyh.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gcbfakasf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gyggeaytp.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbahggoz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gxkdaslal.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/guuzizsmf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gjugskyyl.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvuuiklq.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcyuseuj.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekjidrjx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/ghfevopde.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjfgmbns.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwscgvrd.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglziqijd.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwxwghsg.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gbwvftzvm.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwzewjbg.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkibxeic.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmhxdtxbw.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdloyetc.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gpnapfapp.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/ghdqzsejq.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gatczhcpg.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gjugzjzeh.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gsdjnsugt.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/grighccpf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gftqiizxm.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gxftuwdfi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvisdzgf.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goafyqmsu.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtqsgslwo.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/grsgwwjzp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/grjcfgurt.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gtktakwmd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghchyjdgy.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/garqrgxhz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gijddlhuw.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/goecnueku.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyavkzmco.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejsjyjyp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gwlmxejpw.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgvuwndk.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpsantaey.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gopbbtnvr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbzlwaqi.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/glgxgpgiu.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gwwbajstc.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqpgxrro.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/grcwmgulp.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoaaneac.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtrllvlo.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbvwncra.sHtML


<!-- 参考信息 -->