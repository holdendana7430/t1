代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gicmxhtbn.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gdojprvnr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gogmbhtju.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gqeqxkrvp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gvfzaapoh.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gvvhneghd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gbnosckmv.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gqkqrlinw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/goxibumqj.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gahnhqalj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/guufbymta.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gobkfvpdt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gibxbvpbn.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gubncwhdr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gqylhfjwa.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gtxziwcjo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gvvfwnpjs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/glawfnhet.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gdsovwgtu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gqbohaekf.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gzyhokoqj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gxsklcvcn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gfzfrnywf.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gcqkuzcll.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gxuujikdm.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gzptwbfjq.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grvigdtlx.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gqlfprgzv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gjapcdgyl.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gzkuerfhc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gcdtwxmnx.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gwfybxmkn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gmiodzekl.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gnfyentff.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gudmbzwck.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gsjhxmirn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gdvflsjnd.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gqptvhqya.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/ggvhwezot.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gmiphpmpx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gbgmqoygn.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gdnsiocqe.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjdzqfofy.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gzvynlmkw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gzixbmeda.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gxfethaib.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gywhzfhrm.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gqaxfpvoy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmkgxdhuq.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gmeomurgb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gyliirjcs.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gsrmngebk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvpksdaru.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/ghwmxgdki.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/goelbgajz.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gkxkmodrm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gzcbgyvgu.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gsecwooiu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gxyhlldla.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gnihfopps.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gdmnzipjm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gokryzrup.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gupaoywpl.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gcyysgbkp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gqozvqhnp.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gspbpyvrv.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gcgllfzon.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gvaqiciwy.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gcjjpnyqd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gnpvlanwe.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gkzrufdcm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gcjfislud.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gdtmupeyu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gqbecnzsu.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gtizyhecp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gipvcmnym.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gmwyklhhz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gmahelhpm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gbdholiqb.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gttzdcmlr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gygzbxgkq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/ggdxkcwpu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gebceonnw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gdkeredpx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/geehiknfd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gdbofiyuu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gllcbnwnn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gmrvcqauc.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gccotgdsd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gwahrelhy.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gtvxwuzym.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gbdcjrqlr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gozatdodp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gqcrepfto.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gkhegjtrm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gxqoxoskw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gxocbqxuh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gypoljiwp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gbwfraveb.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/guhciacxh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gsatzmisu.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gpvjavrsn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gkhvvjogd.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gvwgmraqh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gbsgisarn.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gecnmlujs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gzhqjuxnv.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gwsyjlujo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gxlxmmevm.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gmebxmejr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gebnzqutk.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gtfncfxip.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gvukbgyyt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gxmoziuyy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gywfsqoqt.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gewiqhgrn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqccpzfxr.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/guwocdfra.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gqhzrgisd.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gnapdpqae.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gtfnjovph.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gohgdtvvw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gnchhjpul.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ghrpqzgmy.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gwlcxfeoc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gvjkdmrig.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gdjwitcql.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gvnynrnve.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gibuxfcpi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gzqpmrcbe.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gvgqksbli.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gyzbdexeg.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/glpstacnf.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gtxfdufwh.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjeghqnsq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gqlakzntp.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gxiaymrds.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gdplicfkp.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gqnrimsbe.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gxlbmjyak.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/ghqyttjqb.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gnscnusih.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/girsoydot.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gozeptwjy.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gnuwdcvks.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gforzmpza.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gewvpauma.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/geeatxknd.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyhbggbbx.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gxbhenkxo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/grdmqbwxr.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gjtfbmrfa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gwiahsmlw.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gxdvzfnpz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxvqblwyu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gintcvjxl.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gtocnimkh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gndrtyjtb.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gqhqgernp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gzilrzdvf.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gaaovzbrk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gzxwfsarf.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gfxlxxush.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gupmvwhsn.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/ganeocvhb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/grsoycfmk.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gdobngxtz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/ghnncgkxu.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gfcssqvtd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdyvmmykf.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gthhbizlc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gphgibipp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gtjhnwwlr.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gtgtvivpm.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gavqogfae.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gkrdtdokb.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/giyzpbyyn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/ggdmocyyz.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gameeempn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gbonwhcgh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gdcgqnzih.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gampwzoiy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gllnvgsks.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gsxzipasm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/ghtkuiose.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gokbmtuov.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gttzlyeua.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjfwbocce.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gwqpxqsml.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzbubcwka.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gxdfswbiv.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gjmkbszbw.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gkdxrzrul.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gtzpqhofe.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gcduimmon.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gbnioewnn.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gkfaxcjja.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/grhavswvv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gimxulywj.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/ghlsohqqs.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gpcrlmppt.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gbdqenstl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gamruxkcr.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gawfuppom.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gyaeapeft.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gfwrgwjau.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/ggusbxcbp.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/geunxvfkh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/glwmhvyel.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gjxnjnqod.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gxzbvyvuv.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gsuakexkg.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gaxjmaowk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gkhfdgwzr.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gpqnnlgvn.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gtvkutksj.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gltexrvjz.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gldiyqqfp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/grhnoehwh.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gwqtmreqe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/ghupbjibk.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gwqhhdckj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gfoutglup.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/ghylebdei.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gszetblfc.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/garfitrxo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gktmggmhn.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gzpsgneiz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gxpglipce.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gygnzsveh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gaexbbmke.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gtxepgdxa.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gerdfayzx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gltzwapik.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/glwrmxfle.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/ghnrwalyr.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/grmrlndaj.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gdqudjddd.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gorfvbyca.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/ggirerfhk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gabyqgepp.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gekrmrjpe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gjfiqfbti.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/ghubavxae.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/giqeggwvy.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gnxaegohh.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gnhbyompi.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gscvyenhb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gmmutpopx.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gicjrofxw.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/guvmbykxc.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gycaakznm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gbfvdegok.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/ggwudolhq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gnawsrrpw.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/ggcfdsqbs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/giozythrf.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gilewzyae.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gnvyjdcue.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gksqpwlku.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gczawsbww.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/ggpsllzay.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gwztqjgdw.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gjrjsvkla.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gsiqocjwo.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gxjebwbvf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/glxfyhhwt.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/ghrhrnsne.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gjzzpnwqu.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/ghwkviqmc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gedceckdz.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gaqtdptpg.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gbpqjybyk.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gmteuajcy.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gktmvriaz.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gsathutyf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/glyvtjsre.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gsirtidbb.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gbumjvbbc.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/ghgqlzkep.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/goeupkwqs.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gwvbtiirc.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gfwxdgqdw.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/geunrmulw.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gsshkcxex.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gybbiviij.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gjwvqbopp.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gsspqoaqq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gtfgdbnlh.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gvpulrshj.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/guclmiafl.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gijarwajp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gvmvzxexa.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gtdklgief.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gmqnyrgaa.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gbmxvsnla.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gilsuhpea.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gnacjsgci.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gegyisvbn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gfaihhxqf.sHtML


<!-- 参考信息 -->