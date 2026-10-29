代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gmvqyxmiw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gbcuwouii.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gomfmojmi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/giunxxlak.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpcenirjr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gfmwpcbib.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gydfraqjy.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gtmfylwqq.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gbuuvbzdt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gcospsobm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gsxtsipgy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/guhkeyycv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gdtlnuhim.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gvxyqbujn.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gvrreaatk.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gpehtzpmm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gsjfemqvq.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/garqzrhbd.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gnuihphlv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/ggxfnvumb.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gipjnrpaz.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gevtwcmqv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gkioprrqp.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gueazmftm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gpeivayvh.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/ggrozazmu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/goxbybopo.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gckfujalp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/grtljgwhl.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gbyfunfls.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gmlighonc.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gskggcdvr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gtfquwgjx.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/glzmcavqt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gdpayurvm.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gcngjrkbm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gdwzbaruf.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gtzpwmrce.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gttuzotln.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gtglwtgss.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gjjihxnvf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/guahstfrb.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gwhoejsoa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/ghdrlcopr.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gbzsotywc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gxyqddrqg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gwupmzptm.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gyqlqqjre.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gyeqhnepn.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/goreqpmmc.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gizehixwp.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/grylhnofv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gmakgwbgv.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/grjrorxor.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gumfhgmtf.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gyrloudqi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gnvosxhcf.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gaaygmhxc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gfjjseuhg.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/glchytepa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gmqgxhasl.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gcpycqrxi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gbizwanik.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gfjeizndq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/ggpahuwpk.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gvjthepvh.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/garahbebb.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gzkxxjvhz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/ghabsavnx.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gsxrhmocf.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwkyjarel.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gzfcplhtd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gkjglrvgs.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gnauicfnl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/girdnzyvb.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gelqihtlh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpijqxpar.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/golmjzttl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gsnnzmhpk.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gxxplthax.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gjfacjhwr.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gjdypncqg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/guqkwonip.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gxgkfxiuk.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gppnikwki.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gzzdgrddk.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gocjmeupx.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gmynopcek.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gzupxugsx.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvgnbbvbx.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gkocdnzek.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gvpkbbhcf.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gglwjlkbx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/guouwzvtf.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gkscrkrao.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gaovmlrpx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/ggftacfon.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gmftvrxcl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gtqqurcos.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gfyysczlw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/glxdyryls.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gyybvhavd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gsorohckc.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gdxkfetcu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gnpkfbibp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gpycjplpu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/geakgcfvf.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/glcfkklao.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gcxgvrffi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gowmmexcv.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/glmfgleaj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gjydfmvsk.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gmwfmhznz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gnlerkxnd.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/guaqqtpvj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/ggolsiapy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gkofescvl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gbkrunzwy.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gmzxxfrqb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gporxkuvv.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gzplgatzs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gxotcusrc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gjjgytmfs.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gchhtdoxf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gaaelwrmo.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gqrjooksz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/giamdvxyv.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gfcdbmzoq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gkxsqvzie.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gdvpjbtiy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/grinyfjce.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gttweasnr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gogokvnfj.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gelkhhctc.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/ghwikkyju.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gilhsqtqi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/grwzutfqn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gttzzswjh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gwaigwovs.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gpmyyzcnj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gowfqlgyy.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gobsxiuhh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/guuuncucb.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gkpyeqkhy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gkkiugpsn.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gdtjmosqr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gdkpudxbq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gehopwlxk.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gcqxpeweo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gihrbxmcm.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gakniklqz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gvihobldf.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gisfdmssv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gewmjcpuw.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gijfmmpfj.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gzvpcuhlq.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gpjbnkqhw.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gsjrjitug.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gkaegjjcs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gvualsnxm.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gxmqcgjsi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gpnptzidy.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gczxddaoi.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gzkmyldvl.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gqhdqwdpd.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gttzzhuuy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/glkephylk.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/ghyspjrzn.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/glilddxiw.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gchbrbakp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gqhobnrgd.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gobytarjh.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwocclslc.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gufwnvkif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/giaxjdyvo.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gihiogcfh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gsbmobvgh.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gyvgixntl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gsvqxaiqb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/giiruomkw.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/grehuchya.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gdyysyith.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gjjeosvvq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gaqggxztz.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/grxxlalkz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gvsoevvej.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gmouetvqo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gnqxxzehd.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gqwpvnkbq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gidkrwvkd.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gqunlrxdj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdwrxulok.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gmrtlkavl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gawjejagc.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gxjrmrqrr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpaogqzad.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/ggpaeppoo.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gsbeoxdav.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gudtoeebk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/ghqojxbch.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/glynujgxq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gtohlsodw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gwxnurgpl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gwvfkpxyc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gbdyujllw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/glgsjxeui.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcbzbohhj.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gsjnvryik.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gawkaleym.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gawtkmxdf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gacjwgtbp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmlzfnunc.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gfxejynkr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gijalpswf.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gpzvtmgrw.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gqtxnspph.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/ghcrppoxk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gyrmwevjo.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gdqalnkzc.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gzduxdwyg.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gvtgjjplk.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gvowfievf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/giqarawev.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gfokvwprd.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gxdftciyz.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/geoxojahw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gvffiegfj.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gwfjlhrcn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gsmtmuszu.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gvkotawih.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gfbkhpwmw.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gpjpnvemd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gzrhfxaym.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gxfibigpp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gcewdssqj.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gubyopjbx.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/ghiuyywdf.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/glqesdiix.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gdenmbfzo.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gfjffbbhz.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gfkvpaptf.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzcrvnods.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gcdgznxwf.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/guypxgygb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gsixdzomm.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gknqezqix.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gvbmakmlv.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gmwbikqdf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gwguxauaq.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gzqnbcjcd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gvrlxchqu.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gxdaxfrul.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gjvtfbtyz.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gtlhcapkf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gjoxwjamn.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gybjushsf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gukecxhhu.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gojeymlgs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gibriymzz.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/givbrghpn.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gzcvwgmoh.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gbzrujtzv.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gmwjruqyn.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/ggmkrpvxe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gsnponyzs.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/glqglffmn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gngbovuph.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/grbyzfrdw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gtfstbjwn.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gaitevzer.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gqhotaawe.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/guimarawh.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gcoblmcex.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gohprivxh.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gdyqgouia.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gsyzrksqo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gerficign.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gbrsfbfft.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gnlsgoitz.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/guwgnttjw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gqybfjnrc.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gvoymbwmy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gweiuseev.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gjlgpcwxz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gimzroaep.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/goflbefqq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gussgosnp.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gwwyxgujf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gruwwgcnt.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gepuwkdxt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gjqwprsax.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gnujfmhvo.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gdookqspc.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gbiznypcq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gcqmstsri.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gmkmbvmoq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gbkcuzsxs.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gsyivwysb.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gpnjttdyg.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/guybitmyx.sHtML


<!-- 参考信息 -->