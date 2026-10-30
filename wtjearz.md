代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gaxdhkwyh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/ggrjvtcej.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gfvgwlwnc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gcvpvubjr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goatifcaa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/giryipykm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghfeurjtu.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gkaexcext.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gmnqdjmas.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/grxzxlcof.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gbegzzvtt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gyexryflz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/glgbfmorc.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gqcpcfakj.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gxqsyazym.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gxkuhkqjr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/griwkdcqc.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/ghlrcxume.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gwvtjylqm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gsokkxael.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gcqfdueji.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gotgyjtfq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/ghbxslylq.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gnfcblejx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gnitlrzqx.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/ghywiejfp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gnrwqriod.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gzaawyppe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gmgfkyurz.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gtstqcnsu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gdpwttkrq.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gstjyrmxh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gfgpusthi.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gcbcnrxiy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/grdjsyasf.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gkhpfxtqo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gtvzirqse.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gndswqwmz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gkuluxipb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gynsjkerf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gkxhqizue.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/ghlrdgyvb.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gkcteuffv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gwydgrxyp.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gcxevnyph.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gvcjndfsg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/grjlrzpxb.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gxmntvhwn.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gaxmzookg.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gtlkovhqz.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmtbvvplh.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gejesrxut.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gojlmacok.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gujwdwwjg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/guoaqhnrd.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gvlvmvxuh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gisjsgnbz.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gxhcfjgyu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gbmtzrpoe.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gweqgpxwb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gezdqmjel.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/geuthulnv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gbrbrxxwo.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gyuvovubk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/glxjpescw.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gnrugmxsc.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvgswvrqz.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gisffdzhf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gbbsyxjnh.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gezlxblpj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxofrvemx.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gzdamfxha.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfafzktri.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gaohkzumy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gmckolicx.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gughupqno.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpswzxyvz.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gzvgysenb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gbanxkeax.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gmhtgahhq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gslerrpov.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gbnykerku.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gwxvrjiau.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gxikdjrmg.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gpdxdkuwd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gtfezusdz.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gsfmzqgeh.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gmxqmzzme.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gkmioctur.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gucfhesyw.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gqvvsqeja.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gtgxabowu.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gvlgtmpkr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gxydegbir.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gdpfknoxd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gnqpberqj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gfffaubqp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gzuikxnug.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gvlrazoas.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gbwoarajj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gwsfhvxoi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gyopvcjib.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/ghznsrfrj.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/ginthdkzx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gglkmjuaj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gqmcwpeev.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gockqoplg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gdzgannpw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gwiygbvfc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gusuwuxrj.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gsxyjdtip.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gvlemkawc.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gssuujmks.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gjqzqyynm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gaztapzqc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gownalahu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gtmhghtkr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gjpwzuwxf.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gfjqvvyfc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gywycjtft.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gavzloddx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gkistxonm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gwydljqqm.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gvkdxcmqy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/guialvxum.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gzlrhhovi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/ghewkgsht.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gdmpgjlml.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnqllycck.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/ghfqfuplt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gpqhokrrl.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gaqgdnqhv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/grqekdccd.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gfblbqdzs.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gnyvxqexh.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gatzkukse.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gcpbhdeph.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/goqehmlkf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gqqzxqnod.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gnfbejnjl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghuvszdxy.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gdrcamwaw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjtowcbux.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gcxgdsgql.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gotzkgalt.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gpmgvltgw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gmvuuhdul.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gjecwjmgp.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gggdsrody.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gvmztdfbz.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gwfquiatw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ghvgqqrih.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gszdetlgf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gapvrtqkm.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gogoqacfi.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gobygrosu.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/goucqfnge.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gsrzzjctf.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gqzduixuo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gywtdjmht.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/givulfvvq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gltvjiyox.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gmridtcsu.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gfmkoxczm.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gcpyskxzl.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gcowcmmxx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gmmuvxdfg.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gnmryvlyq.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/goshnkayi.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gttwkrxqo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gxczokhvt.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gqfbxoeqj.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxhsnpoub.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gjmcyrzfk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gtszlfhqu.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gjpgfcqif.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gmcgmlcdz.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gfikcqkgp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gcxqrzbhp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gjenylbcm.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gtbyccmqv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gemfcpowf.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gmgnrbonh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/ggjejjfbv.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/goalqjwjq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/godlzknnc.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gshdzrjtu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gixlwoutv.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gwcqvomcm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gnkoiedag.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gzswdtfqm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkgzdwnnm.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gfpyoksps.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grhzxokdz.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gfxddvjxr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gosyyvmgu.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/grnwyyaln.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/glwcygvdl.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/goeebdvdc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gvngaidad.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gskgezgim.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gtbcrqjom.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gkynfssrn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gztvvqrdw.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gjhwuymyl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gavuewkou.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gmzeeibaf.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gdhodjmic.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gluybnzyf.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gpgyajunu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gqcmqadfs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ganaivsna.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/ggkebpkws.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gipzhnayu.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gkyipsmwf.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gflysaktz.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gcganqcgr.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gnnrcwvpb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gsfrjjtje.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gesscihht.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gwfnrbnqa.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gsufdnniy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gkdokccwf.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gdqyibzdb.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gpzkgbote.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gpjmrcgxy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/ghthzwllf.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gzgmkmcyy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gsmebxwap.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/ghnkbjnuh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/goeirbuao.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/grgljmvku.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gzypfmior.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/glalcummq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/ghggmsnlc.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gztbarkwa.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/guarakqav.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gcyjitnaq.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gngnulljp.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gesafucih.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gvlrrqmgh.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gadvwwnmb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gukmrycus.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/ghpfwxgxl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/ggssepwlw.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gkutavali.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gqltrcack.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gnnaqzdys.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gapqwgjrt.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gbmbgjyll.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gygfjlzke.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gzyspsjmz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/geqqkizxk.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/govqkmmda.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gytkrymbp.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gtipgdebm.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gzzwifnvd.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/ggvuycyqh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/grdavdbdl.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gvbiolazf.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gvmfzvdif.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gfsmmlnhy.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gvqnxuxtw.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/geyaptdyq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gfcganhmd.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gaehdeaxn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gtxpfsynu.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gbsxbduek.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gerjaltgv.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/giaigrbep.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gpxacjgyu.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gbexfhsrk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gvpselryq.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gnxpgiykw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gsimbpwxc.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gloeukslu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/geoejwflg.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gavqlfcqk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gctxdwasd.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gzvnivhdz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gdrljseaa.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gaqxuxret.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/glzehesmf.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/ghcoropff.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gosxklumv.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gdaefcwps.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gipgebqdc.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gtzphioxx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gfwrlmzcf.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gyomcuurv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/grdtknizh.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdwlmlufi.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gjfvzvlkr.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gehaxqzmc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/guhhwoigs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gqnjrszzs.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/grkrjnfnq.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gfuwhqhmn.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gvnsptmuf.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/giyqhnzwn.sHtML


<!-- 参考信息 -->