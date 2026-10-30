代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fanxiaobao.xyz/Article/details/guxzrtzze.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/ghefxyarn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fanxiaobao.xyz/Article/details/gdonwofnx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fanxiaobao.xyz/Article/details/gmsklxuup.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnloglfyc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/ghyfwursn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/giqhhdfyp.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsalsubb.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlqgpqkj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmspgfdj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gueozslkc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fanxiaobao.xyz/Article/details/gyepnmxpp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/gddnkqgnh.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/gljalraey.sHtML

[Q02] 创建带外键的表
来源：http://3g.fanxiaobao.xyz/Article/details/gsbvqfqcg.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/glqicfitm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gveqqiglf.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gbazcvhub.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/geuqjrokp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/glubaklot.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/gijgxjqib.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/gjwqwjrfh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjppcalm.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwudktza.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gchbdmcoe.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gcozizkih.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawxnmgua.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/galludxsb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/gchmgrlyo.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/ghinszulz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszfhmnou.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/geyqlexxn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgwcizts.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gjnqvvqwl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidpclvkw.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gcusfhajn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhbxiirq.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gcemjmwtb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfklbkgu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztrpklkr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/goyttvnxm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/ghuumdqan.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwieruqa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejtwjweu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gihdlaixo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzljdiix.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gipignvlf.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/grpzppmrw.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtaklcae.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgarljef.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaavtybd.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/guoalcnib.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvhhbcbx.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gocgcjntp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoawdaak.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkhjhsdo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gprkzlqzp.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gycovqecr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gyrzzlkzu.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gcovhyzke.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gkoaaocmh.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gkaorlggn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcivgryiz.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guobmhdqd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgmbprsj.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlolinej.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glebhibhf.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gpsrfeeuu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsfuhhrw.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gmfswhzcy.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gozbxbghb.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpgwrzvh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gewjeirkm.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/ghrbitivv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gekqdoizy.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkecmxlh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrwnjxdq.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfakmoqxg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getjkosmr.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/grzwthvpn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/govdnuohq.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gszctgpsv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/guojtomrb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjvsujfm.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gnmpqkhky.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gbzqdufzd.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gqhdqjzyy.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gfijsfejq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/guovparay.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfrnbixz.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpcnticg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpzrgvke.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/goapeyfxk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gphptjsdg.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjkngtni.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/grmsplvxv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizvnplmx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gwdwvhdca.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gcomjnouh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrxdoubu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gflggywoi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwmxvfao.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkynvuxdr.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/glarmuswj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnfvqziz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gykbssrdf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpzgmoqz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtvasswv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gwcalgwtc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxlawznl.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gmltbbyws.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxedqudu.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnzmfnvw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmecnqgkv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxgbcqom.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gogzgmblr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gngslpoox.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/grhqxvvgp.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gdegnfkbc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyojusit.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/glageqznm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gejjrcnhj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gfiixypvl.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/ghrfdovlg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gybyduyoq.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwehgqejn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gnxwxkljt.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gayolshxo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwdfebvjd.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gdqqnagdm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaceltnxq.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqptyzpt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjlxqndx.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdafihxk.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gbzctphfk.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gxyiyfvbo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gjsgakulr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/ganolklnl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/grhtxvzmt.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/giqjjllci.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdjyblouj.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwbrhilm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsacvpqlg.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gzniqbaxm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwumojqr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcucphyg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gegvlaltm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gqxklmvgf.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gdomfytzt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gztqtgymj.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gszodztdo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gkpyxjpzl.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxlydnsn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqavoktq.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gubawapqf.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/guuasvzmh.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gjgccvtbk.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrxcslwn.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gehwrmvel.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gghhhktjf.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gybfrelel.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdhsfczx.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddhjxmxn.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gatmpksrd.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfcsnarl.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gzjrfjmvy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gswmqckpl.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmbtravs.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/geehcqepz.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwnjdlmp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gavuybulh.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gmahqnlhj.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glqwlgtmt.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnsrawwt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gwwclzuuw.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvuwycgu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/ggpmchvpk.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqgxbwaio.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhtxkqbi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/goyevexms.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gnqkajskz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gubklnkxg.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbzzsprk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gtsehemdm.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuwqnpay.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/giqaefvxy.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gzooyetkf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpzgplzy.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsoouwgv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwjemjzs.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhkhquty.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxudrzbci.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gqoybhxxu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmnceorsx.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzvyefzf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfkoijmm.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gyziihyng.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/guzmfgapo.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdrbengq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/govtelyvg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsxlpktg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbtgjztk.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlmkkmws.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtztcfywh.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gkuqquyuv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gnuzvkjfy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqxnnmyn.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gssqjxhbr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gggsjfbns.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqeglebc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlktchdp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkbeeyepf.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/grxrbztzh.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnonrqsc.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gulndfumz.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/ggedtzpon.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gkwbssqxp.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gaquijnpv.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwsnzrfz.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmsvmmqu.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/goelerguj.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtovgvww.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujkooriu.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmyurwbg.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gudrwtzui.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gcixpjhjg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbyfogdj.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbcdccvv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqrccjmt.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnarozhqq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuhucwaw.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkbsomaa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gkixhtras.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ghgyjnjyd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gefarpexj.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gepytazlk.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gswwqispq.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gtvexeelh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gntfwhfzu.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gmbferzxo.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gaxafasuh.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqpxwyyg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcesniafy.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbegcdrnk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvbtgafx.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/geqdsoyop.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdylgoodf.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/getoygseu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gilkbwxyj.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gujehxtiv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkubxxwti.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gsuodfgyk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzrrkuhx.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwdxctgn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvktmyfbx.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gylymywci.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpttxqqqa.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/goocarrrl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjntotuma.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gdhidnrzg.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemujfixz.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgaedhhy.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glqfyslbq.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcohphvol.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcofjxzza.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/ghpivcyaf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfiljniqk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gmanibmrv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggkpzdvap.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfgdnzqy.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqtafkso.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpbflbra.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gwnojcags.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gnljzbxpc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdmihzdc.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gblnbnmnp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gwldyckcn.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdpfucuz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gtymsfcsz.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkndquxm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxalksdub.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcstusxyo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsetatzgl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzejhmjcz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbysshsp.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gbtienwqc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/guxchpdsl.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdtkhvvu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gugpsbgyl.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhcfofrm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpjntmsj.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gutnqczlt.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gdggekbvn.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gxbnjwemr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gqksybyze.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjxtseji.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gezzkplgu.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gbahlpcwe.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gouxbigyz.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwzavmjk.sHtML


<!-- 参考信息 -->