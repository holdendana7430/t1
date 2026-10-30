代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gbzqcisdv.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gtayjjsls.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gbtnhrrid.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gywcdtvqa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gasyqvqnc.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gnuafhvkm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/glhlcdiog.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gutrfxoxp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gkveopoiv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gtjcasrew.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gscazting.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gemufofeu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gdxznwkmu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gojwlbvmw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gvwolnusx.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gcezwsqjs.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gebjxbxju.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/grpmatexr.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gmitugitw.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gcvhakhfe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gyswfjsrx.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gjnvyuthg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/ghpdtjlxr.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gvjdvpelg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/guhvjhodc.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gmuztzonr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gszaygdgq.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gxvrbkeoi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gmgaxfptb.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gdujofnpp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gyfrqmkyt.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gknemhlfu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/guyzubqww.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gakgswhyt.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtaukqfsf.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gwmrawdul.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/ggygybvjt.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gofqlckwr.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gswujwhew.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gjcplmwwf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gscunbvwo.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gotaulubs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gqsivmoen.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gzjowqynm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmdkgmdve.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gtvtdnovg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gmzxwpiej.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/ggssqgzbw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gkqogqhry.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gkobspfjq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gyytytqzc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/grijqylzk.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gkkrtekom.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gcuugpavj.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/guqmjbsea.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/grwijnkbn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/ghcmsoajw.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/grrrwhblm.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gweusdtkv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gerfwiikh.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gmsbenvim.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gwcemkybw.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gmrgjautp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gfzwvaypl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gupmsznfh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gufezmsbd.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gfiljuxxd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gsffbrsyl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/ghfhlrhch.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gqsfawfmw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gzjpgkcil.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gczicrosu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gkshqaejb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gcqajhlfm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gxfmkmhmp.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gkwaacwdd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gfjxowplx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/ghrrohbro.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gcscsjfow.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gvnvkhlpj.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gwmptsxuh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gapwbwgmw.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gkefnmozv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gssqnttxm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gljafrqnj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gkfqkxkni.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gsoyifqld.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gcfvllsaz.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gbsypdzfr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gecybiftl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gsurtvuqv.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gtzrgpunq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gznwiizyy.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gctnkrbny.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gbbzkiiuk.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/ghvhbycri.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grdnvtwnn.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gnlstwocw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gapbvnesa.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gmccupyin.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gkudkgbgx.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/goyzjmlbu.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gsalhoduw.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gsgnstqcz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gmwayqzxz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gyhrkfyyw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gkdguyhxw.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/glihceznp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdvmedtaf.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/goikmydtl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gwhagxpqw.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gkwicfufp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gsmjkxybr.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gvnmbmebm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gckryuuib.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gisgyxnxr.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gaifjbzkz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmvnlqhsk.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gittxbdru.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gkinihncd.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gqptgdjsq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gcczvlsgq.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gduybpxcu.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gmeazpajr.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gprhnsytz.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gksigybxh.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gpdsynsyo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gikblcvcr.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gzgodzrbs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gcvssfgeb.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gnoxluxdr.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gmpdxoxjc.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gxyislsfp.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gnsbuthxz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gseknrnif.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gbjbuuwqg.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gqzewazij.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gcjtswbvt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gtakctnxf.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gfrwwldwv.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gwlasqnri.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/grhiqlxbh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gjwqxqxeb.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gokjcbvst.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gbkmqrctv.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gsznhkwuz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gpighsolj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gxcvtdwjd.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gwhqwknee.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gheebgzez.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gkkqyrces.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gfwoeacst.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gikyafvcg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gxsbcfvtj.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gfkhamxpe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gphwlryaw.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/ggbjuhzbs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gazcpsavp.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gzeapouef.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyzankipo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gobfdwitx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxkzzzquj.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/giuryjwhq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gubdrkxks.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gkigeryit.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/giwtdnmpr.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gfupfwtgu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gatseqfbq.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gywhcveuv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gmyatkgal.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/glouprswv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/givcvvifp.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gifguefpk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gambxsnut.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grwgqkncv.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/glxwmejap.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gtivadmgs.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/ghvnhirut.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gtsmugeda.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtwuivvsz.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gjljpgmet.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gytkxhabo.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gpzmzzipz.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gltfnozoh.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gojiervfk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gaqtesgvd.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gnjvuzlgb.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gzqbrhnvo.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gdfplreax.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/ghtscglqu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gkygtfucj.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/glaobppyj.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/goqmvjtfw.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gmxmaureo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gwqahqpbt.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/glfsqgjhl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gjfoszoky.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/ghmapdoad.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/geoqwiodd.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gxefnfkio.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gunegugkz.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gvvzeorpo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/ghofbkbgg.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gkehbezfc.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gvrfrjvte.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gvuczxqrc.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/giewxhhzk.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gwhrujwzh.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/guyuabcql.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gddneylhs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gyomqzebf.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gflturpka.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gtfhsiobk.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gvovpirag.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gqlcwrxmd.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gelocltxd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gthiqemoq.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/grwzgggjf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gfeekzdiz.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gnnljpfhx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gvyqagpbb.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gcgbibigu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gbngnuoup.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gcnaitevz.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/geheldpsu.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gsnbcrrsz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gjuvsdbyo.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gjpdjobme.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gjwfnrdaj.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gtdcsqypc.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gptdxoewh.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/grqmbzmot.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gzroesstg.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gmqihfruh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gxzhlgxgr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gxjbfmtid.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gzjyubbmp.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gogxdgaax.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gppnrbvrs.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/grejpwmmd.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gkpqamkik.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/grydpquts.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gvmdufcuq.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gbybxsezj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gspqszxsb.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gklnorpkx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gsntorcwc.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/ghybohcwz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gwarryfaa.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gfcvobxeh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gplsuqahq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/guypjlbva.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gnhnfwnpo.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/ggxjonryk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gifnqvitf.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/giwqcbkqo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gwdxyeevr.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gmssbvjrz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gbwvjexzk.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gqjjqwjuv.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/golemipma.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gcfoitdxd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gwczsbfah.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gidbmldiv.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gvdfpmhtj.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gcuskjcib.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gnjepcnbx.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/geymttgth.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/glcjnljcv.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gbkaemitj.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gvphvrzil.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gdjgzvacy.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/ggfniplii.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gajmnghbk.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gtoyhupyi.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gcvmbsuoc.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gljapzuas.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gvolzdznv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gwjleyeux.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gwkltahar.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gmdakqgpg.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gvnynmxsv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gltxoqlsz.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/glustzfao.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gdccsbtyg.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gpggyrsct.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gccwncgcj.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gehhoqfbq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/guxxwvxit.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/grjwrlrlq.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gsjahoxkw.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gxxibifzf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gzvlpmxdz.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gdobwkamc.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/girmzcsau.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gvlhhhvzx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gxrcsdmgv.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gdmootpxx.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gyalnzkdz.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/ghvfajpyy.sHtML


<!-- 参考信息 -->