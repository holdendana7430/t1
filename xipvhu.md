代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3keqrvtmo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3blwhcvvm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3msdrefme.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3khathpfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfpppqro.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3rbjnnsev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdsdrmoh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3qfusjvhi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ndmbeqsq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3iwhdrswr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ojibbrgh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hihdjlrq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bcxkkaem.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nxdafzwa.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qocbbuve.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3errodwyw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ckkfcsdn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ddklxixt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3laqtvfpv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fvkgryiv.html

);
来源：http://www.52xcode.cn/Article/details/gt3rousslwr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3fetaatqr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3wzkybljx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3sllwajdz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3upmopukj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rfckmasg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3aomxrrov.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ovfbaczz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3vmcqhlxj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3rigrchbh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3uhyailkg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vqweohta.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xxsnmgix.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vcbmzprf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zwfmaola.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3jhccvvsp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ahcrtccl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3hxinjeua.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bbgpffcq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vkxjnfhm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3rxvogfby.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3dewjmsbx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ivfrgyqi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ehujudyz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qyesvajo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3pzzqshlo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3lrjudkub.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nxsbrkjl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3juxglctf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3eybercvw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hnwjoehy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ikhbkjpc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ahffzmdg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eqorqpzo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3zrmaugzg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ryjqfjae.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zztdkwca.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3iqdbcvxe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3yrhsrybn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3anxzemyq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zgucqdvf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ofuwxcqv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3hpkfctih.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3tndlxxtd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3sfymrmzt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lpiyexcm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfqfvywl.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rmhshfta.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3uxrsbfuy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3jtgozlii.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wloxlhew.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ddshdcic.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ehlwaggk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3nncyqkjh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cdzvgcie.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3uynsnbtp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lwvdyvip.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3rvqyzzsy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zopzobra.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3nllcjzpo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3erswobke.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vgtnpsnc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cfnrhdcu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tfmjisdc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3kuwmetxk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3twtvtedw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3zvoykzuy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3uyryndcd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bxyjszpb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qlmlyvog.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3fcybclix.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rgzpslkp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3fwsvrklj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rbgggisb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fagndjdi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3chacccxt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mfdomuyd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vihjvgbx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3xrxgqrvw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mebcekaz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wyafiojq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3vpplwtge.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3akgnubmb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fjaiwpct.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3nlgtsetq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3dmynhlhi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hrvvhytr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3aapaqdyc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3tainqqtl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tbissxrw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wvgbveme.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3peozhdbx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xwcyvhsg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zibxbtpi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3evjazhzs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kzbnexkh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3duvdtkdt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3icngyvap.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3benffmfo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3abjyzzpv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qwfeiskn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ejhacgnz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mkulmkvx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yulssptv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3glptnxwb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3vruchrvh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wkdofmsa.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3rfgudvgc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3jrbwjfas.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3gjichcuy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3euksmwrs.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3qibzmjny.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zbrccdju.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wqbtritb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3jxyvphyk.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vltbzpce.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ywddlzgj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3drizkouf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qjugbmkt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3nquunypx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fpwlgyml.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3keflrpcp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rjgyergw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jfluugcb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nrsroslf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kigxfweh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3retnwdbb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3acpyunkr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3wrgehtnj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gtaefmlg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3whqkkkem.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qkeummbr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hbqkjkkf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3mymtebil.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ypapppqs.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ynnsroub.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3netmsoxq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xbptmhcc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3iihmqbyg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3nxtluqca.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3buanyhyl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3tjsjysll.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3byjcgcbo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hewznoqf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qezongez.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ikxrydkn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ydaofuds.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3wdntfteh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ozbqtidl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3yfhspmrg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gdksvbrs.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zzgccnpx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ctaumnpw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3okqfqcee.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lazqbtmx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xndfnhfr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hmmotitq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xmyrpcuf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ddaqitpr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3kmshpxkh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3jawzmehy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3dkkchplp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3vimoopqk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ctpjufse.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gkcddeeh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3nlqptzqn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jltqvhol.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wwvcvzsw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zjyuapze.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ybxweyoq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vbviamxp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fbsccstq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3psjpqmjl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dlexkfna.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pcusmqwg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gzfgvkjf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wxyzirbg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eystrjsy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3kbxeernk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zpymivkd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ahabynzc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3qyhrhcwm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3boyhercn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fpwcwxhl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3czsoefyg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mszzfafp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dcsfcdxk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kvscwazf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ckdadoub.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3klikhwun.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3yuwztdhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twvivhqf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hturrusc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jzbzgcpe.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3pxsggonm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rgqynmpu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3iddckaot.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nitpqikk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3idbhnibz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3sjavhtts.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ydlmhvss.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3nozlbnuk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3tkfbsxxo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mnlvkqxv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3rfbnrtvo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bsiltheq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tipkpavk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zbdmtshi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3wfdzrwyy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zeiscymr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zbsrpqwv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3anvmgfbt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yvfczcoo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3anpimcop.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jlezrqnf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3mdiyqlly.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3lopobvho.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ogrdjugp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3hpkfaxht.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3obfotfzo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3tuhbqddx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3nnwkhlzj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3smxpmpnj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wwazgmxk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3okqwbayb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3pqbptlvp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3irhsmjbi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rwjhpsil.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eivvagvq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3imztmwnw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pxlylpld.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mxlahpfl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ilpuiklf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qlebhktx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3kzsnafhe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3urufltta.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mkkgxhpu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3yycnkspj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ovyfxicl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qdxwwjpq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3xnmnkpgp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rbbndxnc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fnviiiem.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lcpicitm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3acpdzquz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fsavbogk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xckzzjsa.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3pinjzjyf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3umhcrtxq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3wqgmesjl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ubxmkmlu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3olcbkhhg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ngmijmxe.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3spjehsyp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3flihoubm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mewmjpep.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3inhkjbuy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jkxnoovc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ficecbib.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vcjdnilw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdnylrhe.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3yetupawa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3omynaqni.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3eaiskwjh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3iqacmstb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3buzmctbi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nowtcrul.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vhncgyrn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3etmvbqaz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ihcywmsm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vnjveyqc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ojzjvrtd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zphvdvhd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ttzfrgma.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3pbllmymw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xerwwkni.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3iqqxnhlc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3fnqmlfyj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3drlenddw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fauuvzql.html


<!-- 参考信息 -->