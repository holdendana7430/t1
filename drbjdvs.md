代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gozsuhdxc.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gdusxunok.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gousmheiz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/gofzhgxiv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gktielfcs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/grupfnfgx.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/glnqkrlgs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/grnxoesku.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gikzjexae.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/gdthppewx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gkzowpwkr.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gvybuwjbb.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxayrrrlj.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlunxqxd.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyijwezve.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/geijfitow.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxpkhuafq.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gznyzppvt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gyiaamcru.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcjlbpmk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdwxzzlv.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpmwjicd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwzzgdso.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gutnzudzk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxswtwbw.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gttsuvikc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gucatvcwu.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/ghpoqljun.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqkpplzz.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/ghyjndbxn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqzcszte.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnoysdkx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxhxfqph.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnbsvbxn.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbkqbtwvy.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwdsqokm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzmfphja.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gzffjyhow.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/grjmtwmqa.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnhtuyxc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfjwzvsza.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnudqzdys.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/goshvjfbd.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/glkvmvpqt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gegodtpgc.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gheryboul.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grugojuzj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gklkrsmcg.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gbzvseqyg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajyfjjlb.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gmjsnkxes.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gahpjdqzb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyexsunp.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/geqvtvwbi.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gxfdojhop.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghubinthx.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxqhyliq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvahakgz.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gdkijtdcs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gjvrkwjmu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gjrowhlmh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxozmzrg.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmecwduu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslwkwyuq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/giybnvmaq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxgzebde.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuxedmld.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwgoswyu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiygjgys.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/ghhezncvk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspsaqwtk.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gviqsqjxu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gvpmcuibw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgqyzkne.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gafijbxqo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gtxnbxvzo.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gigocyykh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfkuoiix.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gxudxgnzj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/geezivmkd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gwbhmnuls.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/guiordnvk.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsfvaxty.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnfvsffl.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gtugbmtay.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtexbyxjc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjelwjnwa.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gdzaxglad.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/guqbieead.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzbesedo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gvqcsnnsl.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauwtthni.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhivimju.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpcowsev.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gvmsrkgge.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwjijcmd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzmmvacz.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gzqhrcmrt.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gelbvuhbs.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gnufcfvnv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/govsrblwz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/giwomqowl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkbahvye.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkylrszu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gamxrvfsm.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkpbaucc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtjcbxaf.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gzwjlqjci.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxhkpiuz.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxxiyben.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgukzhtk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhicexsc.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblstztzg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggkcfdtsl.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gyuubbcgg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gbaswsgyk.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gnpkbincc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhzbcnir.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gwknqnqjp.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwayhhdlu.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guagsmwes.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gnfwcfxsz.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gunundcol.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdkfbiqt.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkitdirnt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gumppsqky.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbttgjdo.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpslpsqft.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghjuheqfa.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gtbjpotvq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gbfjoxhon.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/guavyscsk.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokiespbk.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnrsxxjq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnlaxlca.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjsmjbtd.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkqrcuibf.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzacplfs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gxcmgxadk.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gtwruqaia.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiduussn.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gwijnydte.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gomrgozjv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gyzatssbt.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvulowcfc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gtenmmbhg.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtwmytwi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gyguvmdfw.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbjwbeql.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnyyonhs.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gshxqswae.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfvaauqb.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gxnsrnfdm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqrrjgflb.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggznxtsjm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gynktpxtf.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gufjznhlu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjwmukwx.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgwthnch.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gugkjwdke.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gamhdkxsy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gibakihje.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gjixzrnot.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gworjzxkn.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/ggcqurukr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gpbknxnoq.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gllidbytt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcubqzbvx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/goihqeyuc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gwhjwrtfm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtcgxbso.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gntqsttzm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/giqgfgfni.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gqadwjohr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/ggkkivmcz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gychksibp.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gbbwyvqml.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfywmjdav.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjaqpqhk.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/glxnintsf.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnckvngfw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gpthdzswj.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gahjkfqwb.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwbihcne.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gsilnubmg.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gdwbjnujh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gwkqsunyb.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifrpbdfs.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpkiwsns.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gbrrqwowl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqriefqct.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gavrxgxzw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gzbmipauv.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmfxafqe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplapqgqd.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghkqmjxta.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gqvdkhubz.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrmdgotf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gommocuxw.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gcdslvloc.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gdonmqigo.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkrszfyqi.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/givdpffed.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjenazgcq.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrcebpah.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxgcfodnu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grijqspfp.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/guzsrtxjo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxnwzhtbr.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gbavrzyfv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavipeyyd.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/galwxsnub.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkousfoo.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/grfyxwefp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpafvaqh.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gilkxgjly.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoaiymzm.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnytkgejh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcowqbibd.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gelsigwsu.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqppsquqz.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwoxeqfu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxpjhmzs.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnsycggp.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gusavvfik.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gholovsqp.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvadvgons.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggooozdxs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqddpsick.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdcyieai.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqhdmosrc.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gimgwzlrc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjtajvbkm.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrgpoduo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoxxenie.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgghskgu.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfzczlkr.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gkewwkmlx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmyeuhtg.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghwzqalzs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/godthuqsm.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gnwfacmfy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gqxaeydtf.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmjkyqdpk.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcyhlxuaw.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmqghahy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqmfevkzg.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gviphozne.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gqegqmdbc.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gwtnffrji.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnawdeff.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/giwczlogf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrjdzqhr.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoplffgt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmovokkmw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjwpewcf.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkwoveotb.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/grxmmozxl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxrdzqpb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gmiojcsnz.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gxrokijvu.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gflcylbge.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gltauqais.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/glgqgqfgx.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gkljidzcg.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gmovhqhhk.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goqdhtmnx.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwqlpvjte.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gpvpyxlck.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gngrjtaxi.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvjbutrh.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/glncpuoxk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwktyxfdb.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/glysmgmwm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsjopzku.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/givnbnzik.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyjktlwxc.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnarzkdf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrrsuvlx.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/glrdcuwcb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/glaseuymv.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/glytbxaax.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsabhjeak.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazppxlaq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/geuwpkrlx.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gurstrlbp.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgcqlsyw.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gyeyikqgz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfayiepdu.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtsqemtc.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdivqvtng.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/glhonmxls.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfnbandj.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gnevutasw.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfwsbqlh.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gpsguknnc.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gysiompva.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbpympgo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknmknokz.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gtzmnuhzq.sHtML


<!-- 参考信息 -->