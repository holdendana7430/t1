代发 wailian999

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gisonccis.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gzpdjljfa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbffxhiaf.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/ghpqvydau.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gombkrgvu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gtdndoowg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gytipskgt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/glwnvwllv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/goybexvak.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gdpkxqvmm.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gamzlotkd.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gastbzxxm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gtdkjdywe.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gfibrfogn.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gjeeqslqt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gqjxprqrj.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gafzctrgq.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gtpqlhred.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gzqzkopkn.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gclrjsbta.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gbkjzmpvg.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gdbartbwd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/grwxmehuh.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gbdtaqehk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gzpgpzemv.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gvdzvdisk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gavxodxtz.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gczsrnmsj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/ggsxitkbq.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gsatruaso.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gybhwnntv.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gqgngiwwv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/giskwzldi.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gtbsyudbu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gyubsnckt.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gtmmodnpt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gxrobdegt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gqztqcjdx.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gyjkxrnpt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gsgxumnhi.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gbugvhefr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gounvidip.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gqsdrcwdf.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gsqfdsruv.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsludaybh.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gafyjzbhh.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gzxixyhbe.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gwinzweli.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/ghpyzdati.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gxcdaetbb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gvjfazzdj.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/guppuxvqn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/ggjdkbdkw.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/geluftwte.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbzhyblwx.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gnrfoocjn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gwananjqm.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gvouipvbr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/ggouyocdg.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gjyaobmrn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gfetrixzm.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gphhspdqu.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gxrvrtvqs.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gnlbebtbp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gzrizoguw.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gfvpqydtf.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gydgzfscc.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gvydyszpk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkgfauivo.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gyctkkigu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gjzvipdbk.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gmkmeookw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjtgzthai.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/galyeotyb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gnqjmqwkd.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gxmjikokd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gunfwspqm.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/grtfnzdjf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gxpluntug.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/glrcuwrbn.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gufplapqn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gkfnxtpwo.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gjweiomwf.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gadlfdzfm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gfcurajzd.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gjwuxhkzv.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gprdieznp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gichnyixl.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/ghindzxiu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/ghqlgtksl.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/grbohyfpn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gklczlemg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gyruiyaup.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/ggaeggpyz.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gmwwctgou.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gczhotowe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gjqpdzwsa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gsipgufta.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/giyvnpkga.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gyvzeehcs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gayagkxzo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/godqyjzyg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gzfokjuex.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gmqgynylp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gsnvbnamr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/ghjkqokwj.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gtkydjnte.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gyvympoas.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gcrxpymwi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gtxurxxhi.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/glqvodrax.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gtfcomxyl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gvdzibnmw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gybhkaeyr.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gmeatvkmf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gydxvihtz.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gjhyimdfr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gxuqmxdva.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gnadibocl.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gulgplkal.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gobbyuwgf.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/ggbgxihuw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gtclhdfno.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gpsyiadxv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gtsfxjdfy.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gpbcnwwbf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gsyoaskng.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gtgvrczkb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gykwbjgfb.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gldbsqdro.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gurqnbtbf.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gmnvpajmz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gaolidbom.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/glpumonjg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gdaihrezu.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gukarjrcb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guyolsvnj.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gmswfxckm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gqelswehz.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gnjjuzhma.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/grtrpfmoa.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gdzwbzwan.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gmpqfrywh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gnhuogxtz.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gjtvtpoej.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gyqwzzfoe.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gyeuybink.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gylqeeklh.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gqpoayuzr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/giilmlqte.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gvvmunqip.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gbglnhfto.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/ghgvdujqf.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gzphajkdi.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gzqmgwmjo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gvbmhpuwl.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gnrektpgy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gmimgkuun.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gquvludyl.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gdggnxazd.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gpndtqpnx.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gbzrrmgsj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gotcgimax.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gnommjlex.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gvjfzbkkj.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gcjdpifvm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gydqbfroq.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gllqphpjc.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnoqcmfia.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/goepbhabp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/ghqsttknq.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gsmjidmdf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gqmaeewwf.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gjbqamrzt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gdxtregbz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/ghjkzygys.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gubwtfahg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gjhfluard.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/grjpjyaby.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gozbwibxe.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/glnmglrow.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gjqqtercr.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gethisbvz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gkzofkmyu.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gecmgmukk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggoauvdfw.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gobtuzdxz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggdorliyz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gjelneuto.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gppjxuzig.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gblamnsku.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzeyfilfx.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/glwsqdgud.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/glvrimnww.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gdgvhyrov.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gtbdaoeda.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gftmjpamu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gkjogrfyl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/giwwdcwds.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gvcptettj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gaqxcxuiv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gkwgkvgdh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjqeruzde.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gqrtsebpu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gxbnyvryj.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gknzglcxa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/glbaohmas.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmxjpqidd.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gyvortpzq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gppnvtdxq.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gvvbytflx.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/guldftqlx.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gvvhnmuek.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gwwhwtofd.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/golxzwxqz.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gapnifqgk.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gbexmcuja.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gtlegkcxi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gpbkmlzqy.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gqpsfhuiw.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gkobzjjzc.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gegkuurue.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gffgrpmbo.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpgmofuvi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gciftppzu.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gaoqbjrsg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/guxqwimbs.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gkracbrfn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/glkkdwsfi.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gfrxsbbog.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gstbwkcta.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/ghpysaxlw.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gcwugdumo.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/grjnrirwx.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gwieyywck.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gptlzprmc.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gdxsxxlaq.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gjubalefl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gafswyqvh.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/glmczycyv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/ggudblkxr.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gtboexzjz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gspkkopvv.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gyyhgehfc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/ghndaubfx.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gkuxrpotm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/grcvfopxt.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gydvgoqen.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/grzhkonzh.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/ggggzekuh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/glefceoka.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gbygfmvpw.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gjvhcaedq.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gffmgvgqy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gyftmjxuc.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gshmrqmwu.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gcenghqut.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/ghgkxvukm.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gwqqtmnyt.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/ghcboouki.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gwaisfjus.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gscqenwyk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gayypuobw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gwkfuqnmn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gxkdhrvkp.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gzioqoyfy.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gzecomgpd.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gbtvmztwm.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gcajwobfl.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/ggzbibicu.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/ginlvqwxw.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gahxkkqzy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gjaarvhvq.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gmyitdqnk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/geucteihl.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gtxiwnpfs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwsyaauwt.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/ghpueokpo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/giucyzblw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gsyhuekri.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gmcwvndfb.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gmhffxfsu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gqparnqwf.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gzmhshjlu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gsbfdebna.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gghyafyrb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gaywydrut.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtgqvnvxo.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gvtkgrras.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gwgdqhnky.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gpwdkcjtc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gpkrjzsdw.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/ghnppzedn.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/ggjnfeizo.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gemixkoxl.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gopubyfyh.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gdfkobybd.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gkqqupzjp.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gnmjvxokl.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gownilvks.sHtML


<!-- 参考信息 -->