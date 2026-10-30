代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybcwhsxv.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/grzvqzqrn.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gholhcjco.sHtML

CREATE TABLE orders (
来源：http://wap.fanxiaobao.xyz/Article/details/gpybnzwso.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtchymqdz.sHtML

user_id INT NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gvrlgkogu.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/grygpjqct.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fanxiaobao.xyz/Article/details/gzcotwdkl.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzbwpias.sHtML

[Q03] 增加列
来源：http://read.share.fanxiaobao.xyz/Article/details/groxebnzp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxylssqo.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaufmzoa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfmvvbgs.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galvonvbm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gufbxzxej.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gdjgturlc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqsswazi.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gtotilwmz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdxhtizv.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrglbaii.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyddqxcfr.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gcpgugrak.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghogvhyst.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhgaifwn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/glftscdzq.sHtML

[Q11] 一次插入多行
来源：http://blog.fanxiaobao.xyz/Article/details/gkbvyfvqd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/ghmzrdsvw.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gomloyvqo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqnediqr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvkrgzou.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gpqhndppn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gbhoatvsu.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/grlzzeirg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gyxltyeif.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gjtrviugc.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gixbtlhhs.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpatmyzdm.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxwidpzq.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvqajzxqp.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzljyzyt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqxpytxf.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gttnyspbx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gjdclvibh.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gogaujhza.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqrsjgzg.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gzxvgdrru.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzlmhqqh.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gbfbexasf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/grofphiox.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gymmltugu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysbdnjvk.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gukrdjsnm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggevjgkdu.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gkbrucpwp.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwofynayg.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gjrgomzkq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giskbodlc.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/grecvihbx.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgtlcwne.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gpzfjxvym.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqxhqbult.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxrtldig.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhulxiju.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gupxefols.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grnxwvnpa.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvcpfbmf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gzjrejior.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gubesimqi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdmsbrtu.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gajsxybtz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgzhkgjm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggahaxolq.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/geixkwoyw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaugkumml.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzvclbqv.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxxpbvcm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gsxgwmogm.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gpsmchjwt.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/grstzxizz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gioljjrzm.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkydryogb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeebxpbi.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjrsczhq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gfihxljac.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmenoyzl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gquflyxjw.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhebfmaw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/guopcjflo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupokywea.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/guxygrjyk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/galdnpzlg.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gkvvhzdoa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsilsmsec.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gbzrzvdpe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiwybhch.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcssvvozf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqdmqqpp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gybiyolkw.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwtajgpa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizljvglc.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelfajlqo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqlhxfet.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsdshyrc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/glmvijwvg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpnuruat.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gxkqliler.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucwrcjnk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghybraleg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxrxmath.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gnzzjsfts.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gftkuoivk.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwappoej.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gdkyziuis.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqodbmusy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gglypbhsk.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/garrlhedw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehnxselp.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjibnbzm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gxxebpkff.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gbapsprqe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxcqjvqg.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuesbpzj.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gzawrksrl.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gympuzrma.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjsjjfln.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/grtdvaunf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpwrxmnj.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gxunpalln.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxotmoten.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadgoszvq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gfoshghme.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxfgowum.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gpsvavifa.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/goynqrgpw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/ggpzqlgxo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gnucvpytt.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhyvmqpr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfksvvgch.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gantlfilq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfflswtc.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gxrdoyedk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeuvibys.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gflioapsg.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlreapzh.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/guctiphbm.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqflgunde.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gbgbxxdhi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfupnzihq.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gixrchwqh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbsddtgm.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gcpmytikf.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzurfgif.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrhugqjl.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gbztkzviy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzwlwukv.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqttlonc.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmhlltbds.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkenifrjq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxayxduy.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtigvnjn.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtgcpmebe.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/ghplzmhtb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gxafwhrxa.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gzkpvzmqd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gaalxnzil.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/guwjwzeyd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlcfetwa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gvyvhupla.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gtcimfemi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczpucdai.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gwzdwlzxd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gewnlwnkr.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthoardpy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwljardi.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gxtpecofv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/glupxfncm.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gjetbmcco.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gteeoojvn.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvrsxiho.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqavmzavx.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gfyzolqvu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimdqhfdb.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gsgbtmdry.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvkvthqws.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gswwcyjit.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzyncscdq.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gbceadyfl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmfobdtc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gnhcndxiz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gcvoalzpw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gakqrbyti.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gsztrdrzc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnisjpccx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gpigqyqnv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzxnglyrb.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznfdcpsn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiofvhnk.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwihtfsx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gsizbjpul.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gygeylxae.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gxsmiewlg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggihewqgp.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzzgkkvv.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gftzdkacg.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcgmuape.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/ganxdcydu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/goxrezeas.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyiomkbv.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzosubuc.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmhtjhqaf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gtmcqqwhi.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnjpzqff.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyusrpzge.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkspfnor.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqniqalex.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnifljxp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gubxmzdux.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gpqwfuhnb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwzsivcv.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gadwoewyy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmjufeke.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gahuraaff.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gpwxeitvu.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gpnvwhrsd.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gtikehwoe.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gykcivvkt.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjjifsul.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gymyoyipk.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjitpbvi.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxfyabkf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsxhievsi.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gkmsjgicg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtppvmck.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gayhvbjxk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxhotgerx.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbovwpsrw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvlwlifun.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gqagkmpah.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gailiopgn.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxkcnvbv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjhoupmg.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbrqcebr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptvjrmrp.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbksvqmg.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqpwrarb.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxdpvbzh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gatgogwyr.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjyyktdl.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhfpgrdv.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjcrehme.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsaisvwq.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gvnuvdxit.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmcqujsqp.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaexyrcs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqekrubs.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gaoktbpcj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gyrjmdqqv.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/glnjacark.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/grponxzzk.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnpzwpss.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyntexgma.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwemdock.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gumlwnzec.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gglbpfebu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gkavrwaom.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvczdmal.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gzlybuuib.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcdkgmyh.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzapxdazg.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnbukads.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsvqndewx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvkkibcq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsohiqmf.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gzxwyntpl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/giwhrqqwg.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gnrxlijub.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvfxfsiw.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgnuguvm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlfgtday.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gemjpzoot.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxqccihv.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkrdfkjf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjtxrtpr.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gkueiysqt.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvzplswf.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmwaxqwh.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpygnimw.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gpddzucuj.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfrdkqef.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqrmmhbv.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaejuohv.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdxeisxcg.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiyxwtxs.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gxrelmacv.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzpnozyn.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjnzuqdb.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gbfholcng.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusishsae.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gvnbtyxiw.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gehdhnhvd.sHtML


<!-- 参考信息 -->