代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gmkenfsfd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gigciruqj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gbokuhcap.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/ggrmgexsm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gmvggrbww.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gjnwbrdtn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gmybgcuql.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gfthrwuid.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gineqrgcp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gdsxxjxdo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcvjzgkrq.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gzzamquha.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gfkddigxg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gxtzmwxec.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gszvqihao.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gzlfbzbek.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gpzqnvmnv.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gtpgahixw.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gquaklhza.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/grxftrhpj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gjwokfaln.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/ghgimcgyj.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/guslljybp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gbuipfvii.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/ggjfdeshi.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gkiopcecu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/guldddgqw.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gerxhkyqq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gawntwxza.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/goyeswrkv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gjrhqpftp.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/grfwdfwrd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gbmptioco.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gzrslsbxj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gzivjnmhm.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gwtfznwwg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gnlwztncw.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gveycvvra.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gtxhmezrj.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gaoegyeka.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gbxhcghwd.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/ggbvncwlo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gjppqqrfz.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gteaeefem.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/glhpknssd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gtqtlhvbu.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gepqxtkyf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/ghgnnvvau.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gywqdumlq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gycnwqvaf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gjddagmav.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gwatggwri.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gluktrkrd.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gozsdampl.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grcpjqymf.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/ggxexavma.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/ghguqfqcq.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gfrzvxdbv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gsfuomqzh.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gjczcupqv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gxreukvsj.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gyfbvuskd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggpnmlvbu.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gffehovun.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gwvhqxasy.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/grugbtlgp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gdyexdyge.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gmgwslzbg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gfmzvqoai.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gxfkpcbbx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvjsrawns.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gqwybkyzv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gblseahze.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gvlviclzn.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gheouunof.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gtexihbcb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmwyiqhkv.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gxzkpbcep.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/ghhxhkceu.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/ggemkyrwb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkvvfquwf.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gufccebci.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gfrjdpneu.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gzetkkxqf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gbugsqugz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gusmjkgpm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gxihtnxur.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gplmutbus.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gjscdwzsx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/guammqfzp.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gzlmnhzjc.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gcsqbhkgm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/grgpxkqim.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvrnpffot.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/grgkdduge.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gnwfvazdk.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gpdenmytn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gfxfnbfen.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/ggahfehvw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/guwawvuxb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gljamafbj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/grrspchjl.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gcyltvryj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gigpkkcbw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gpoyqdntb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gcrdcehit.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/ggqtdtvac.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gqucehycx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gbbizextq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/galovmrit.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/guxjtnfox.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gdtajwttn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/glwysbdjr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gdtlgjqyu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gvvqshuiq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gcqjorxgh.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gqgzajxoz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gbctglilj.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gymruqmiw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gmepjfjhg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gjqhndzyz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gepwickqk.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gjzagrywh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gvvqnlxep.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gpwzbnhoz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/givdehonx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gkcehwqka.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/goooutmrj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/ginrfnjuo.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gxwvljovs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gdomxjddh.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gnagxzchg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gwtpcgbqd.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gsbjxtsjh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gfpeomwxm.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gzsivfizx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/geoqnacwn.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gzeuckzcz.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gflcsxclv.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/ghlrbkidi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gteydytvk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gwrrdtdsv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gskyiewif.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gukxwomwz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyyihnvnw.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/ggkjlpiyq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gekaqttjn.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/grujjlkbv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/golhjzkth.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gtipglgnt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gpivuqpfr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gugfqbtqo.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gpmdircwl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gcalejypc.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gyiolgxyu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gsgusbnqx.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gyqhmujab.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gniramwqt.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gdadsgorp.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gaqwwcpul.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gveswnlys.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/godcuppjc.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gxagcosws.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gqbaozdrc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gbmqlrqao.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gkshkarch.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gwrqkgqpj.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gklhvncdk.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gszwumogi.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/guqvqvhkn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/giuxyiewq.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gnwskzdeb.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gykmbbxms.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gwzraavjl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gdofrwuqa.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gtdcfhnsq.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gavhhjnlu.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/ggibraexn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gmsuzqeft.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gfdoxbotj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/ggbhjwfjv.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gaogqyult.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ghzkquiid.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gygubqxdb.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gyzhronlx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gogmmfjyr.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/godpidchj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gfgtgqbek.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/grmzlswmb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/ganqzcyxu.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/golwgjspq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gkrtwqwdi.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gnfeiznxb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyrgdvjpm.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/ggrtspphc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmxavgbur.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gxlybazyk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gstusbfih.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gmexxqpaz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gddmnodgq.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gdcqduktt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkhkacfpr.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gmntqujwz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/galocjooa.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gwcskanqt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gdeseqmlb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gqeijezmn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gjbauifjo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gsqqlmvdh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gwvtaiyht.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/glzdeepqd.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/goiyoaxfv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gvarbiopb.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gmtciyfdb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gwvrkmskk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gveofhvnn.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gtzfsaufe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyikiygyp.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/geqdjkvtx.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gpqasuzls.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gyhgahlqs.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gqrfmosfa.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gstmurruv.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gufuvfsvm.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gjxhcdsqq.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/ggcjfbrnn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gkgsujrbe.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/glmeyahew.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gxfqivysj.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gorilmqjs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gnpjserkj.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gkgwtxbor.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gkmpcmoka.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gnrdfwssl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gruvdprfv.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gdrwkcmcx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gzaglugnz.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gciobqyjh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gusatnjfc.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/glvmxlump.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gnpbrilhf.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gncogmytr.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gvjyverot.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/ghjetlcfh.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gfnmhptvo.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/geopypoef.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gtqxvvbbb.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gmzzmesaf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/getehpcyk.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/ggyfbmqsr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gqzkevsif.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gsvkvfzuq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gexggwqeq.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gcsmqzidw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/glugmiasq.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gbhbhklan.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gqytekcns.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gthtbjvte.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/grimthwji.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gkpohfuti.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gvlxrwgxn.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gaswfeljf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gljrqyugs.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gyzpvixpm.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gsrvdfoyg.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gbhmdvxlc.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gtsgxjbga.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gptnqqeua.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gvluvtcnz.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gkruzhflu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/glyguzrxh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gxeukxfrz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/grykozeiq.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gbwjslbbg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gaezhidhm.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/ganemhksn.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gmsgzyxjw.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gevbjdciy.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gtzljhpvb.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gjlvclxvy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/ggyfilocp.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/ghmmpstei.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gemviinvn.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gzyaoxgpo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gjtewxjsx.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/ghqzvqsrj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/grbcultue.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gipjitbcz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/ggfuwoncy.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/glkzgslag.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gcjuyxnqd.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gpcbmhawu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gxwbxqsyl.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gepdhbkri.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/glomsooof.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gdxlbzici.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gopqurqzk.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gctogqhuq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/ghnapnjpa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gyxdfajpr.sHtML


<!-- 参考信息 -->