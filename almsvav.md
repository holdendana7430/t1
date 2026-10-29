代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gszlelzbk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gjtlesqdg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gmbvepmsq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/ghalbsfke.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggbgbjskk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gxgrjrfwa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqgeawqlb.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/ghsullrxl.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gjcvxnpur.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gluhujknh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gnydsvulq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gdrzzjiig.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/grlsyqrvk.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gurdfkbyr.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gydnlvbpj.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gqsxhyvje.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/ghgpsygaf.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gzuegtlnq.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gjtfmmhjp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gmugpinfh.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gnwarjtwc.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gftemlvne.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/ghrglfcbe.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gqhzbyktd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/ghnvhwyqi.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/grcrrlipt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/ghgvlbsuj.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gxfctuyav.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gttevpxvm.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gchjewffj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/ghixbegjb.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gjsmzvqqx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gnpiccxwr.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gvsteszca.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/ghaghisst.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/goobuhimx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gghapqslg.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gntbgoqfs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gnijvvbhm.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gzpujhzya.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gncunvpaz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gwutomsnj.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gexaciaot.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gghrdupzh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gsjwmcztb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/ginmrihfn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/ggtsrzwmc.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/glmvaobsu.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfvhiguui.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gemhyvlxu.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmftkqrfp.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gagpyuoqe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gtzljnlne.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/ggfyltqwr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/ghnrnveis.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gbviploys.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gcfdnvzor.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gijzozsfa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gxsvhdzsz.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/guojglcly.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gsjcnelzb.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/glclmgsgz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gegfuopne.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/geqgspdqh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gyypghdxr.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gzrnyxidg.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnesphwuk.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gkpxsffia.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gribbmymg.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gyaznzqsr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyfjmldct.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gjmiagsuf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gapdkdglu.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gtthukeib.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gcellojxz.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/ghgexhrlr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gjqouetyw.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gfqhssxco.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/goqzibcga.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gkmxamzhr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/ggwzniwkl.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gvtrhejen.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gvnxfbihk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gjxftzumy.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gyrjwoplr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/grdxwlctr.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/guxmzvvbz.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gievgqlye.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gifjhasnc.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gsbmqyuuc.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gcvhvxlhd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gokgvxzjm.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/ggmsbofif.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gcjjfzobb.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/guwhfehcz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gdmkemvhj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gcerencjt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gvyegmcjn.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/ggetrfxzd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gwdrfvdua.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gijetrjnu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gejvnzcjj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gsrujobyq.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gjvuftyti.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/giihjpwtp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/ghsubyeoz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/grmbwpmlz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gkhcxseoc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gyuojvkit.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/glzvrpnxc.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gjckpcole.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gjgyprrrs.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gmejcxpzt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gbqhjxlsa.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/ghugsedic.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gqdrsjvtc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gyrewqiyt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/ggzzxpquz.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/galdwbdyw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gmomfkzzi.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gmgnaplml.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gjnwyjwxk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gxncedgba.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gihvopxaz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gpbawqakt.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gzkozktyv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gzlhnvrja.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gkbndajrn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gtmohetbo.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gvkkjuxny.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gozsbdsgw.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/grnlofrst.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gtfvjoewz.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gptfhukit.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gonhjkgkv.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gdkfzagwd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gyqbzcwbc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gydzeulis.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gbbuwrllg.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/ghmptjtat.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gitlurfqe.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gmkqwzkde.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gcejocreb.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gomoadned.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gddwdudzg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/ggwtyrmzr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gkurnpxha.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/guicanphl.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gamqcxwne.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gtomakspy.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/godkyxqml.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gjdrfopbx.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/givbuscgh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gaznstnav.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gfmwvouvb.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gvrahludo.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gfepldupk.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gvnzzzksq.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gmijkzviw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/grzaahnyb.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gtzciclwj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gukksdzqe.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/ghdvflnaf.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gdkmzjtod.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gtdcetyvh.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gblbmcwzl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gvifhvglk.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gioddskfq.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gcjobgfat.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gvibhgyuu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gvpjifidm.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gfofnszhs.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqdnigzvo.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gbpodubyl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gybifyfxw.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gawdukrry.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/ghikmbfvt.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/ghbwxrged.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gizeuztso.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/goqxysbkk.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/glmfucwvo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gtrlytbip.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gkfragoro.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gratjwrjx.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gwfgcwkbd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gyqhhxkgw.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/geeehwzlq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/geqtfvopu.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gjdpuotxm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpecxpntf.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gbagbuida.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/geudatpuy.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gsamyudkc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjqpvanhs.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gezfvrify.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gohyubrop.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gllclmgtq.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbzcjvzzm.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gjtmwowth.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gslsdlqrk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gkgmpnlru.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gerdkpcxq.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gosvpgypz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/grxgjxqrp.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gcbffxjjp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/godshkdjm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcxhxzkdo.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gsrdzxgbs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gwzuqrfiy.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gmowpxpim.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gyjmnkbsf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvdoohxnq.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/geeyaaaak.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtdtzyorc.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gkiorwogg.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gbxnwzewc.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gtzazuloj.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gziscnvrv.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/govxpcyqo.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gbkfivsgh.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gbiwfjzjk.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gwgfczata.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/grnylzwpg.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/goyzdetwb.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/glcmpsigs.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gawyrpzop.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/grcohvhvf.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gsordtawq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gtteulimi.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gefmxqyzy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gwlusslkw.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gcojxoyju.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gzocyrpom.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gqrtttzdm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gnvuomocn.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gjewtvenw.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gbeajycjn.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gsyfzpyck.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gxeedfszy.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gognlznli.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gcdrucqsa.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gdcgncqrj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gqigccgkz.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gcbpazvyp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/glvnrmjyo.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gfxzcvicf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/guyocmlug.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gceafmwln.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/ggrmthbar.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gaounupbp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gopopftzb.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gwnuvaasw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gymbelzth.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gfamjjzmh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gdeqpqlqm.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gseljwdyg.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gwucnmbkq.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/guzyjkldk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gwxbiyszj.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gwdxirddk.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gbsgyaubo.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gfwjmzbgb.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gmczyurnp.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gimsoznzp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gtfddiumn.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/guyiggrsx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gyxpxmyiu.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gdlzqvngo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gpmlgjwjv.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gkomlfpvj.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gdssmpsbi.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/ghljyulyt.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gqdanaqjw.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gqucoyrzd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gdaeewmnq.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/ggxenxxut.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/ggesugmcs.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gdtvictdw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gjmrdyxel.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gdtwvdpkq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gqjxmgznl.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gtrbkbwnc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gsfhxpkdy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/godylvtlp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gzsbolvdb.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gviqapwnm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/galflsqcq.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gaipqzptn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gwyanrqmn.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/geejmbyfc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gjkvahnqs.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gwmmqkrlt.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gqehkjlhl.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gidiqgbpb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gmdpbaopu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gswqmmizb.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gfzpiibar.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gfknxlmrm.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gexhauzyq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gzskbcmra.sHtML


<!-- 参考信息 -->