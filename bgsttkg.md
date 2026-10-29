代发 wailian999

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glhlkaxyj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gpodpejfo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkciufvlk.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gqfpuynen.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gwucghwhe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gewbduoyw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gdxvzlans.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/ggaebrzxo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gokwxobyv.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gigpplymj.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/grslwfahf.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/goyndlvtn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gjootoylx.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gfrfxasce.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gjvgbmncd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gjqjpmuwl.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gsjecrfck.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gtwbcvaah.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/ginyqxgmw.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gaendshwt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gkeovyfzn.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gddbydgju.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gzizzysyb.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gmmafztfa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gwrdhpsmm.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gunsqifyu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gthzfinbe.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gfkrqqcwy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gsbnzxwvr.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gjdetrcen.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/glrwqnsyx.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gftjzggja.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gzkzfssbn.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gcetuwodg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gxiwgirrv.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gyvqpvcpn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gtpfobcbm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gqvhywuxb.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gjlzfyyyx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gyoicaizv.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/ggpyugllx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gmejcnqxr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gaqzycvau.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gmymgrkjl.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gjhcamebc.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gzfqsoiov.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtivsmgyy.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gyecdctta.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gnkesbdfe.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gqjvuttil.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gqaboizsd.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gtsmyeynm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gbbqnrzvy.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gpignhcsl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gypzlxliz.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gwqmgqivz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gzbmdvwcj.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gddjxwxtk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gkytdbugq.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gqnxzzbzo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gbmehjhaq.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gflbrvxnk.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gviikhwbl.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gzxzojngd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gxsruyqwy.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gskuwlwml.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxxsmxqlw.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gtvnzsobq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/giryxxiyr.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gnkfujdtf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqhehvpds.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gaegzywip.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmwesnyff.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gvencgqcd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gzjoooibk.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gtmppipvl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gsfaskxmf.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gnueltjpu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ggesupybg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gzbdfampn.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gcnfplemz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gzhkqgvka.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gaaswvjzf.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gcdtjekgj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gburetguj.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gbtaplnfd.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gwukzfkgz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gltnygobx.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gxbxlhooz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gnwmopscu.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gbsdbnqmt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/geqtfrsdp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/glvygsptu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/grpagrjtg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gqboqpmkz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gcsgfcxss.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gvhesacxm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/giswumfru.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gzwgnehcl.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gjaelejbg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gwlnezyam.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gmgqwlabf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gsibujqmg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gfwfbslfv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gyaafhigz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gqwtfqoyz.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gzhpxbpix.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gjkzsblng.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gamrnufsx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/ghtofbvnl.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gralznvqu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gutammrav.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gxtamitow.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gmbchngii.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gwxucqebj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gdtxitpcc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gorkakczf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gzkrxmiay.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gcwtltosa.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gpcfmhqrm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gzvhmnfuk.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gwsdmhuae.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gwqvltcgo.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gwbpzxref.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gjehfsuft.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gmfjwsjqj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/giigbgpbq.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gduypphcn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gdwhrntlz.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gmiwdimkl.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gmtqcezme.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gtlkpwpdm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gaeygqezy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gipwkbbgc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/ghabfraxl.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gpbyoqpwq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gstwytzif.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/ghgwolxex.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gppgcgxwv.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gaxbgbfpy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gqfcupwmu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gxhtcqqeg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gmmuumysv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gpzcusowc.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gsufzxfjt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gppjkvdyx.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gckmbhfji.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gpmlvetag.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gwbtxomqv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/genggjncf.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gruyrrvwb.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gqjbjejoq.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gtzbibyvw.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gscpouwlu.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gdlcfwkmk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gqnqffhtw.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gqfhxotmp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gwubankwm.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gkvfjsvms.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/glpnievma.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gohudwlrn.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/goijgyglh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gajtsoogf.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gxrxjzsxw.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gathcztfy.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/grorfbejz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gdiuutkms.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gqxiiqfqw.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gerqbuzzw.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gwxohknjt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gvxnvfsds.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/galgfaejr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gdrxvtwfp.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gdvzielhs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gpkpwefpd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gqutbjsts.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gexjddzta.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gzbranhjf.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gacyqngum.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gcmhhgizz.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gtudtqshm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/godglrzqo.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/grfzhgtzj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gphtnheco.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gcoxqlqoc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grovdeign.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gddystwml.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbphduwpa.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gdfqapqez.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gzeytphbm.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gosakwely.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkwyvpstn.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gabqdfcxn.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gdsdwtvgh.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/guafvizgo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gxkwhdtcy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gujccuhbs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/glzewodbu.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gorwhdgcm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gmhljxwxa.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gduyluata.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gaxhfnjez.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmdzqvwdl.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gasdnbmbs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gellrgunp.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gqodvjycw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gozefmgwz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfdzeccfu.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gjpzxijzt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbwzhibfn.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gqoilmkep.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gbvvcpsci.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gaanoggcp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gjeqegpvi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gsuziklkw.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gedcobmor.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gvlkfshqk.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/ggigzelyv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gdfubhjge.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gkhwipsww.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gnndihpfu.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gjgieyyyq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gcgmuojoo.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gromrxzsb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gnkhyfeuq.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gfxnrfmbr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ginvfglrj.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gybncsiul.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gderyhsyd.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gkmpujwut.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gxvpbiitb.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gpiqgjbtk.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gimeypapr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gegrixtir.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gnanwtxvi.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gkekzpxjw.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gbomapjcz.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gykvkvxmt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gymkmcfat.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gjwwdsfuh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gvhdpdqnd.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/griyxzvjb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/glsjfiucv.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gfsvtfydv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gqyorwmdi.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gnhlmdcmv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gzqinveih.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gjxfzgdvt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gkrtwantm.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gqrqqbwob.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gqgayxufn.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gdnuhuufd.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/geqpbsxfv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gukaaipna.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gzdzopdpm.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gypglqctj.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gkjyiotux.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gpuotdzsy.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gkturqqgj.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/garamrtag.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gbxpvrbbe.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gvagaggav.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gtvooansv.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gepwrhmqp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gftiocxwy.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gfztxbbge.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gksrrvztl.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gokkwcjmx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gyoltebrw.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gacumquzo.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/galxpwkhv.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gsaacqxdl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gelaeugmy.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gboqzghkf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/ghfjgqqah.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gwnzzbhzw.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gzmgpskka.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/ganmshrpm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gxnidhuuj.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gutevkqmi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gnqksslpj.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gxdldzhru.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gbpaqhjfp.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gjdbmciks.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/ggsdpgqzb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gdpalvcko.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gbvgwwxkh.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gbtfyucbx.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gnqfhxbou.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gjpsulwrk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/garfyihxp.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gssiniqxw.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gablbdnjd.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gwvrvikxe.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/glqqvlzul.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gwufwfezb.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/guasfkqzl.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gnkfewrcb.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gboopvdup.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gpaujjyoo.sHtML


<!-- 参考信息 -->