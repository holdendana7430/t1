代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pqokjcms.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2izonwjch.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2grldsiqo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pjpcppso.html

);
来源：http://www.52xcode.cn/Article/details/gt2pegmvqfe.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2penziyph.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jodgvojm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ywucytjz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wayphmtj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2dqyvnxgd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2yalfugui.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ukxcamzu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2jlpxjvgm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tzwharth.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nwfndhvn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xvcrdjzn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zfoietwq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uxdwigmi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gixgbfmy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uwpujvpw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ufslbkdz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2nvhwbihz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uhgypsfg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2yurstweq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2bkdofyuv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mcbeycti.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ygzydhfr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qweeszed.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2okuvknjh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2gfpmyydl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2xqjvlrel.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qpwawmfq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ndqaouve.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2snqwgojk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jdrrapwx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2eqttojyn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ifnnynoc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tmnrelwv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2foqqieps.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2avmdohyl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2izfayliy.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2pkspruqa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gtyuerni.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2dugfdxho.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2phankjxt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2teuwzlto.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2cysucdmk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2majbaowd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2htjuphif.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pdisxjbd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2adxkrpmy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2gmfpcxaw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2veiykreo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xfudttqv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cegxopvg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rrzsqwtr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2btwhzcnf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2usebnhit.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ffmvzjtx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yxhzbvdq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pyswloin.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2hrorzzsx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cmgskikg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2iewxtznw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hziwdbam.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wcxkrlzd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qkgenheg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2occbnwvf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2utrbwkml.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ibgcobqc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jovqnouv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2jjuxqnww.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rivdtrcu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ogurkeuq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2cgaztooj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zjanyqsc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2kbipqfhh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pmrbgvsn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2lsflsuub.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hnikultb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2pygrobri.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nfxawefd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2sdizhrhm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2tkdjkppt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2toeparni.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2axphuimv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2irgcoslw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2pgipebkh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2kmknwpdu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ehbcdopi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aemhquzd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vujmcnwn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2afcntjce.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2scjuwxdq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ssixxoyp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wobfaikg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2udtdaifj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2exegqebg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rezdzivq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2odeghdbu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kdbkpkxz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vnsbubou.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kuayfxxu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xphadurk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2itleqeqt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2tdysxapi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wpiiwvxg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2xcslgzxc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rplaauka.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2auuumgym.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bhdlxbla.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yrkyngtz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2fifwmbci.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2gnrhcrxg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gulrzfyn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2bsdxanaz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iyvgivxj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fsqbpdmr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mwyxohar.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2oywlykda.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fqynalla.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2qlhfkpgw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2pexhyjrb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ikrkufil.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zvrnukfc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2tfuzdhbc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tqtfvbpa.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2fsktbbpc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vkylxqiy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2oauydbux.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2dzbeicuk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ueomvprq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2dygdzowm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uwitcdsv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fzzxkemc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kqykedyc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2argbpmgc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hoojsdsr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2oupxpwsq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2kejrmnul.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2djaobfkm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2nuhlphsm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bjuwwcwz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ruaviyqe.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2umjoonra.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pqygbsle.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2eiqporyb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2yekqfxrw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mohnlbwh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2wbhtkkgp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2cxxjaaby.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ahjhptis.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xpgisxpc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2kjcwhpgh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2zdofgzni.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2dyjfyzxj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mwajiahb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ipnklrfv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ngpjpcxv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2mreoaahk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ofrpsrlm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kkzjllvn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fjnvqllw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hmibseqf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fmtyfirr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2moswypov.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2eahznveb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gzxtckse.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2gawvnadt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2prvnummm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yqwtcofb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2urksnomm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2pnfnbfjr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lfnbxmwk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ojfsfhll.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2heezvjkw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ggpktogd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rlagkcnb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kvinhiqk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zejuusgs.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2adgezmkm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kbfvjeup.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2yyazorxz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2bovymhzj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ovtsfzpn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ytqtfpus.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2uetltkwt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2fzrfdmew.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2udrhipmm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qhgjcxfw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klzevhbp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2czviuomy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2daofmxpa.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lzuepedb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ppfljtvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbityonf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qewqvvgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrvwtlpx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2dnssopaz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2gbqnruuj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2nirjmqbu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2fjnlbvyf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2kkfjavik.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2exivggvk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2kmjgxpjo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2wfrdcypa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xdxprcau.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zsgvvtgl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vxavykss.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gslkmzke.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptnzitff.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lrwppzlw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jeqnstpz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rdgahohq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xoyqjlbd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yvnedrfu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fodhpvaa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cqkdqvio.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ixvcldjv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fbubtvwl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2dhpgccmn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bedgkwqf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sjoxnlxp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2devbehti.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zzkqpgnq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ttfcykpb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2hknmvais.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qshpvsrc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wlvfrnip.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nworfsqz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gmjsjzez.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fllyfcwo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2gawvwpnr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xedgbfpl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2coiclkqs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2drvavwrs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2sbtfgite.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fsgurmur.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sevkmgyq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2eemxudwc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fyfwltgg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rlamkexd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lfvvlvxl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ebpellsa.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bjrhltvv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mplvonqv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2eypicltd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vdauawwm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vxusdpap.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zmgfnnpr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pdoecvns.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ydenxrou.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2rsnzigha.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jftgylqd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jgxigoud.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ilysdwdl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2idggjnji.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qhmujliu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ofscxynx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qygnuxgr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2kspeigob.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2kupkjjgv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wyierkms.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kuacttiv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qwrndwzi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2twrjuins.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2krcaunwq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qqdwkyas.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jpgdatur.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2zocoikwo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tggcqchl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2iiobsyyr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2gcaqydyn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2corstxww.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tztonhln.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2kwufzesw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bawthfax.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rmxhrkwp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pcqnfefb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lueemfkg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tebojuzw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2yvrzwmai.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ppfakpxe.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hfznhpby.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2placzdko.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ckvdejfr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lhxwvprt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qqfxuqhb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2uuzuxlft.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2nluxfauq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mgrenigw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jodeagjm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2nbhaijok.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vyxflibo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gvnrozud.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qdfvvqnf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bsngtade.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2wbbcvelc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sireyhhd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2rsvkvpvn.html


<!-- 参考信息 -->