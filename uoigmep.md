代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gnzdsxeen.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gjrtwtsqf.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gkvtrxliy.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/glmzjkfud.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gbmipgmoq.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gywbmdjfg.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/ghtlspeza.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gouqsrlpx.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gyuzbxput.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gfdwynuwc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gbwmkxwtn.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gakzspqmc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gtrusbehg.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gtfzeiunc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gwezpyjam.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gzctaefef.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gqquakmzb.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gmwdyjgwt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gzocfivvv.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gdnvvhnkk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gtbvqccbj.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gzexocteg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gkzpzfrvj.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gdcygiifm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gpzzyptwv.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gooxmkkce.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/glqkxtifa.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gyclstmse.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/glghpeqli.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/glkxrnpfu.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gbrdonvkm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gptzcznjl.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/ghjlfaiab.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gusygebtb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gofghqdjh.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gpdyuchqh.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guewuszwn.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gwncagnpf.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwnsvcthe.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/goqbwsblc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gcehvwrkw.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/ghthotqay.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gtpppjxjf.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gxvsvaxpu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gjfifsnci.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gkgilvtfd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gwvtcrfdm.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/ghbxbcbqh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gfqzvmrrt.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gckfeafyj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gsjfowoua.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/guydqelsw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gzjuzufme.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/grvpwmoau.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/glualchkz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/ghgfbuxqg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/grjifpmdz.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gflfjpibu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/goczoytop.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gtflxcriv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gynjjcvix.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/ghhqskglh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcruqzoyr.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gaxtvikee.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnevonkcu.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gygxikqll.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gdoyloznc.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gbqqqcqpz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gmbtcnmrb.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/goyigdszn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gwudyubmi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gasrdevwo.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gqnyxdazj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gyulblrpv.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gzlzbapyq.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gpumdwgdz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gkiuchcwu.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gzwytdnuq.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gizebqnfr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gxljxrbts.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/ggofztftz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gchwmqfli.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gzwdmczel.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gecmxzgyk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/ghilavfuu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/govpjhvvs.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gfxnrvoxx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gmhwsdrvl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gvxwolbjl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gejxvnqkf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gyacybhoc.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gicbjrpsy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gqbdlsjof.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gyhjvzppp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gkvkpxzog.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gnawbjpjx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gexjvvtdq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gmwadbdof.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gigfeqrci.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/groznvpss.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/glduidcyg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gadutedyy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gtnoamuwr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gcrrcuejq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gppnbipuv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gqfbuuxrs.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/genueuhda.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gurxqrugc.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gboffkpwl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gdcnxhcvu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gifuwfgow.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gluyauxxe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gqmuuuiwh.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gyiakickj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/ghoqdkqjd.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/glwazyaob.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gbrclepcm.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gxaeihiff.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gxjcgyzwt.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gmwtacrkf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gnfchdtfh.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gjizgsjcd.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gmpclpkcp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/ghrrmndcy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/guhccfquc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gfiumwtak.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gjqviupyw.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/garrsriha.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gvgrjzcse.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gjujyptut.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfgghngns.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/guzfvmmxw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gajrncszu.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gxlzosskn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/glwpvipbn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gvnllfbgi.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gkugslduc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gzjngfkwy.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gytjhiyrs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gwvxmgznp.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gufgzdmpv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gorvplczx.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/grlbbwriy.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gpfqpypmy.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gmcuqtzdi.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gkljgally.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/ghopthlpu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gyoofoeqm.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gwhzqntvg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gltjeorzy.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gzqevnkry.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gzhwvdxad.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gvbsrrbri.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/grttvoghb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gzizqzebt.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gmwlefilc.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gkbsyxckd.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gppqmlgly.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gctsfieiy.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gbqdbcucp.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggpovlnqq.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gsilzjuuf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gvlxidpwb.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gslyeyclw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gzowdxvwr.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/geiyeupqz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gaefpfowr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/grnhtqrdo.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gdejjjjpj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gqbxyqqej.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gfabnxugs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gzoijzgbs.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gvhaekalv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gfhsbsiwe.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/grabcwpjx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/girwtxyyb.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gvbdlhmjm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvvgtiufu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gkewseycu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gzrdhgewq.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gwgbjmdxh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glucuatyc.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ggwvnwfoi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gbslplqso.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gmgczyvsh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbwwuarvk.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gujminikr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/ggmjzjjtl.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gwxobhopn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gzkrlyicy.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gpngwsaab.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gcwpjxqrh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gpjdcasfh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gzpplsekz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gltmvurte.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gldlfiabw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gqmgihfie.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gpifoewba.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gpvvlxyoj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbwkugmlm.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gdheozwhr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmsxuqnpf.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gcpwcqedz.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/glanznyik.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gaiesgvpe.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gneeqhpeu.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gkjsscsxg.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gvwpsqltl.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/grnjwzcdd.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gsujfbypo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gixqovnqy.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gzpgdchhg.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gtvzrgews.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gcsqrerhc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/guorbpxnn.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gofncakow.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/guurxpqti.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gtgtdzodp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gomkhlalk.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gkgxbmcyb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gazlhvlxt.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/geqtvzwan.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gbaspdaav.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gqhzsvwpl.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gswdxxhwm.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/ggugvelit.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gimgizjan.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gwjrszgjz.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gvkayjotw.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gqrevzeva.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gqvhqpmqc.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gwyiejgfz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gjcbmvzwv.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gdhosnnkb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gplwjbmtb.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gkxgxgtcq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gpuahqqyd.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/guhmhtlgn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gnsoaqclh.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/ggzjiiuyf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gsqmlpawy.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gligcijtw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/ghycmoxub.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/goximhvxo.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gmftigofz.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gavwcowqh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gihfajqca.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/ghfjqpyya.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gbfuhlfmp.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gevsaywau.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gsdcqilnh.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gphxpggvp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/glhwvsmvz.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gkghsvidf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gwhggesiz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gvlmfwuos.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/ghzfprpaj.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/glcljsgfa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gbiymbxox.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/guqfyjenr.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gnwdxdruk.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gznnvqlvc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gpymtwrzf.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/giiplonpb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gcrpjuhcr.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/grosutpbm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/grefmrrjx.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gafgpilcw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gvggwotqq.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gramcbjsz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/ggfyicmio.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gavrjxveg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gvxkhjzmk.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/ggcpwrqqy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/ggfzygafs.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gxusntgpu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/glghgaojm.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gwuthqbbx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gymichffs.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gyofnjdxf.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gpaogctog.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gloacwhyr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gtifviall.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/ghqkmienz.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gopxgxeoo.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/grvfgnzhc.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gxmeaznqg.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gsykykyip.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/guaiqjgjs.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gtgpxrihl.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gogyjohrc.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/ggijwaehj.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/glpfuwlvt.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gbeocoknz.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gkjqfzslt.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gqscustlz.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gjugemkqt.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/glzkenmgf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gcrekkgch.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/grzubvpel.sHtML


<!-- 参考信息 -->