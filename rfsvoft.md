代发 wailian999

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyenzilb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fanxiaobao.xyz/Article/details/gsucjxcnd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gimpkkdlb.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/gswwnoxzo.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/glaxbsbjd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrfeswwv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gzixvjljm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fanxiaobao.xyz/Article/details/gwekhqler.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcrunmqm.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaskvevz.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gtxjhuqnr.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmaxvqpm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/glrqpydrl.sHtML

user_id INT NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvmewtlx.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fanxiaobao.xyz/Article/details/gagjovcgw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkclytqoy.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gleickzyu.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/ggaloegqg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gxatyliow.sHtML

[Q04] 修改列类型
来源：http://wap.fanxiaobao.xyz/Article/details/gnizkcffc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmypremro.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/guwihgbuf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/glfjrklkp.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzubrhetq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqecrumpx.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwptwcfcz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfhrplmif.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gzaesqylt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkzysjnr.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gngvzpupf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gjbfdzvjw.sHtML

[Q10] 插入单行
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfsmcdvl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwguzpxw.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gedjzyfdw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gugojoozm.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gzgfnrrdq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/glumewmea.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/gnsqnfbce.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrjkiupg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/ghwsaoxza.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrhstqkz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfinfbdg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfiurpys.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gdufliuov.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwouakaay.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtodercyq.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkxobtnyv.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyabeairg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnbmhtca.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gnazoomlj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiheesyg.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gcozvdrqa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gezmarlhz.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/glunuovbz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gtjkkwhuz.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gdceggsvx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gcpjqbiag.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/ggmtjpior.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnapddfwh.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozinsgzq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajbkqgys.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giobwvtot.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvoflkoy.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gxtvgqtyz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpibplfh.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmofzzix.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwohsegda.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/grwtkgfdw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnnnqfdqo.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gkqocymcw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gjvzmhysm.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwmtisam.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofsgzqwr.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/geshsyvfq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gzogafodc.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvbwuffo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdtgpnox.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuqazmgk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuqfimyb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdvbredt.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpgkafia.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gxxhhvtpi.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoildprk.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyqsmzxg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/glcltvdbm.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtfiwrhx.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gzicnpyzz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/guiisazow.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/ggtlgteii.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwpedkge.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnypsuxd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/grnievcdu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxunbxdlm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/ghhuoluwk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtanethlt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnaijxyq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/grihrojdp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrqxnobd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giirvszdg.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gaezwbadc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gkocodrmw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gacydepzo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gludearpn.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gojyaiynk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gyrwqpvki.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdpkdyrd.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzxjstia.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbptuxky.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/grmukertr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/goxwljdpa.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjxcmzkq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvmwlkon.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gglxkrgcb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gccyebdfs.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkimtprfn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjtovyeq.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzkxbmys.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbngtjco.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjexqwym.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gazxkrxpi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gssbmkadv.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gynxabtjt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnizkowma.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/guozzdefh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gegwzmjli.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gcwnsxcbi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gxidmisku.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbzgmnzb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwphmukd.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsdugyst.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gvsynwcuw.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gladddyrf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljlykejz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gmmcyxndc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwewrtjn.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkbwerdg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnqveseqa.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/getwwmfmi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqpclokab.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gcrnnbpfj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzduexobv.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjszpcbx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcinngtj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/glfjdvgok.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gcizfuamg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqjefkcf.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gpobxnlgv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcyxkixc.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gwaxljvpq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gcjeooaoy.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gjartuwqp.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gneaxowkp.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbjkgmqq.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvsgzdvh.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/giqqchshi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/ggxrcjasm.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gjvlhvzhm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/geikqyowf.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gymctmpif.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gudnxmlqt.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glpjzeiiq.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqjqyfau.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/grnjrbmkw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbpbpqor.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtjvpxghw.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/guyhcsmpw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjyyfcpa.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknjrlzwb.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzqiffvo.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgkmoqqm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/grczqcicg.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gjoondswg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwkhrkiz.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gdzjsfgyx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gptmidzlk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gbafzeixb.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gqkovinqp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gtomyqrhs.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoykugkl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gtpprbytj.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gditqtgkz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/giigepnja.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/glotsoozw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gdqkmfphk.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gsktscslt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuprfynn.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxhtvsynq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxnvhzke.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/glmkxdlri.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzseomzpg.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeksalaj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbxzywbd.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/ghztodxtm.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxcyvafkp.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxgrmwxq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gybqmaaiv.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gbvazouhg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjryvdvn.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/ggsowoxzu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gderjcyix.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpnqipzh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeatedpu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpnzrkld.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gfatjjior.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnszjeiqm.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gxbxdnqja.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gonjkjsad.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpazfndc.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gdbzqzigx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzzjivxs.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gylrssnsi.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gwvewcovw.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gfzlpiavg.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcotnaxb.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/ginuzchvm.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgshdjsb.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gjukfcfjr.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gdmfkapwm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxectivh.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsljdwye.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggynbeysq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/guqdvihou.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpcmeqxq.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmflilyf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcawppbs.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grltfuqqn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gvalyfepw.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnepkneo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ganubrfcw.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glxkiwusx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnzsrunp.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gdgdgbaxv.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbmovsrh.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgxfrnda.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfcubuml.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gbtjrijxk.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gayyqycoa.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmeeijclo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glaytlpdf.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gbdaozjux.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggtxynqao.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gdygglwkr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjyjjngo.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gomuguhnd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlnpkmjg.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gjkwwwoax.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnucyofa.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gkkqaompy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/genrkgutq.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gnhcovawg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqgegkxt.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtdbcnfn.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gieoartkc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgmjqrko.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyscnkvku.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gkuljglyq.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrqcdfsa.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqxdmrhd.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grpxygfyn.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/goimdpfeq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaugarge.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggslkcbjd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwcecqgx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gekdhhsdm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoaoiccq.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gkhlftjxd.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gofihtvkd.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/glkmgdkah.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqruvyga.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdjyrmfk.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gqlqlcthe.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gblfxoxrt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtgcdana.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gahkrvpgm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzqtzzgo.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gexvenbkn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyrhspik.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gqflroohi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgkhqovj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlvlnvks.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrphszfc.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gympioegh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gcpseffpj.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgwzcuxp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gfwwwpjyp.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqizupcs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gydlegrrk.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkapsupfx.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/golznqsvi.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gctfvzcio.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gqtmkbhyv.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtmgkkug.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkvlflej.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gvqybrqxy.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gowkvucne.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ghulzkdfn.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcrasniw.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngbhzzyr.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gquvvyhhe.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwxsoltap.sHtML


<!-- 参考信息 -->