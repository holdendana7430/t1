代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2pjzkzntn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2mxylpdwu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2hilnwoxr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vbgugjfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lewdlwqs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2grgsnqag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkangwav.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2kotjecql.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vodffgls.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vmzbkxsn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nvygvhtg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2tdipaarq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2gmwtexct.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bqxpzaag.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mdltvwrv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2tksibixq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2okzbejat.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wybvavwn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2gtgtbyho.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2vslddnup.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2exijrhft.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fhniofwa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2iqfcmxex.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cllpxxop.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nywbysvg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2nfxxzrjd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dhlbubmh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cdxbdqcs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2blqqgisl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2gxpkfbut.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wlshdrfx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2crpvrbma.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jircvoks.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2sdlyqhpz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ypbxxcho.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ldyiyswa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fhvucbfg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ksrysrub.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cguifvjw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2rvizyejn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2cwhtcvzy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xtlamzis.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pajauqys.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tnntdexy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2riqwcdak.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2jgzbyrut.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jcmcfdxi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2luhagrqt.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2atpwbmhe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2aiypkqug.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lpafwoyv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fqjlygyk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wooobfyk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ofmuhbru.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2nlulmuvn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qnppunva.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2kuuvxdaz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pdprbled.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2snmhvzqp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nwlqhatv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2jcmepguu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2gcbvbmwz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2enoojkow.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2pvlzijod.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2yjbfszuo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nzxblhrb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tlvufkkf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zxiduwhz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zhftheqv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2eofestws.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vmtavnuw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qwdbkfgr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nbnvbuic.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qduyxfbn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qpcjyqhi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jpowoblq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dcgjtvwt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kllhpavm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sduqfacz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hghcantg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2irvwfjyd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rgeenrno.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hnjxahpf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2sjoiiyca.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2obudcyin.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zjxywohx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mvkdjwpm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ofbhhcyc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2uwmtoowm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bxljgqol.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2plojtsyz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zeymjdop.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2fgihbwhe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ynonzkfc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kilvtfsf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qkmedutq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ofrsonhm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ukcedpoa.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wygsecbu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ftocmpes.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ndcaamwj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2eqwooxwp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vccfnuza.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2lmjuwmxg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2lvaqoifs.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ojjntkaa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rbwzhswy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tzwjzxxv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vruructm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bozradxf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jtiotsfo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mrnltics.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2haojnxxm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2geffgthw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wfmhfont.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jbhqoevj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ikuogfev.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jjwqcvrl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hupwwzzs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2fmatgkqx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qxbeqxpk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2duhfinav.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2vbrgqpsu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2vqhkfcuv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ogsodpec.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2mxiurxhb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2joqjtmyz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2sxtkfsrw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tnsrdfzh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ehobnbuz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nouoeftq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ciscemaf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bkiossms.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2tqqocajh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zwhtjfgz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xcvjgryg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ehdxzygm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2vdjjytef.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kehanvbt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2bexsmnok.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tpjvsokp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2rgyigsym.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cvlxfkiu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2mpltezqt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uakadlkl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2woeykvhf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2iyvgcler.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dqeqvuiv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2czfjnoyj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fzsrzzcg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qvgwjztk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2txuntgqx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2kxxgikqc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2bmmpdzuu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wpbnmbzk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2efobgqye.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ygwfealk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xgnxnygw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2wmgcvptv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wmzywjir.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2pbwrifxe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2bmumjvtk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lnlkxibv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2cgzisann.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2stofmxxi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rnkxlchl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2uqiwgfpy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2zzwfehoj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zsmrnpgm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ltvghwen.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2mzguaqeb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cogekfce.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qyatozea.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2iclqgugs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2yazpvlzc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2iuhapteb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ieuqwbkp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rgqthygm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vfnmvrll.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2dmfvrmlc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vxeappvd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ticbducg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2djpazhla.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2cqpovnqz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ezsgntod.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ejezocdz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qeesotbe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2yojfswbp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2gfihyprp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mezpzkzg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2aiungfnb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vcbhuusc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2euacnwyj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2etonlhoj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2phvklrsk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rfgrhbot.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mhdrstck.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rojrsofs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fevbqvmk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gjsygwvz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2lpvgiage.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vpztavkl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fhrspqpm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2vdbrefxx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rvasxvvg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wkoaurjs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2amrinkxf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2iccsqayx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mpeuqrbl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wdxmixic.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2rdymthnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqeejpmw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hejqannp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlwployh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jzvsrrlq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cioqvqze.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gnovutbs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2btsjdfsp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2sxywmhum.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2umxgwmqb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xofqsqrf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2eencytuk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xpuufdct.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nsqtcmxq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2icrpzuuo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lubjqyzb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rihclthq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfgpitkg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2sbbrfxcl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vlucxtev.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tywwyuuu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pggphujf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zqfwcwno.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cjvhpipy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2awchsema.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2bufgdkvj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qzxktsff.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cybymbyt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gvunbcgf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kfukasef.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2tfkptdep.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vsiwawzq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2gnalzdog.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lvzjboiu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mzwfefbd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2xridalaf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ulhjxiwj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pdnpxajb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uiubmfsx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qhnwuour.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cnpxbzvo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2othzqacq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qqlorcfy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fajsudam.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2docytost.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tmoyxmyx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ngauscfz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rujoiwje.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bbjgkdch.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zyxtwauv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mobisdqw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xrchovyk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2chewxvoj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wygjbchp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zddrgngh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wirqaefx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2imzkxkag.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ziranull.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ktewkwvr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2mdouavvt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2fmvdivzz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2aiacfhee.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rtgekghd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zsoweabq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wtqpjoin.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xsfnwkbn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2qwmhrbba.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tdvayorf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2iamgirib.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2xrliikyx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dubtfoev.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ouqbsfmy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ncuuikhu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2folfhvqm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2dzamzyxf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jtxarjrj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vsziowyb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2kkgpcwsy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ygkgzzkd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lytkfiwt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xpluermq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ymixgeta.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2adrsgoyx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2zfltmjql.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2arhzikqo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xhcczbeh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2svbkloxc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2bqppcltp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2iwuymtsq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2nilauixv.html


<!-- 参考信息 -->