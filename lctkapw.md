代发 wailian999

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzijdjgk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fanxiaobao.xyz/Article/details/gwvndwspe.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glyfeuywu.sHtML

[Q01] 创建表
来源：http://mobile.fanxiaobao.xyz/Article/details/gluxecuwk.sHtML

CREATE TABLE users (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjadbjwgh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/ghuzbpwpz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gojmjkbjn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/gflotuylj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzpwqedr.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzncfnww.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatmqtjcq.sHtML

CREATE TABLE orders (
来源：http://mobile.fanxiaobao.xyz/Article/details/gavltacdy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gzamgyfqf.sHtML

user_id INT NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjhlcqnd.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlfszfor.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/geigrwydh.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtmxtbdt.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpkkmgym.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbghejnsz.sHtML

[Q04] 修改列类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcrvtexa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghikretrk.sHtML

[Q05] 重命名列
来源：http://www.share.fanxiaobao.xyz/Article/details/gecitzpdh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvglpcxhy.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/ggffhnwva.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/gsdawbzil.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gikdlvdtf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksdjmcob.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgcimsti.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvmkjuvs.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/ghrudmfxg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/giwrusllj.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gvdgzhxkp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gzxeqicko.sHtML

[Q11] 一次插入多行
来源：http://read.share.fanxiaobao.xyz/Article/details/glwpkogbb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gfgcsumnm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaedicspm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gjysnotzp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/ganbieran.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/glwvvkmbh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gymqaevfr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gliedmmsp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgpzgylj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/ggupjjedl.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/grgkmpmly.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwnxzqad.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/ggdittfkv.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/geamkfxds.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmzcfsal.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gzsodfmor.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/ghgwhljgl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/ggbkqljto.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdscfjqb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxobwafn.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/goyuobjiv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqynzeiy.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsnkcghb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gbyebxtsp.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfncnyho.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grovmyovs.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/grrwcjzsf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gshapiwet.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/giioecxlw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsfcrjvzy.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiygacgg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/ghiazbthi.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/grpnpebdj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglrrwktu.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvogacbg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhxypvov.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/guldkcvkg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmmzwewa.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxabprcy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzgnfqrcn.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcffbikd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmreydekf.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxyyetjx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/guyjmntuz.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gllczmhrp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/ggcgutndu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gwydivnkg.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrrtxijt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gslstjzcf.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gnscqjtfy.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gouxuacyp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gxgfkaacs.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbglepyp.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gsfrwjjra.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxpetvaj.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfphoekub.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmrvllah.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gioebdpya.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpzidjhh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gzhfhxppc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfxawqei.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpkvkiqw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuiqrxcg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbldghcan.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxludvevq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/glpkgfvce.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gijabehba.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gayldcvzk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gaytgdsrf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gajouekbb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphjcvqnh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwtnqhpa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gxjyvaiqn.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gyonxpbue.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxqtrzuc.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gwvkrovte.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaturkbv.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gxznhvsut.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsndnkssg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdubbatfz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdrepyez.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/glhqpcqhv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuflhafs.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gpsabgavq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcuzussq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gdkvvzvcg.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gxojqtiha.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/ggjcvswhw.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/greqfnwvw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkniakyj.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/ghpprltgn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/glxmaumyf.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gaypgwqzg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvglqxtc.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfirwcry.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gnztqlmlc.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhfksiar.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gridjpvox.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/guhhlkspx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gxxkofwwg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbryjrnfu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpslxgab.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gupmuhlzt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghoawehdp.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwlrcpdy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpozktxs.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/ghdunxzwy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsrbtitp.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/ghhchdpme.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gpoysjyby.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzikcmes.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvotddcu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghslsdyog.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvdjgweb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gxdwebyvm.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfszrkjjh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoljygyi.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnfqxjja.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gmtpipvmt.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/ggtolqxda.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgdaybfk.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gxxugrmai.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqvgtheg.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgkmqrhd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/grkjzaaly.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlbjeouv.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqawmdall.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkzdrsje.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gliusqran.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/giepkyszj.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/goauhgnoa.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/guritvuik.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmhppxxj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gellqerxk.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/grxgarxzf.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gajfphhyy.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrcslbiv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiaacfma.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmkkjrff.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gfeescunj.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gioqsxiny.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsmqcmai.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwmsewnd.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gfwwexosw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtkxxsey.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzxzscdy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhgvwqmh.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/ggqtagfsz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gloywoyck.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqwrptew.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/grjniuhpz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuzjdevq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdjrbvsrd.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmvsoxvg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmopqaubb.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghafuhcgj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gioeftrfv.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gishfjsft.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkptjfzbe.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gfetmjhlj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpdqdpre.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnekxucfd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gpygbrrfj.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gnaibxnez.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/ghekgbwvk.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbrrxmllo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgpuhqcm.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/geulakpsf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gyjvlhrlq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/genbclwsh.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gewweqhvl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejruxbkr.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gocrpdbxw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkdwchnp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkexlpled.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gvbppirys.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggyyxpbvm.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gioinahwa.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhmnsdlt.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoqbkiii.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gskuomnxz.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gklcdeuvu.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeihdzhz.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoxygmwm.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxerfekt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gxqiedqpf.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gxupvfplu.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkubqeeia.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/glkdckivg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwttzqeni.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guucfrpjv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpapmjyya.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gotvtwzel.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gttevnkuc.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxpnreds.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/glvcxjjri.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gbaramqly.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gtzooshox.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gtailumdb.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfposefc.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiarzxkr.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gbcphnvaz.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gbqbrdixk.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gvlckikrs.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvqpwahsk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gaoddxfpk.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gijjiksrx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyjpuzsp.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgrtgwef.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasazcbyd.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawnuwpez.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpjqevltq.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxvjqfgs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsitcnkx.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gqqkgtfwq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gehbxtjcm.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gnlfnhbxf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvxtrenuy.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpxvnvdl.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdeorrbd.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gmasiktwy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmlmzvblp.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmrfblrbg.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeiyzrst.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/ghtymbbfo.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdekbhse.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpvwltqt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gexwfdqhh.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gfkwnocpx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppyrzdug.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/ggbumykgu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkxzlgkwn.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcuaupybb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/galvnljbz.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpskhqzh.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/grmhbudjp.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gdpbwsbkx.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqzerdhc.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gylhrdplp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkldeskq.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnbonjnn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gktxjqxec.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grwuhphif.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gactkcidb.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gklcbjcpx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcrrwlun.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqfqeqvl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/ghqwvsofh.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzzwbqne.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gbrkugswa.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxezxurt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuctzrhf.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gifusglwz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gyxvtyfgl.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbmcszjx.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpvdpdnd.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvrjjxmj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gyjvhxdoe.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gmpzrgjvh.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gkfauriwv.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoxprfni.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoasuvxk.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgmvnzvx.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqyvxfsa.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/glhvbdyhz.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gehpifjcv.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gudltnube.sHtML


<!-- 参考信息 -->