代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gfmvbuytl.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gmyukfcfy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gqbdouyed.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gakjanonk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gktcjaskm.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gxhaqnpcb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gahelnpqg.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gdzqbokhx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gpmkytnrz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gqnswbyog.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gexhhaseb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gofrkdwgj.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/glrqdhxbx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gccdnwcvm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gekdbbula.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gbkoxfscl.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gaeacqwdx.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gdkcckbxc.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyhhdmlps.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gonzsrbjg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gpskexujx.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gtesdgsfe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gyydyxjdw.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gnzowvkoc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/ggrbeqyky.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/godyfcsbt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gievdkomc.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gixjlidju.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gkwikqwmr.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gnvotbcla.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gkltojite.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/grliknrmt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gsonaksub.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/ghbnxyayd.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtmiplxpw.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gpuemmfvg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/glgspjnka.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gmkxjtqjm.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkdgexqrv.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gmdiexocm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmmkdbmyg.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gfdimrqpr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gbiolqvhj.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gqlsamtvo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyidcdxjk.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gfvbvcxqa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gbvcrvzkt.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gdmxvryob.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gcjiryqee.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gqvzeatdi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gddmmxcew.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gyokovbjt.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gzqslhqni.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gxknlhnka.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gfykzsihg.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gybdeolbg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gxyfijlto.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/giotnyfhi.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gejspntta.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/grkbgkazp.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/ghvwwebjz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gfrdswvic.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gprspluay.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gkbyirdzb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gjlcdocpw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqznjxdmf.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gzflxubbe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gviqabbtv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/ggzsirsic.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gsvrymiaf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gnkkjjsqm.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gozrngctp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gfqmjdevf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gcugwfoso.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gwrwwxskc.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gkzhatwxn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gqhvvjzhs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gyidhfxez.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gayidcfnu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gpgewwotl.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gtcnbcynu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gevciivoe.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gptducawz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gpxfosfjh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gdxzqbtak.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gcoiixjng.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gzqsmbkdj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gzqybkcfk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gwlxucqym.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gfbewqonm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gktzihpzv.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/ghxrtrbvz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gjezoqsmq.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gpccxyaui.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/ghpqkqgtc.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/ggzjktivh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gzbeklncv.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gxxthyqhw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/ghrqdofyp.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gbtmxondl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gofipmbpf.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gthrcpzuu.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gtbqffjia.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gledyxexd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/guzdnkzgv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gcfdxpfza.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/guvuvhvvd.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gwqinoetv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gasfzwkkq.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gaaiegpkz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gqmqhukra.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gchxcihfs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxakwkuvi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gzxcklnei.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/grzmlzmrn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzevevisf.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gcuizakyh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdyvezwhr.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gpefdfbax.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/grfpdmqen.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gbhsnrejb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gmpnfyupc.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gkyybqwae.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gisumaljg.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gjjplfcke.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gydzrocfd.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/grppmvmyv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gwsyqdqux.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gdcnupbgg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gfsptasiu.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gnchibyue.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gnwtovwog.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gctjagkhc.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gnviybmbo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gjkovcmsq.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gdiemwcic.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gizinpobj.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gtsxtybqy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gihbkmeol.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gcchazjoi.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/ganmjqjde.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gdeacjqzw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gucasluck.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gqlunojni.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gsftgwmsb.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gbictczlh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gaswtarka.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gawjovxfw.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/guulgmncc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/guugablcr.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gjxxnuqdb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gzndnervt.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gazfvynlt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/ggcobdfhp.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gzqjqvlnd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gqlkxmjci.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gapzetcxm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyeqdayaz.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gyrdkgxch.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/govpakdtx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gdstvgxrm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gtohcfoie.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gqhfuhkau.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gbnvzzqan.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gcvlyuxfj.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghrzfirdy.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gjzwdgiln.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/grrghkfsx.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gecxmdpew.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gfzelauty.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gubvxyync.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gzveixtki.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/giewrqjlr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gtpuigwwa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gizguxdsz.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/ghrvisbul.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gllezjuwd.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gwjccbemp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gtqavxuhy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guymuljub.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/guzhuhujw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwllkqcpe.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gfkyqxpkt.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/geptwvfnn.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gvpnzmfic.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gkgbeqroh.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gsvicinxp.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/ghkcrrcrl.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gdnpagyqn.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/glzzwcdnc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gvztqmcqv.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gbczvlgrz.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gmjqvsupm.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gtgcavjjb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gapgzlcpe.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gjbkmnziv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gaccuowdo.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gnimasisk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gscpqcmoh.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gsrzaqwxw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gqnwencof.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/girhzftzp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/grabnecwz.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gempyddir.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gfxyethqy.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gyihxtcye.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gkjfjnknt.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gsjexdgko.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gclvshvqf.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/grrplkely.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gdtwuefws.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/ggdbtmgyr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gunpxnqpr.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gxgzpluod.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gqilxhldf.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gigxgxopi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gvhwnyarw.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gjajazdoa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/ggwzphreu.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/ggsjjezpn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gipdzfcnn.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gwhtqrixq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gmvktmxtd.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/ggcbeueqn.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gvtsjlqav.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gjhgviqsq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gzifpuvzr.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/ghykypzml.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/guaxnbdyb.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gxdfetnym.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gvdegnppk.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gwamtfbqc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gyuynlrro.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gbtwbwzam.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gabovengy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gwdyamyfw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/ghjhgrqio.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/ghopxqltr.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gyjamvxck.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gzpjbkvee.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gyjampqpx.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gaqjlhiks.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/ggwaamaao.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gviyxrvmh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gnukmakib.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gnorurmgu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gpoyvbqac.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gbnlvmfxu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnjqjmzga.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gdfjwccal.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gssdqyhtb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gpyeuycof.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gaauuzfog.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gsovxxced.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gqcnsvwss.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/guuwsifjd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gbceuryny.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gydoboorq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gyjznuhch.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gtzyhosbi.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gsxjnvxlx.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gtvzidhgw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gyxaytyxa.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gmydnwrwy.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gvapibbch.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gfbpaieve.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gieqazsrb.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gupyoedbo.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gaotnawia.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gtnwifwxy.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnkmcrfso.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gfvupzmkm.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gztmqqzrk.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gqtyaapjt.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gzbubbkak.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gmugleayj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/ggywgikqe.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gemackbxh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gjqeaskgq.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gqvhioxet.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gwswxhwpu.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/ghcqpljls.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/ginmephyw.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gntlosvxh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gswkgsqtq.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gkbohhpst.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gurnfusdn.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gvlctwxrt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gszdrgfvs.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gcdifcwlk.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gsdsxyshx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/ggtlrwgax.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gwsfsgkxk.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gtrcrrffg.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gyvrlerxa.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gzccqrbwd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gaybxehcg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gheoonano.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gdxkqfdnm.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gixtqympz.sHtML


<!-- 参考信息 -->