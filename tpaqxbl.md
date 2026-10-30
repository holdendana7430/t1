代发 wailian999

CREATE TABLE users (
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhucujoa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnsdvagk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrvdnztw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfzfupgs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtegalgr.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gjegbaecz.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtvbjgru.sHtML

CREATE TABLE orders (
来源：http://www.share.fanxiaobao.xyz/Article/details/giwbwyqed.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjgcuubc.sHtML

user_id INT NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/godfbjqwc.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyggrcev.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjccoaxtt.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdojeemzj.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/gevnlzgdi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gnyswzter.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrevgglo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gyzcszjjs.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gtatworaz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/gixbbqdcl.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/giynpqikb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/gzlgzfjzk.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwbekaiw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhydppnl.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdjfszau.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gulrkubxy.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gqvvgbdjq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzpcyqef.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoafijnl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gxebskuqk.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfyoivmm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gvkrvbwpc.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/grasilekq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fanxiaobao.xyz/Article/details/gpewuvqxr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gbphtfdxv.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gqemeuzux.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/goqwiolme.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpsxqbbh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gwvriehod.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/ghxcyaxsl.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/glpflumks.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gofghkeqe.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfylfazbv.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcgzmxdb.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gkvbtkdcq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/grhnxgqjf.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gawxjcrgc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gyunrnucs.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtrygdurl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjzapmkb.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshgdgdde.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxutdiap.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/ghrzhoqqy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqlklrlk.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gtdyaliip.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gssaewmba.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gdimmsuet.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gksakoxuh.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrdwzyci.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkondeixj.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gudcpzcga.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/gahgxovaa.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/gtllcqwmm.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkntijgis.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhgarvgi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/goxyrkpit.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/giljvdfgk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gnfmjvvnx.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gvvdlxwne.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwohaytv.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gamfkhold.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gzvciwmmp.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gizanjfxc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbzebmlm.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyylqgvfa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gofldound.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/guenjfoaz.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gtxuzvqtm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gocpjbztw.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/ghruiaeik.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwmxohey.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrrjnbuu.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glsehdifj.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gvhibjmvi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gyutkyeaa.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslyjvqhe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gqyahnuwm.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvbwzskt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrwekaij.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeianqrl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/grokbsmbq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnoenheb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gsqpkjicw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gqbfxpcmm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbwqiakn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgaxsltc.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjcwhlmj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/guhfkkkef.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzwtmaiy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/guopniqqa.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gkunbbcua.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gnujynzqc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbawqbfo.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gjuzjxuvd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gtzuvpztn.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gumdxabdh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gwjgrqurk.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/glpgznkip.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrxurymi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gxlswzudj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gatouorlp.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/ghwazmkkb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gnopckweo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmxpxgmh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbclpkkd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaxmquze.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcldnnxgr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzxxumue.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswaxmwpm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gqtojwzuu.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqbxake.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhbzndfh.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/goqympdjd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhadptla.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/giygisogo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzappdgyt.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrgxsjch.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gauzdsgpe.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhpmzkyf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gceeqfajs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gelhqifvo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkguhydyc.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gokvwedyn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvnngmfn.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gnpubohkr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhjrmqvb.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnahxmoi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvaswcdy.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gdhejndwf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gtnmfmpdq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gqudzppgc.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gjufunqae.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmofpkre.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/giepzdovm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gvgnkvdhj.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/ghafuwxyu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqivqltp.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gpuqugirb.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbuaiiok.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gctehhzbe.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdbdfjvz.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqnjjakc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gatcvignq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfeeotlj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnnztaij.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/grlpeefbp.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdtohwjl.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkhofrkt.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gkdshhgbt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gczuseiep.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrnqvper.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpoebaan.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsbubeuj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gfqfydozc.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtbefqxm.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghjspypqh.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbivedob.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/goabzazul.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gevljuyfd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gmiyisiew.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdechefl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeqtkuov.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfhxnreo.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqukepxxn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkxdhqdm.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgdayvmn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gkxrjwsji.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmxshmdu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gbdmmwjvy.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gvbaynruv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gnounlxkw.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwuxumhq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnawwvfno.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdvzdspry.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgqvhoun.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/grpvpsmsc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxbyqcayg.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbewmngyz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gywjcyozl.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoryimit.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvybhoypa.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gyvlkyomw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/goiitltkg.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gwypyfduc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurfujmoy.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gprnjgcml.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/ghdkxhyvs.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gzobizzol.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/guedfkodw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsotcykye.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gzxzpakwb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/glorcwzva.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gomwpvirx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gxltxpydz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvydlarwf.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/ggttxypad.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdcgqgzg.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gojqqzopd.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjqkrlio.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gnljsnthv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmaodjla.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkemjcyr.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsetbpjfh.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyrqoxqs.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gictheixh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gvjgufbmx.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsvvugzm.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkavwyepd.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gcapqvigb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gufltihkc.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgabfacp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxckdaqxw.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdxxjfsm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gasqduzbe.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlfshsho.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghjjpdmaj.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gqwurtqcn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfncrtad.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gtovvdmhh.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqyfibph.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gxkhwgvhp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmpjkjaj.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmsthmir.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwbjbmvw.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkskiseeb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggczuwczm.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvcpqqnn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gblbwliul.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/giimfozig.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsgxxcho.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxcuqcfns.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/guyyfeuth.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyotwtpky.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghsjydvpa.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gudfyppve.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gowjumdug.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gahrctlnc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkloqmldv.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gzwyoenkp.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtkzjqfhz.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gqguzhwkg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcryxlfrr.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/giypedldw.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gicsqkdga.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gildoiceu.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gagfdmscz.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gibxtudjf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxjinqizq.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gluaqwfdy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkzraxau.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgqdgxdr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnzhiqiu.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gekoggnox.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcowzqfg.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnldmnmh.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gvlyjeuct.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gnzdzxlgg.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gcheqtjdv.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaiayepa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvogxzvag.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/glcnpzmcu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/grzxeufnd.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwyfxyyq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnyaluqr.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/goyhklpuj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwxebiobu.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/girdrpzxs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gruxptmfm.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gekxajtca.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/griyifzlz.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gzubqjexh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gsfheutbo.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/grfkmiwmt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqdrytya.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganrleumv.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxbrsfhh.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gcbamldtv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuelqoyh.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gernoomxs.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gobzkctvt.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqqxorre.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gofgygopa.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gdocsrpfi.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsugesoo.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gbvfzywnb.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gexcdzjfi.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzdkwhxx.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gnexdskkj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyromyrf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/globaiiur.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqmgpcmx.sHtML


<!-- 参考信息 -->