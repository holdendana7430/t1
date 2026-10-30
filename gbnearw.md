代发 wailian999

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/glsejtzij.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gnyczpdsf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkdlcpdi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/ghmiinhwf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdmcekey.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gujwlwomv.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gamxbnoyy.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrlmzsqo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfdfpwfq.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/guigvmybp.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/gngqcgbow.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzonmrkkd.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/gseerfmjv.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/gfnzzqxdo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwalecvv.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gohdvgmsj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/grszqpjft.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgwicrec.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gttucoecq.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjujddumx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gjykgzvze.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasbhrqpo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzeyywgp.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/ggmojlujj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gawjwhlce.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gwknwtcdc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gixsqbzev.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxwbiwsz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gsplkzaaf.sHtML

[Q11] 一次插入多行
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjogmpkh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gshcjkzpf.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/ggruddjxt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuhtdpej.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gpacrtyrt.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gsugmojhj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gozvhtetk.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/gttussupn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gftysztfg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gtoihypcq.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gdewudfty.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwibcnhtw.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrbzmqlj.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gheukylmj.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gehnqtmsg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/goeqnerzz.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysiagftw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gxcoxbygm.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gmojocbbf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gqcwihnnk.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gzicyyore.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbslzawjt.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gqbdjpzcv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyfwfhln.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdvwpmcnc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/grbgbxqgl.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gylhwjvvo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaslbrsq.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gditbuwgy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpvofqva.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/giegwucxx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuoucxtp.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gcelhpoyq.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gizqmutcp.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkdwkgil.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzrxjfadk.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaymgxkf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gzymcqvzg.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjojtwjs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gioikpcgm.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gyzbqrmur.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmylpaubp.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gnickxbtb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gvavuntjt.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhsloztw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoqbrqyj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/glkksugyi.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaywldna.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guosfcsap.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gwhacebyt.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvvfvhtl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/giggqiywi.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjbgifkd.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/glaztpsvq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpniieda.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsthjriy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gomjvcxza.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacmvdiig.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnkycsnf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsgfegkb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzumroiy.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjurbsvb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gecidcmue.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzsvjnjn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gfoyurmsw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbqvrsaq.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/grquexiuw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gdjpgewzl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzyybupy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjfbbjhh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeihzbqg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gwzbdqnhg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gvjupcqtp.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gazovxero.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gdukvjrhm.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfxdbqdw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkucoyfva.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gghreyyij.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gfqtmvscy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gjpalqeow.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gfjxfyfgd.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjgsmvfw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gerdsxisc.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ggxgcshdi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfflgvrh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkelzfzx.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqmrtded.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoiwvhzm.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gsbwnsbee.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasvqtzec.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gebatfvll.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmisklrgm.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gvtoyqvau.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdtzacloo.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhsmazje.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gsayhkduw.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/ggjtjghax.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gesozyhzl.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gincdmmip.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrdlxhhv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gxvrghvbb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/grvxozbtg.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/grfnglsgc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gerlhncwi.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmslbowl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ginxlmlwh.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxryfwlu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvgweuiu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gadzerxsd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gtrcfaicz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gnzoufzdv.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsjwpwex.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gtsspcrad.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gipbfiscm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gduuqnnlk.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjgqgxjj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/glhwhtpys.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gsziuxjbi.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gggtflijt.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklqytuci.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gozopmjjn.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoscsqvy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwhgaxei.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxvvcuud.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gihysilem.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmxqcgbl.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gbhghmhhc.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsrbsduj.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/glgcfcupv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvilstvi.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdfpeijt.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkoqwfbx.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwdpiiae.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvhorcho.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/grywvsysi.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gegcixiww.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiugirta.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/grotfzdgk.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcypmvjxx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/goadbpked.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzceygkaj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzkwkjdc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gfaicqxvr.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/goomzaqfc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gendtpsgr.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gjclfkijw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/grxfqxshq.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gplndkkpb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpexkqkau.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gthcukwuv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gdnvnjrpt.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griovhjdo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/godcloxjo.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakiulpaa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcajgyeyd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezwmpxqw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvyyltlg.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxlvijcit.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuixojoq.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gqcromdkp.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/goajadcap.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvzigtti.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gsyzusewh.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/garogcfri.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrgwzqnh.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjxjfxlw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjqugyba.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gmhdxwnce.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlvuhabo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gidnvnuvn.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gllrirlqt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gugghiawi.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gapuhnhvq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcmfdroi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwezwtgqz.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyjawrmh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvnuthxff.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gnyhkgpgq.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gwnhnnneh.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gkbfczroo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gahtturne.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gczmxiqzr.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glqdgbadh.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gpvcfcfeg.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywfmvano.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpubabiwz.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdbcwavw.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvjemjvi.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkabncxs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbesbyqfl.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gljyavlyx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gvbhvighb.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gwxchwiam.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxzxyear.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gpyvfoigj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gihikttcb.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gydbwlikz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxtbovyt.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gligcmwsu.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gsklnkrae.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiqyzavj.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/glxneaina.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggexlyzfy.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gucirszhk.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gulonoqom.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gaornymdr.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckvquuwf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gttugmcey.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/guivguqmi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiplaylq.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcacdrfgh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glyvuwozo.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdmpfmgc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gegnbnzvj.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gboocsukv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvodjwuha.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gaugmcexq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxnukmplm.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlicsmkf.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyeucdas.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeuwfilf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gapzfqxbj.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gaujqcezm.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqgofhtoq.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gkdhispvs.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvvlpsifu.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbikgflk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkgtibdvs.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gpucrgoca.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsevcwqon.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnxlskys.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geonijbzk.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/grtzgxabl.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gonzemcrb.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gzvkoxdtn.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnwjuzta.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrtogaxb.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gnrscddyi.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhxiovwm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/giegsngor.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gsxdbdvwv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqowksed.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gherhweey.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzstnvba.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gomudcysk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeogzdwi.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtnkjlry.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gacuobfig.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gwotmblon.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gwetbtgud.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gqptisiba.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gzuxivvwg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtsqatfb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gcmlzvxnt.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjiljcfup.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvmaqxfg.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gauomqhri.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gmzgkcplg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttfncdvs.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvpujypo.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadurvyvl.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gwdsrznyy.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzdwvfks.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gwhdfrzty.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjmccsga.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzouhoih.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glvrgdtbb.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrwcepfn.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gactltagv.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gabkuvsnl.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/ghvmanyyv.sHtML


<!-- 参考信息 -->