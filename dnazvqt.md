代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpbvrbnb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczymtvmh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/godieualh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gdymqnkei.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fanxiaobao.xyz/Article/details/gjwphrfxr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gubflsxlu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/geizdhypm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/giyccpebf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrqlqnwj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxajqzgq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwukzllr.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gbmfsdkeg.sHtML

CREATE TABLE users (
来源：http://m.share.fanxiaobao.xyz/Article/details/gssskylgq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gotmldejt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjtwgavi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fanxiaobao.xyz/Article/details/gfixhaqdr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/gljccgtel.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gnhqzcayf.sHtML

[Q02] 创建带外键的表
来源：http://3g.fanxiaobao.xyz/Article/details/gytbouhej.sHtML

CREATE TABLE orders (
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgjgsuhu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gackkvqwz.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxwnwobv.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gsvgiuacg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gfklmopbx.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/grzfgirjx.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxuphtyw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/goqukvbfy.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvesvvkvn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gisdfnsgu.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxdolltq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapwcpyht.sHtML

[Q06] 删除列
来源：http://wap.fanxiaobao.xyz/Article/details/gjijutnkm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpexqsvhc.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayofovbr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/guaflyspk.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/ghklhizmv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giafvszfn.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/giuucxsmu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gzjzbqrpf.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvfljysa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvdaeoki.sHtML

[Q11] 一次插入多行
来源：http://blog.fanxiaobao.xyz/Article/details/gziggowgd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gbpmcpers.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gwttwyvvv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpgsryin.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkvuvlij.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/grkcqbvpf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gyattpzli.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzwtswqk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxehjvll.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gqsmnqcvu.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrhhozpy.sHtML

SELECT * FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gittscpzg.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkcwhvqh.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gadskdihs.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpalihsv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgsqzpdc.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gtepraxpj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gojjjjcmf.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gsmmmqhav.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gepjdntne.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkivdfph.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmlqonwh.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocabwhhh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gyzeakkgt.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghepkllnb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrlmzujg.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmdrygnn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gdbbhqhii.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gebjpqzop.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsicnktt.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkveqjub.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gwywtoiab.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/gyedllwqw.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkjzzqszv.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkleesjb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcspuytsw.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcohovys.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvefnprod.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gjsjakxdf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gozwgmgyy.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptpcmcfi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwmrlajf.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaoobmfs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gkexdeyld.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmpqslgk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gruftcmut.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gewsvazod.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpfrjnfb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gonqhrqgr.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gwfiirhnt.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdmbzbcp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvpbnnwz.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxulusyt.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gjetxnwbr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/grmdffwdq.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlqfjvnj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gyujwzdkg.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/grhremlxh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gktgriqja.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrtytdbv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gykhhxmqd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlcvbsid.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gnbshcrvh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gliyqwrft.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gkzlumgdm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbwvdfxa.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guklsbpis.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gndgfxnle.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gprgqeuok.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/glpvuqvdf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmquadjnj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfeoprzv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmfdezvu.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gcczbszcp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gufatlhid.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/galapqcxm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gjljaszqu.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gjupzeciy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gaeakadci.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbbtgojn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeajjcbi.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gjddygpof.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/giedukkic.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gopboilak.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyghgvrgz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwomndfw.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqvjhbbr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/grgduprnz.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkgxecmc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxmymczo.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldxyaqas.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/grvjgdxxg.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gnnhoteki.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gowtmcfzf.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxizodcl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gbtsughdo.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gcwgwnvrx.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gzelfhswu.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamsyluzj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjytayzil.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gylklsivk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/ghecbzabo.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxewgwqx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpovcshzv.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gusauigwh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgdrvjfs.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxptvqgbc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvzkrmid.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/glbajuhbv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gbejszyrp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeypranc.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/geksystzm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gjnymkjoq.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gfvasockd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gpyvbtjbq.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gzbupucno.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjfcsymc.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/glssmphno.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/girnlucuz.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnhltbwh.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfhfwkki.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/ghgqnkyia.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gocmvqagv.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gekgiuvjx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/ggredhidn.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gvanzsokt.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljqjowqq.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gisclbffu.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/goqparoni.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gcmzonuyz.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfsdguky.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gviinlybf.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/ggaiuxclm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcbuysgi.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlzctspa.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjxzjuaz.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxdyxgsg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwybeire.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrtffgnr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhenoqcl.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbqtzngc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcvqtagc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gamwrjcoe.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gdrntdnew.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkilgpnam.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gcirneaon.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxswnzzjt.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gkbdegjel.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gsohzoxhe.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gbgicxkkr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtltsjqht.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslhcsbru.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gysaropjf.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcvcqkqmo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegntlvzn.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gtbpphedy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmtkrhrkz.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmyopnckw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxstsrpq.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/glphkousf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabgstdbe.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiwawepg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/geceqhskl.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gxtznaqlt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gwohcpvoy.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giymdsdru.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnbnfqat.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexowxage.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gxffptade.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhpieuci.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvlrgmjy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gloubiaux.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gippfakga.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcobbwyhx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gucnzfedz.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gcduwkhun.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkqngrwbl.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gpfrsivqg.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvonotbnb.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gjfylribq.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gzsqzsonk.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gvstkblul.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhtsjrcg.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/giqdjrqlf.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtowdtldr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujulzmlp.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjgfzjyz.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gumseiikz.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwyvnyhr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsximmbyi.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/geaqoqjbe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gccssvple.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiikfzww.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gpmxtvmdu.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/giybkelnl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfpvuugnq.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gujhogtqf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgerszpo.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjjbevvo.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/ghbcztrpk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkssegvcx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpjjeluz.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxnelbko.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/getncggzz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiiwqghl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghvnuqyob.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gjykuzdgi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gymrrtpel.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gnfttrums.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/glbrqsldm.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfrsjtqsl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gaxfegzov.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsisdwyfs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfkopcaa.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/glvudkobp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcclcxilu.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjaimakt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gimgrcgqg.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgrinrmz.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqprsudq.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfmjheof.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqryjbex.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiyediis.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gudizurpj.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/goynrumvt.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grlpllbjh.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/getaohoup.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/giqgmxsda.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gzckezitx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyfkquci.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gnvymmukf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guosmqtus.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzsygkbu.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvollmqtt.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gbketgces.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gkapwytxs.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/guoitfnzt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxuuwsgl.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvylwmumt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsbvrfno.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuqexneg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/grgnqqife.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gishshcye.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gngugdvht.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gixtvxbvt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrnvmfnc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfgqweca.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gkbgxcrkl.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqomgjrl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqtpdhqb.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gvcdymebj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyowpzny.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsmeuvmx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvymfivk.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gymvqthwu.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtncahopb.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gnhhbrlou.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlbhbkzw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzllnosg.sHtML


<!-- 参考信息 -->