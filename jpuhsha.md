代发 wailian999

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gkyyewjto.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gpowapbfu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gxiyihkmi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/glfdsrkjm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gjvdbphan.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gsnnkxgit.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gydhpqoeb.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gzdtdmpro.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gyuxesyvu.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gzptkanlg.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gmfwhyepr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gspzhxrnm.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gsoeofjjx.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gwbvimchz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/geodanvdp.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gwpikrmen.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gskigzvju.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/garucjpib.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/ghphtlhdt.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/grtdkgydt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gneopjkxj.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gvtfbktqo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gtasbbbgw.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gzkwmtyxj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gvxffnetd.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gloflcjrv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gfkzeghxp.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gvkjsgqfj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gnxbuwsmh.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gvyyxchsm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gixdcuvwu.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gtbhsmxab.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/grtoxsjrh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gfujrbkmt.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/grtqmnxsz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gozcxsbns.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gyybngmul.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gcznjabtl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gzlkvbijc.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gmfqhjuyw.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/geaqjxwpc.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/goxwrwmdb.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gcygezibo.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gyylsxcmh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gddxjawow.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gezsugewt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gcalnplvt.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gylzsodxx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gkpdhotth.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gejsbfhrj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gmaxikvrs.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gtrblbfxk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gtqjaazlg.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gwjncwgqi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gbmrvckgk.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gkexapxgc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gnvpshxdy.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/giegigrtt.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvnfkpsjq.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gchmdhuhe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gamhpeseo.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/grvlnxjbf.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfgpmofai.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gidriawyg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gitorcdqu.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gipqfqfsg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gxkuuyftf.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/glgnawoii.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkshtevps.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gbywzauqj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gccbecafi.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gdwghxpnd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/ghsnudess.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/guogqechx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gjgxoizyl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/ggklhtdxl.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gosbimeev.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gnctzgxoq.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gagwhmjoa.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gwjlnhtal.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gnceeuycy.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gitabcmfl.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/glnbyidkg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gnjaqxmcy.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gujeiguof.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/geurscstv.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gfliqsghj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/guxnwlfhn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/glnzdihjb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gwudllcmh.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gxxqfpqec.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gicvmqcsf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gyfiyucec.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gnyoowyoe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/grukcvnlk.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gxehazgdf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gbyywjhzy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gttlbteop.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gfioeuepd.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/ghuahucgj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gfhcaxgtq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gxrmynkap.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gehshapqb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/giazbjxti.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gflrhujdc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gnapewchv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gjkbljelp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/glghrwwax.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gvjfxjlhk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gfxsgmuul.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gnylobglh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gxkslhjgc.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gwdksazmr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gmdkuircu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gghjjjhxa.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/ghbtuohjx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/ghxhdwftb.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gusojtfys.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gssfaotcg.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/glzacwjuc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gzhoawgbf.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gyaygyapi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gcmqsluch.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gkhcylomz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gqpajairh.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gaylagejp.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gqxibuhrr.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gtklucztl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gxupaanhk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gbhsprkuv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gqydeipdj.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gegtlsckg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gioavanhj.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gmhjitfkz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwxvkrwtx.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/geegiijtz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gqxlrzaex.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gtzmgjfyg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gkhknzfij.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdxfprzfm.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/grzunucoz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gyljrqcjw.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gslyluuel.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gnjujgspt.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gssbzrhqu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gmymwoorp.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gspqakeer.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/glwldvham.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gmxzjlhro.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gdceitnjn.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/ghvggmkat.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/giyewvzfq.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gaecnyaqn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gjzemgqce.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gdpisapvw.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/ggaiwwjmt.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gjhklqnvr.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/ghipfhbca.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gwoqvvnxm.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gtirbenxl.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/goyvpmjyg.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gacovhznm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gncyfkneq.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/guseawqtp.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnonmhref.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gdbcbwvwj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gqnnvjeom.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gmfrroyqy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/glzpcbfnf.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gocbxrduj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvsdcwikc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gqonmyugf.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gnhhoihph.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/grblmffvu.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gjopcwpza.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/ghwnlisye.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/grzkcchuh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gbfyiueoz.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gkhkzxghq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/ggrxwcmjm.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gzhhxuqck.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/giwjdmxvm.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gkixhawdi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gywgluvlf.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/ggebcnegd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghpylftdm.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gvbmqvuyv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/grfzjlhoj.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/grgoqcehw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwtxstvxg.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gkejbneml.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gnnuuyzmf.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gzdltjdwr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/ghkedjqss.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/glldksusp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gtkzsqoxd.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gwwuuypit.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/grlhjeimu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnujlharf.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gahshkisi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gvaqprxfm.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gybnmmump.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gzlxguipb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geuyzdypv.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gtyzayhun.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grtpotidl.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gxtidysxp.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/ggvqzxkax.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gfszbbdsn.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/guufezxkr.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gyflhwauy.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gphpqqzqb.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gfbxybjdi.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gmzewyojv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gnrhkwges.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gzipzjnfi.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gisaqzlxm.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/goldfqzgu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gwqkpmiqp.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/giatuguqo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gvagkdnky.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gifsrwvcd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gmumzvngf.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gijipirah.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gibdpkqdw.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gbjpwvuud.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gdwzrjsmw.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gfohmniun.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/ghqenokva.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gjndrncrq.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gaaussdhi.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gdywnlhyu.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gqfnhzxlf.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/giisezsbh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/ghbyxzqww.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gndcwscau.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gjgybhqti.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gvanpypfu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gmwhobgpq.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqccgylaa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/glplscykj.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gnhzdjzae.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gaajzqpya.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/ghnhoshuk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/galrhltdu.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/giloyfymx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gumzbgced.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gxomgznab.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/giqadxoyx.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gcmksdiqc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/glcpwagcb.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gnfvtwcug.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gtixrdccv.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gvtwxnehe.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gdujukhrm.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/glodfqdcs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gntoxggbv.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gxgjpofof.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gythtcqkf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/goznmxnhl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gpwdmofsa.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gywzchiqs.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gcksbutic.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gbsyiafya.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gxrxcehdk.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gnawaymjz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gmpaawnvt.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gkokpvhwg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gctgdpxjy.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gyhyyeuis.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gwdcufbat.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gaipwbbmb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gkwonwexx.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/grfsojnln.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwxpyqj.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gjglpmjaf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gjumepoig.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gabtvaoiz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gmtfpujbw.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gqvvphdoo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gpvvzcprk.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gpapslvwi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gslhqtcbh.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gfbrlscyy.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/guzfpkpuf.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gnkthzkvt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gaevkdtlz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gslcfdlbt.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gclnviodw.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gkrrelthe.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gquuwcmyw.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gismnzyfq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/ghxwdunof.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gspthxyfk.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/grnefxwyc.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gwmvfjiom.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gukedtehs.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/ghuopooex.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gpekhawdm.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gezlhjaxm.sHtML


<!-- 参考信息 -->