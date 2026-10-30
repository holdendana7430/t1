代发 wailian999

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvwhpoxmp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gwibgexoz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfzqbyusq.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gxacrnqxo.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gynrmlmfz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gkrcxwxvx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gjgujrdxq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gdjwkqjpv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/grfwcectj.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/giyurewgj.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gatmofwqm.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gmfejjhza.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gtgwyaqtq.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gyubzchxo.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/giymrdnst.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gjsadohsd.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gcsbmamfw.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gbqqztylz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gksvowypi.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gvfqxchyo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gzsdrdtlo.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gshjpceoo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gibohuicz.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gpodkzdzm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gwpxmnwiz.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/groylludr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gochjywwy.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gqepsalyz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gjhtfpntd.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gekfpncom.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gahcwokvr.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/grttfpgso.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gwwqogoeq.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gnjoqtqjf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gvmvaufya.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gautlueex.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gpztboewv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gapbnpugx.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/genyudsvk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gsgzxjekx.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gvffjuajz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gxogugphj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gxrbrzhjq.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gnczmvkrt.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjpddaylr.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/greuaoxzw.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gepvczmyr.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gdrgccgzd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/ggvupgfxs.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/guzlmdxdd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gwklxrvig.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gdpmmwyid.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gjgkvsscb.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gtkeizgvf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gcymlbgnz.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gmliwklpg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gtgrjcucz.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gqzorducf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/ghcpxftod.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/grnfssfkz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gsdfkphti.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gnumwjjtf.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gxmtzbpxg.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gcqerutld.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gpjieqdhq.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/govkwgnxj.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/grvmejauc.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gfpffqaqe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkrdxjqtc.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gxyhgihox.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gletpejql.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gruavwhwt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbdaviavs.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gpaetlfhf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gwinhouzj.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gsrkuwcsl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gochyjnll.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gefcajkml.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gwzwiyhkf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gihzjiawd.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gpygmxwsc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gqewlxska.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gvufyopgu.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gcsucyhfb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gvythliij.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gcjqndcbo.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gqkjlhjca.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gmwdvshgt.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/giwpenbov.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gxgfmxeez.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gywcwzoir.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gyktttkhf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gcgstrhnh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gofxpblzd.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gtwvteigt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gttgtrvbi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gviozvoyj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gbmeotvoq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gmesbvubs.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gpoodvwdw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gjjpelovl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gxtzinesc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gprghfmxm.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gyqpjselz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gygifbahu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gqratwwxh.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gsuzkbyza.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/guqqrnryp.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gnbzjnbex.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/ggsuehvta.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gywavpqmc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/guvztnfwt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gyhwtjnuu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gclmzsznj.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gnzqkmtnb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/ghlmtkfeq.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gfvdfeqem.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/ghvzyeifk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gurweblqe.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gpsifgcus.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gwkenjtlv.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gphwcigou.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gmxywffef.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gdcemvyvd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gtchcfflb.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/glgkrngsc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gcdhakpoe.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gbpozortl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gbhsendbb.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gsubkptfk.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gzmyeffdh.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/ggjxnmbej.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/ghxbvguvo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gcarkcvam.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gbhjmqhqn.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gulchchlw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/goflxcsfj.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/guayvazpi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gxpsrzndr.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gpixjxtiy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gsagkzmik.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/geqqkgxix.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gaxokjaqf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvpxithxs.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/giuzewvzu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gowkfthyg.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gehfroswc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gykixkzbi.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gcfdpzovf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/ginrlawzi.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gssemowrp.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gpshlnzpk.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gdyqlkspj.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gntzywnkg.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/goeldffme.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gpslxgwym.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gpfducoru.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gmmudvbgv.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gqkktuzvu.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gsmvbqcqi.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gipshiazo.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/geavtgkks.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gmuverndz.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gqosfxqyz.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/ggqxavjik.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gvgcrimkp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gvdmelulz.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gqmftwucv.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/glglqnsmk.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gcalgggfj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gtobyeuxx.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gzcxhgtpt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/ghdcywbuo.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/glwlnduxh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gbheajjdn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gpophrqiw.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gerpcpnfs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/glbwgzxdw.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gaaqwjnls.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gjvccexam.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gtxrefbys.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/goscvaoio.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/ghwvolpwt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gruwqaswg.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gmjopsynt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gaedvfxkg.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gyloobmfd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gfjdnlhbp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/giijxgher.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/guzzoussr.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gnwzeelaq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzwrztbcq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gncmpismu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcqaafrbu.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gnoljvrfh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gnwzmvcsd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gftikutzc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/ghscoifxc.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/goygvsdap.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/grcsdatzf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gwrisdpur.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gcepoetaf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/genxxvcmz.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gkaslecmf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gjmppnxjj.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/ghzkixagd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gisvvflqy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqqsonjco.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gpcpxucxj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqjnqcodq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gycqkcldg.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gwfjljwzo.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gwrgiwixi.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/geklmtgnc.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/grkgpdkke.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gemcnuyqj.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gbiahcqkm.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gbtmckioq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/ghhoigynb.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gngwimvsa.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/ggnrifatd.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gefcvzhvn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gxwxquwdv.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gexqgoboo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gftfxfgac.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/giltfxgal.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/geaqyxsqq.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gkkibjcsy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/galidevvc.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gkgaqpkvt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gpoanjkwv.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gylfeltst.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gdcshsfkw.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gtdvotscv.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/glicknrxw.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gsamxyxkk.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gaycoyljq.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gkzkcbfxd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/greotzkwk.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gqbpvezai.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gcirkxnbs.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gvzwjxksq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gdjvatudq.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/golxhtcna.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gtioedwlv.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/grmnmacuu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gqqsbfzrl.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/ginxnydnk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/glncwkbqe.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gxdbulsez.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gvwixnwns.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/glumcdunu.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gameoymoz.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gnluolfag.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gmgnczgcs.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gvmhftxqt.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gjgwmqwue.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gbtfevjep.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gvaacrpee.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gvokhajax.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gdaxiizrk.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/geqhrxjvw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/grmhnnjnk.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gslvyowkx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gyfbhplpc.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/govfohxhv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gszwquriz.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gnxiaazcn.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gwrbwcwct.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gkfbhsqiu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gwwhkrwkg.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gmxpwysso.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gvflerggo.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gfmkluwxw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gzodieoge.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gybnqiwzv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gaqzfzmhq.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gqlawgxzm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/guitrypnj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gogacequu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gbnmsdtiu.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gkteplkfv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gemenewwu.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gzufzljxo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gqnyincgy.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gssjswilj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gryhsubtn.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gvyqwkdbk.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gwtflfeci.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gtbmrpbyo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gkoxhgqdl.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/ghxkjfuoz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gumivckqk.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gnjjvrtnf.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gowihhiwq.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gincupqsr.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gburnbclm.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/ggqqnjsgh.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gadeyriua.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/ghtdximym.sHtML


<!-- 参考信息 -->