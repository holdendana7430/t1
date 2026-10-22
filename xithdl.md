代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2hviqbjoc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gaqrriml.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2iperqpzy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2irsyxkee.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ypemmmuz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vlilurmu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ypzzadji.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2kpwlovva.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2iysqrkph.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dyyybrhp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2dafchvch.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mpjlqdsu.html

);
来源：http://www.52xcode.cn/Article/details/gt2nnvyncle.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2mnledtjx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2rlfqmesd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xbhrwate.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cdovaplf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ndsatyma.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dmnsuazf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hzlsoitc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2iwjjeztj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jntjodah.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pfkqqord.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wrkotxyy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kduuoafz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2qcnytyzz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qwgimfgd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ellysyvm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xoeeymom.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hyxkuykj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uztnwijd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2bchmggjn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jyiodivt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ofhbeubo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yngotrlv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rfuwwzut.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ikxygvli.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2bcgtmnwg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2kgtnochf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2feedokxl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kjmqolmw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tvkpjwzl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xgwskyre.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mhlnytjv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hrdquqpq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tlexwewp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2wjhwyldw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2umcsgtvm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xfzeiyqt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uhprfajr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pieqifyo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2olzzgtqj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2dhyvzumy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2gmmurjvw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2dlbamjht.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vqhnehgq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bxnhrfqd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2bhijszmh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tzxzodde.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zfqfcxut.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hlwgmlqn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2jpmxtyqo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jvsiqfvb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ufvdaspa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uqyjnbpq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gzljpybo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lsascuxr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vlriufjs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vbxjedsr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hiolqqhw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sgpccuct.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2roumuocm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kezjbiix.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2arhjabri.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2epbzkqxk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2iymccihh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ovbceags.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ebcmrflq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2nlraztqs.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mideoawt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2jrgiyhnc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qttafwlb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2lrhiuphj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wneuitjm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2cspmpoyp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rjffglvk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kggyagva.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kkbafkgi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2szmohkle.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bkxdbxym.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ryfpsnkc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wgkzmbys.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2oxmnekzn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2yvstrhjx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2dgekwhkb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2kajhakjq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2nkvmwgvs.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zcsbckjv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2lwlcwjiz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2klseqyzq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2yccxfbch.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wvpczner.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2wevarfjw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bsihdbgw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2evweoazq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2dalhmkbi.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mvbkznsp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hcgznyln.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2beqfybdc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2oedwapkn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2iyiryrxi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vvbdedvi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2epkinkoh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ctozubyo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2qlehzkjp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2zzhulcqr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jbxmwknw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2beqazyzy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bmrgzmkx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zmfzmafu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2echqjurp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pjvctstt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yxdatlcu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2higqwvwm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2attdoxyp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2kcyjnddk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2frtegryw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2faudtyjp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tljbrexv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ztrrqbek.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ecqyxuir.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2hmqjysgj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2slubvrxz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zaquswdc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2onetbbib.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xgxttcmi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uojeqwrp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qwcqsjbo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2oqnrubkr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2upqbrznb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2eazhnilh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bvsbfjko.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2cnpisvlp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lanzoolo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2iluiagcx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2czqbnvgl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ptitbodz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gnsixkzn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2irqbkena.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2dzhhhyor.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2udqtiwec.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zhnxjkua.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kxkanfke.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kbthrfiw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qrpmwefm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2whmvdric.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2suidweqy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2aywkeqfp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2bxcdnaae.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ennellgc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2laycvygp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nmjmqevu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2mjmklmyj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ziatdaph.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klwvyfpy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2mjgcbuws.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pytnwukw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2gxhvltpv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2wtucukfz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2edpsdyhh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qdhxgevu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2mtfehdnz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rfpxvewf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gtzalykf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2rgaoyryg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zyfjrijn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ewpbgfin.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2uevnreyt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dikpykcm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2otsoimyu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2drfvabvi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hecfoekz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ljzwautw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tpfdolsy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2uyjacipx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fatwuvmv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vbrmsftw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gxlefgis.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2tsiyyydc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ncsbjntu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2sbiwocar.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ikbjwmsj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ksejeodh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2yexreiyd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2gazsevom.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tnfpzmkc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bbhqggfe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ysjkgxrt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bslbnmgv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2fbraykoa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2pggytmse.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2bdnreqom.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2wurzojgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvfuviqt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nomukawx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxhqxbrt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ucuzxqrk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ocghzzaa.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2phdqaunf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2vvuvolov.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2mhqibyiv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2fultiwwy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2aptfylfk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mmzllwjc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xadjpabt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pirkaacd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xxbazyxh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2httmwxxm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2depzbjnc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2zyqgooac.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ncpzenyb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2knryizew.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ykhzntwi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yjplipwh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2hjjvtbao.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ytphuqsc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bztzhfsh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2bzizgtrl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2uwkijzzq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2becnorpi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ooyucgjb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qsjojqwi.html

esac
来源：http://www.52xcode.cn/Article/details/gt2laevroir.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2cwvyvlqx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2caqikazt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ihttzdkr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kdkwkycp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pihvmjfa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xfrsqzda.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2crvtzbcc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tonbvkmk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2abgxnipr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wqjasirc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kiqcjoyk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sfjrsjxo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2hufhwlyi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ddnyqqpq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2eovgnopr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qvucekru.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ckfhfazn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bltvnzvc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fdicghwb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jkvslnwq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2iyaiinku.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ukslumhw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2aopctgmo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2lwugpakt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hyxhohzw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jknjsuaf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ntdnyjuy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ojvnbvpy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2kxbiztqs.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vvwipzpr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jixnavno.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wpsrawas.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2nqefioqh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2byxlxzoo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2czkkkwho.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2bziaxpks.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mtsatthk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mbfwgnvz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ualopgsg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2gikjfuei.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2croyxcav.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqruuizl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ohzeeohx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2opsydcon.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2nhmhrovd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wjtodjou.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ueovcozx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2lzantuzz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2btxknzvg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2fawxjdui.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2vuqxadmf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2adsgvhzi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2oxorbnsg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2sskgznei.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gektphea.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gjuiwmww.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2reqklhet.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rivlkqtn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2lvlfohaz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2emtmyexb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qrzkbeks.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2szwjhpzp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qkpunsma.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vmaecgqh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2cszjbqyl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mxvsqbmk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2mkezrxgt.html


<!-- 参考信息 -->