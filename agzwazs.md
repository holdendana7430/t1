代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/gukdtddrr.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gwvtsmihe.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/gufgvgvdr.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/glkchqkdn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmdpvhnj.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzebkmbf.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/gximegvwn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtygkhgmm.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/greoyppbz.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcleplnw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gspxcmdoz.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/ghuvicsdi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkopkltxw.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/grybwijza.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfncpjimk.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/gydzjaolx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmzqjyih.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/gmstqcbhx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuixcbao.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/grqumrbgl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/giklaoqmc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfzhiyek.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gckzzoefu.sHtML

[Q10] 插入单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gysqlsuxq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gaymggcwx.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gjotgckci.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gjyhkvqea.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gvzxqnblb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/glxtdwusb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gludvxaem.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhzvcelb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gzjaiycau.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gaseoqxrt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gvibayahz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrthxmol.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoebliwk.sHtML

SELECT * FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtjnhkwhj.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gephaoqlc.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grciorucl.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtcednwax.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkxarvmt.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gecdsbjmv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gckvotpdb.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gamvdzyrb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gruetxgni.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gjcivkkrl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gnwnuoyyj.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/glgfplcoj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gtfuwimbi.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsmxnpul.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhzceeop.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmvmbiuz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gugmeasmr.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gmkkflswl.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzacnnue.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhzgzzqa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/guwyjwjea.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerrtnipx.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/guzgteslk.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gahbazlkc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvlgjexr.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gdmwwinvy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqxnhhiq.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gbfunghhr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gyfhdkhsv.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gogwvqrbc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqodznpkj.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gyfhvbmgs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/grvffpejf.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gakcxnfoi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/glhblbvwm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/glhpgyujz.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxysjciu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxbiggpi.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gepcfyinr.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gyhjkwcea.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdnqmshg.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gkhlpttce.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnjufcpi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gcowmjhfn.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcdcfhrm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiiriopv.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzsjpgxy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gonselswe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcraqlpk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/glakeqmvk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikugycsx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gaanllkcz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gxmsatesx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixsuuevd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gwxqkzmtg.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gkzbqqwud.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gxjwxrmxp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgrumoso.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcnxqyjt.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gmebpixac.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/ggrhpasqu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwmckkrc.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/grngrnqdz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyanhfbvr.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscutxmvv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gknrmnjaf.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/ggcuhldee.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gutkntofr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gsskuzawg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejsnhgyp.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gkyyajvmu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnarlhjqj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gamttkwtj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/garkqsmmm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfmxxwnq.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/glnmwrzvh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgsnxspp.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gcpvbfutu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gvkwniypw.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gylknfyvr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grbbgqoqx.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gfzhrdwgh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goutrzukx.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gvhootauu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemuuqihh.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/ggplzskko.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwovvdput.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gadmntxkb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcquuihx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gebdccfcf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszgfdyhw.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkigvunwu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcsitxdn.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumonnfdt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwesabigm.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqivvsiw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gzdrtwpwi.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gnrxnptug.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gribmqurp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gtjytjvlk.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnegvibmp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkghhbkg.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvbahvys.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpyazcig.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjylzfzec.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbwnddyq.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gympkdksv.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfnzmmxv.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/glkhggemw.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqhjeogp.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhqpprnb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizqrnbfl.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkwprjrx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gazgqoyfk.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbezebmct.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gapxypdqb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gciaqynyx.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gzbiazozc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gwermyhyk.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/ggfybeuva.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsdgauum.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gilwrfmec.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gonavudze.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gvtbhnwja.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxpfhoxek.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/grppqmhdb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaceetnlv.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gktpjzvxz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsufrgsdx.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvjggnjy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkvlxubo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwzombzb.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjetwbjln.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gvvpcfpyo.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbzgxgde.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkjntndk.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvgjxess.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gimixizmq.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/glehmpgni.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gjmfesrzi.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrjpgyhj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvvtaaqif.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grgdsnryf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcesulfxd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndaizxlb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqltnmyy.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gpxbeljcz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gyjsuhmvl.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvanmosp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcarvycs.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/garjvmkgm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjdmfzlz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkbbxdkd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/geeowscae.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gyegpmmiz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgiebdnc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmoxzrtj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpmpfzdl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guwwyqmja.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gnojsbzke.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiniqgzd.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/grqlcnacy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gmjavvnio.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkqwluhnz.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbpicgma.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gigjlvjbp.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqqoxkqb.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gtxrbhqyq.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gtcxaaixy.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gcroogkgp.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gcrdoseic.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghxigqmmr.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gtccbioks.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gruxqjdnw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/grfmnuxqf.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzeqebev.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewsquyrq.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gghqkfdfz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goahtmlaa.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnerevoen.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrhrkdjw.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcoihqgj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gsucyofxm.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/geehehisj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gsitemeqs.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gipillyor.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gsxigozzd.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhuaervr.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwvrzqxg.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gcrkgcmmt.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtestvenz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gfpywpzkn.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/glswbbsro.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guvzrkkog.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gojhrjcrp.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbckyunta.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gesjgxbgh.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsakewoxm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gilpghzrg.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/grripkbgf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxadedoui.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxemkmasv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzkjozzmb.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gmdahjivi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjxiaixq.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/ggryunsjq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjnjjqlx.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gugboohgh.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggckfoywp.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gabifwziy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmnrmulkn.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcnwbddn.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjagllqz.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnjyiaug.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiahmpjv.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gotszcdft.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/goidscyfp.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzmvvnzc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glydddxqu.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/ghqfxatpk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/goddrrsjl.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gobefmdkl.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gshurktch.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkmrfkch.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynkuprlx.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gncjasdgd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtkvuehg.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grydrqxva.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/ggjhihkyd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawgseibs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gfurzkces.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gogzqzadq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtihtesaq.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gblldjhra.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtqlaejfr.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gyrigkjcr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gizkqgagy.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gszvchwhp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoacsmgs.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpruqitj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxknajpd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclidqfmt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcnsiaob.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gurjkgqtu.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glimwtoop.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gujcpmqrw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gyvpafhfy.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkjopfxs.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gryiwzgxb.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdowwmln.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesmqfpgm.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytaqvybx.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgdyptlt.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gcerrdbdc.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxglxdcc.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxtllvtno.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gxzjpureh.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdecnpfsi.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvojavcr.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gruoglaet.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/glfjixrlt.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gctctwdei.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkpmtnfl.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gffvalpwa.sHtML


<!-- 参考信息 -->