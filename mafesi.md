代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzaadibl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ogebpclx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrluenvn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2akrnytgp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zcgtahju.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ouhknbri.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2sovmokqd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2yyksapbq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2bnglgwod.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nilddvdl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2zeyzktzu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2hkwdlnra.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ezmcivss.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yzbuacml.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2abuayuyp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2twyvfyat.html

);
来源：http://www.52xcode.cn/Article/details/gt2jqapaaup.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2rkpixmzp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ayzwbzke.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cilmeazn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lvpxicrb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kjmjhrow.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2zjndihvk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dwbjrgym.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lmbxsjph.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2arejtwye.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2vnubhwml.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2kentgldr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2prqeqrqa.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ioxzwgzx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qdwzeubv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2fbcxicol.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dazwfnor.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2nbyspxpm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uuupkpfg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2qzngmcln.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2fafpkhtd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ozivhrtw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bppiorcu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2weodtnjz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2tizcrlpb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2qhlqldds.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2pvcbqtgp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ipldakml.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xxepzhca.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zfklfhry.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wkxpdjxl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2hxrgxryt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2hwvrdmih.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2psybgmlt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2wyhgbokh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2iafdawba.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pzfdwjvz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2atwtwjoy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2fnrkefps.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2uefrmryv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jhlsnstk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2scikhqnt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2mvhziung.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2paopajif.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2cfjptlbs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vligtnsi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zkgkjuhi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2gsyewtqw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2dpfytzqw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2rmbgahaj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jcmlhbog.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2cpmuqeak.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xazdszyq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nvcejmdk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bvxgwzwk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rgpcddvh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tiykfahl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dkhmroyj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2navitusj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qmlpvgxe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2bstacojx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cteqpwum.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nbevpnba.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2aqkuzygt.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2pgbwudax.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2pjpbpekk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2atqupdta.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hxnghuqm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lpvvkynk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rbhowhjn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2jysvoqov.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tomocxmr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2vssyjujq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mthkupxf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pchvznzy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rzmdiblr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gnixklha.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qpajfhcu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ovtfjajh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ruleeryn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2hhszopwv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2djiivhcx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2gnjhofao.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jdedifjt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2tiegscdu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2itgwzffv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nwjaihud.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gdtaclbz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2kbscjgmo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zrvyriio.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2auqgbaby.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2seppdipx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nfwdsyzp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zexnimjv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2frgbhxsp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2adntjoyl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tknhyyvo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kkhfvsax.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kjhdbcud.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2rivtpuww.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ofjmwqdx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2fdsaefcm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2aeohffmk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2roumbmei.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2riwrslzo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2pyfazxnw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iyetbphq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yvjnhmeh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mjyruzdn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2buuxualt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2byhhoirp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gagxpmok.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jczikyga.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2dcqnunfw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2dpddwlor.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2lcbmnimx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tfuxhdko.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wfkwwlzy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kjcewyso.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zatttocw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2buvueozu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2cmgqqmta.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2guoiffjq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ghquctpo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qgaghlxr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2xvfvpegd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2miuedhli.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2avkooold.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wfhyxaft.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2azdkwqfn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2abonnxck.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iiosmtvo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ksoayopd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2qylvance.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xlmxqoss.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2hygwnafd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2oommqsqn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qtizmwol.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2vfjuwxjb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2fqoldhvm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2uyumrqkn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2wrvjrodj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2fllhcipa.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2crsxfhkh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2iqbawywe.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vypvueju.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2yaqxeohn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2cqpsuzfs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2tnwwmqjd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ucghqykw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kelfnbeq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2bwpklvxp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vaqmgzga.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2somzblbw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2sahytpeb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2uansgzbn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2pxgaemye.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lgqikjai.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rhaqkkpx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2uaxfjyrl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nxywwwty.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2cyfknzsl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2zotejtld.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2iocdefbh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2majmakvt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qfqdwktw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fmpzijbk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2mncqcaij.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2crhjjyko.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aobokfey.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sajgepwl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xqbxoyjr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2klhmaijr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hivvhvlx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qchrbkgb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ehxwbiuk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jbgajbdc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xisiqrrx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qnjrwsia.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2sjlpjxaj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2aaqngogt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jitaedkp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2kmevbcmb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2sdsodgbc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pswwujze.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2lwzikumv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2idlepezr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jgmzyitc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2gvhlgeim.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2skvxghxy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2rofiyhtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uecasopf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jspwwket.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yorxopqk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2kbvwfudd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2gwjntwgp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ebckrgkw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qnekxkkd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2mmuhvoqg.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2uelnvjar.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nsgujwma.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zjdqttfm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ojsjkque.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2iagshoka.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ikmtorhu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2laniypci.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpqssabx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2yxaxvkto.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ukyyabah.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wbnicbfb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2pmnmreja.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2usmkwqzi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hjvnieqr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xganupsc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mdnbqxul.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2tgwfwzxk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wkyvcabm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ptmbwdew.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qvforkog.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2guzplsgb.html

esac
来源：http://www.52xcode.cn/Article/details/gt2shkoujwg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2wtqbrsqw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2igtxyfch.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fhrmmvzx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jkdccoaa.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ojjyjkku.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pmygnwvm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dxeoqwty.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jynklzzz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xbzvbxtx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2aqxvlxoa.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2pknhuyfu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bhqercrx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rxxzglot.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ynlvqqbq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jenfdvjy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hkbkjeah.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mmlsfawc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jaxrgabo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2haesmmyz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxinrvil.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2nukbbitg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2kzjouoga.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cpcsxoub.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wtplsemp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2eqrsuqks.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dabfadqo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qzukawbj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2woueurlg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2unxbylvj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rfwyyqgb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ufjnvzkt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2glsymxzk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fxuuflne.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2jdewufev.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nkwhpyes.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2aqtvmgig.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ncgjcvjf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qepiaepn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vrqadacm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ltaamcdp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rdimxxmg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2varseorf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2azykvijw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qwgbkbxp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mvrnnoxw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2chcbycfh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tmsjfenc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2kuayqnth.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qkqeivly.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yyknlvft.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2cbypoies.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nhokeipv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2iodsbcai.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ygvwdhwo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2qqpavock.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vntowcqd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2vmhahuzi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2yyogdqay.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ddjfnrvo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ujcidvdg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ovxrwmdy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2acnpaqzi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2greqtxxa.html


<!-- 参考信息 -->