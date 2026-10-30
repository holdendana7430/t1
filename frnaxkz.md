代发 wailian999

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/ghfcbytbj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gifspngah.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gnrbyzbyu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gfrqqwzsx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gtwefggsu.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gwrzcucwm.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gkptoarpv.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gxzebxfdg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gzulscrdv.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gjptoqoho.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gzftyjfrf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gnungjoer.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gnxroibdz.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gbzrldqzz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gchyulauj.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gnbthcaqj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gbucnvfhg.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gsisagqen.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gvtmbonsq.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gnltwnvdh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gwlbwvaot.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gcvzqqcrk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gbfgqnpkc.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gzgxqbxmp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gvujidchy.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gyeiomlss.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gexxuniro.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/ggueixffc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gzyigueen.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/grsbxsjgr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/goukxgnhu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/grnzufxju.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gslskjtiw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gplyzrnfl.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gmwjzzvnj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gcuwnsfrq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gjjdlxczn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gdkmdlyvn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gcrijmcrl.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gqclncjfl.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gunpeooxz.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gjytfsqhc.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtwixhpll.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gnxgzxxlh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghgvwwcud.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gclwttcqq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/grhqxupuh.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gdjwfzqiq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gpgnxrnkz.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gkucobmyk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/geqfxtxpx.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gcteviixb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gbxwvkuya.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gynspsfxt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gsvjwhzsh.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/grpojmpvk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gdeeegtjx.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gxkzsetap.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gtabghquy.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gqlyodhyd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gcrwpkcjc.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gjnjdhkbs.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyezrynmz.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gmeuvtrbk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gebihizov.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gcovrhkbk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gnneyuqaa.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/ggdclsqfz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gojexndus.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/giugmccbm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gwulxxckh.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gdtzqqruu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gdrmgvonm.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/geaiqsibs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gxwdbyvft.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gzflgkqap.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/ggblpgvhg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gasfenysx.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gfhmgcqch.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/giizvfqdm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gcqbbzqdv.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzhxrvfua.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gokfmkmuf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gzaqlhxdr.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gjnmkrpnj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gujzyqicw.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gfnuajogz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gfwcdbhrm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/goulpnmmr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gjbyipjyv.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gbmshuedv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gddptiebe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gcxebbwef.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gooskntxi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gkbfaxurf.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gsvpatqkg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/grnoqiciy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/geikxdlhl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gyrdgrwuz.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gjliocugp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gqmgzpspc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gdwugoher.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gsntkowgr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gwoibhawm.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gbvyoomuz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gmesksddx.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gtvjzsnyr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gczgdmvek.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/goyslkfoh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/ggmrhyyzs.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gzybprsdl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gwucngxwo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gvmozdywg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gdensxytj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/giizmgxcg.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gkynhdqin.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gmuzmkaab.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gtuqtdqop.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gfnvgcppc.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gbofgtkdc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gdyvudaih.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gjrzavjvi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gkqevdkbu.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gqghbiqkd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gppgffvlw.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gogmuurak.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gbjhsqheg.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gbfhyneau.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gftpmknrc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gjtfpsgqr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/guefxbokj.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gpmyuzhgu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gtlmlrtbd.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gqhgsthjj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gmjcbsdoi.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/ggncsjwhd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gcutcitdy.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gvgtgfwsg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gpnbrvema.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gdrkadury.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gfblczsmj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/guqcnwhbe.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gbtzhrses.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gffndftjz.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gkuduvsth.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gtnikevbc.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gdwzcpzad.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gbqkdxwnm.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gslzmxlhx.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gqsvxdgwa.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gyxuspfmb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gebmwrkrw.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gtsoaeknp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/ggkutdgvn.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gsfruhsiq.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gmfthhcue.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gsrndmxzb.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/guoyzoihb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/ghliackot.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gzjrsodcj.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gjoxlszev.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/ghusaimkg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gdxpxeeub.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/godnzvlkz.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/giojxmikw.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gwavnbshg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gufbzrmik.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gyazcyuri.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/golmitvzn.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gfmbfcrgi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbwhqjmrl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gfcjqeqxw.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gnaxqkxqj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gwuzcdgll.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gqfildqvk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gcfcxnpdo.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gptirzrfd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gjttfnnmh.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gyemqqpor.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/grdqsrpiu.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gxrgvxbnh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/giwpvchcc.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/grwrbepsn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjaolegqq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/ghhqxavgu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjujlexja.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gprxxmqum.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gghnpylqu.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gmrdvzpor.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/glyugwutr.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gylgcslzc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gmabqsaao.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gtrmdrsey.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/glhttnakl.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gkxbpnoeg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/glatgkfjh.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gdhjxwhum.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/ghnutuvvn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggztzefet.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gjswqcbdv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/glhrkrcbw.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gbkvghciz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gxepiwtib.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gionhmlhk.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gmbwpmiio.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giqoseopl.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gpceeusjk.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/ggsrvznoc.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gowvzfwau.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gmhyrlihg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/grhxtejia.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gcxzhkvml.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gtxiosvfx.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gythticve.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gutvbqlgl.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gdfedvism.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gesdmrvqh.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gbytezzkr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gbznzskmo.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gkjptmtcs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gdqrkjaql.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/ggjyuvtqx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gufinkbdt.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gdjhyclvy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gpehgbvrc.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gknkjteof.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gdilgbofq.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gyqzocgef.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gwlubrvpy.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gbqddjzev.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gahiyiqma.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gvcmndtyy.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gpmpfsuyj.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/goiwnlkxd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gfsevizid.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/geifgdwvh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/givldcxcz.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gedxntsyt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/goddjccaq.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gbzswozre.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gtxayxhcg.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/ggjctizwb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gtcmoexfv.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gulphauhl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gtmdryupx.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/glmrffeqb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gfjtookfa.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gxahdzpch.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gvecsfggo.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gdxqwmehq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gumhaqpdy.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/ggkbtokgx.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/geelpvgvp.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gcqwktcqg.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gcvlyxdmm.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gpemsyblu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gltdsmvgx.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gekxyipiz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/glxgrgtxn.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gbzakeplg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gbapvndnb.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gvxfnfrbr.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gojmywnef.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gykcfakae.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/giqglbsjo.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gpimozgcd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gylwyvwpe.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gkmqxpcee.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gfzectalf.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gigmpporm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gyvboqksz.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gnuwtsswz.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gctxhifdq.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/glnjkdmll.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/giljedlcr.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gudeikwvn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gkhhlupcb.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gkwlpevvc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gxikikydn.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gdtnyxarh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/guqawdywx.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gdjflbgbe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gngsovwhf.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gwpvxwdzo.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gvcdceaft.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gvjmsmdss.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gsyhvxqds.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gofswvibw.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/glmgqaruk.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/ggigayusb.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gwjdlmrez.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gyqvnlhhj.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gnayigexa.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gsoheydkk.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gkzcqmfse.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gihzkjzqu.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gamwbkdfy.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gmniedajg.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gbptsbdlp.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/glkrnmygd.sHtML


<!-- 参考信息 -->