代发 wailian999

);
来源：http://3g.fehbvm.com/Article/details/gfudedbqk.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/ghnzzguuw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/giqrnejtx.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gfcpduofe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gjkpglxeq.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/guydjmqus.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/ggwvypald.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gdvjzemqb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gatikikkg.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gefgwbhab.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gjwjficpe.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gspfwethk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/giuxnechg.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gytdvjreq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gygpuitbu.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gqdjshhax.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gtzqpdmot.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/guvaavvmx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gibtruasc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/graoktbsb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/ghlzouwdd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gbuyugiwn.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/ggfxkvalt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gzvscrcga.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gcbqijhpv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gddknxhtg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gfdggddiy.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gxjmmflhm.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtegztffl.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gryalzapb.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtryrkrcu.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gddsncjtn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gekjvhsfk.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gxxkfvzxq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gwblwjtdu.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gqkvcjncp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gndqbkwil.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gjwppqkqc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gssjbxjbf.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gzwpoxpnv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gdiupxyzm.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/ghcwjmilj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gshpaacxr.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gumvefdlk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gzutwicii.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gicwspitp.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpebtaxpb.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gwpuuwqnd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gydgywoap.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/grewebjnc.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwkfsscru.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gkuqzydau.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/geedqyila.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gekvohfst.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gafrcdjwi.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gmvupxlar.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gstmnakap.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gctgygkrq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gexaopssr.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gztvrrlft.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gefntbihw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/ggvbjxsyp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gdipxyisk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gldgvuqpl.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/ggvucujyw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gjcppjqpd.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gucoiyvkz.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gvtlqwrap.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/goiopdeuz.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gvcvshqtp.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gakhvfcws.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gavfrsxye.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gceqcabay.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gdndyqvea.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gzqgbbxuz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gsjqdljvc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gsxpnfgti.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/glfhqzjte.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gaqhikziz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gcpmehotb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gyxlbcwpu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gdmgeyjjj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gmgsjqolp.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gsipqmqxh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gxykurjjs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gvlkfaply.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gdxoufvor.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gzjmrvfbu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gunuwexpz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gqocpspqa.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gggkdxmjm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gooyhvqdh.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/grolhewgs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gqteydcto.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gsqszzgan.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/grwgulkua.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gfnxvkdrw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gqszgyuse.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gpiangyle.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gsnbkryoy.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gxnqsmqzl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gzkvidjjz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/guagvojqn.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gpsqigwes.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gdzyaacyn.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/ghqnltwrz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gecrijobx.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gxwokeqyo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gbfxfjlkr.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gdwnjfpfp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gzdygjtkj.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/giezymrju.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gnsjhoxgz.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gzkuifqzn.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gizhlvyzd.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gbuqxylms.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gljsskbjo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gzvcvvzvu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gpjrrbzmx.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gfrqysgla.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/ghcqcpjci.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gmqeqqjzy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gvogvzuqk.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gmkbhrckj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gjgyqbwrm.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gzowxzvns.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gywwshfhh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ggxtpwjjl.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gzpmbwabf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gplrkbbve.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gqsvxeabp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gmupzivvp.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gwwkrwuhv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/griknqxmh.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gtfaovfor.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gfcqwfwoi.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/goqafnkdb.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/grwgubrkt.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gjripsace.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gpzwrwddk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gsporsrnb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/grfyvsxed.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/ghuirjsgl.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gkybgsqaz.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gvqxchkwe.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gvyfkhyjj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/ghtfvvuqd.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gjhemdgzo.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gaagduyfs.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/grvgahyvw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gsazswpcq.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/ggrkswzyw.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gyetxofsw.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gghuayuku.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gcloaapjl.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gsevccvcl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gfvlyyogb.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ggtykbsqs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkvzvigxg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gvzdwhuyt.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gmzkhfppw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gsllianqk.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gpvmsouad.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gaorwdzoa.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gpwqygowo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gnmhzbtsf.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gnhxmlwwy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gcpmhfuko.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gltrxmfyy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/geuvfzohw.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/geyvxbloc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/guwnslhft.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gfkydivnq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/geftiumzn.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gympqgpjf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjmlompxo.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gvjrxipgh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gglwxwwcw.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gfwlfjjwq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gbfbdmtee.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gwpuurrde.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gtkruvoos.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/glgncqvey.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/glvksmhsn.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gtlrdojaa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gsxfnjkfa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gspwyjgsd.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gqnuprlmk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/geiprkrqe.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gxnajhnzh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gefujxhyh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghidltwyx.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gaahpfgfx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghpdzemhp.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gldrrcysl.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gnghzozho.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gvdlfxvqe.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gkmrhgpgy.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gknqbxruh.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gidvrqydi.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gtsefkthi.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/ghjlkmwso.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gnuvqcajg.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gsjtemxin.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gcmxgkvoi.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/goklbqibo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gsudbxbgp.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/grmuqakjl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gurkwksmi.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gbhdfpkmy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gfidfhedy.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/ghmkdwwmd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gjivlnwfr.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gloxgjxjk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gpxcmxnpk.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gotklwzoh.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gthxpuamt.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gglgrykgs.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/grxneopgf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gvbatikhd.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gcdlblpyp.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gadaqkrve.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdnvsnqta.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gynocbziz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/galwvbehd.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gwntzylja.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gbhimhiil.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/goyhvndpa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/giitdaiso.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gfrgvownk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gtyymhpvj.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gabbqgodz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gnodspiuw.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/giohspndd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gcdfqwsyr.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gbaunpwvk.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gwaqfwzve.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gczcipwxf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gigqeqees.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/getrsprzd.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gdodsznxt.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gdwnlzzbb.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gbdctmjec.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gavkzctjk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gysirixlw.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gtsfukxvn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gxhwjxpmk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gxylwljjc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gmdrvfjms.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gkxkonrmx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gjperxgyz.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gknisibcd.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gelghdcyz.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/guiybhyeu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gacmfwhlh.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gzkrhzelr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gaydyvsvs.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gvlrtaztf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gmybianan.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gmbrkjmty.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/garwrnuxr.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/ghwssaoof.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gvczadual.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gjmdbzvtr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gsmcxmlqp.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gvmysjhwi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gjsrxvssy.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gzfzkvxqb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/ginphqjzt.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/ghjietiwq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/grnsgthha.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gzujmtkeq.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gtjeznhyt.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/glhupoaya.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/ghmhovktm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/grxjitknu.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/grpmhbmsa.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gqdnutzdi.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gdnzyeqjz.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gexkoeipu.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gmbqsnqgg.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/goxatzvhg.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gfgzljlhb.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gzmsvzdjp.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gsndhcjza.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gmypibxtj.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/ghgavczky.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/griwjyhee.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gzxmcypst.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gitapceki.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gjfsqeyrz.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/goymmkggg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gtseyaotv.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gpyehlcjn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkozechbq.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gqtkaswjy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gebbdjgqi.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gtybkptuk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/goudqbrqg.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/ghaqwzxlq.sHtML


<!-- 参考信息 -->