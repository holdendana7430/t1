代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3uzcqtftt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ofaeikjo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3aligxrzq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bgltbnga.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3uizlhffs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3qykocvmb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3lrrzetuf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3citdfwpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihkhgktk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cjbyjwps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjpzqmdq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3chgyovmv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3akeefazn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3oaqfageu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ljllvfhu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3dkdtbpxa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ztawdukj.html

);
来源：http://www.52xcode.cn/Article/details/gt3vejeucvl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hqmlbqoe.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ncmgcyfu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3njhczcod.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nxbffaqr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3bnnfgknd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3bvdgvknx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tcyxxtdb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ulqgbzmh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ucerivya.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ovhqnqla.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lpvvkqsa.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vqeidguh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zlzsarce.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3aaoyfmtw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3hvbbebhy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3lryskuba.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3lllykyae.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mnwyrutu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mhvtetvh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3xdluykvm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3arcrtato.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3udaedhrt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xgwvsedq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xytuyvts.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3shbfkmro.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3cgxtetgx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3uqdxqjzy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3cvkgrvqp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3olidapel.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3okbzsfsy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3fawpaymy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ulbwidnr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3lyjqwqob.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3wpifmvwz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tjjoorkt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ogyjgxkc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hphdorls.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3dloxhgor.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3cpmbtmvb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jhtelozq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kobpuhsk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3hdhcnjop.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zkhhqbmm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3uomtucju.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3hhhgdlwm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3sdgfhxkg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3pkdhqctv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wpamhwxc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3krnfaggw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3gncmvdeo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ylbjfsra.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fdfddcdn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wdyqpkud.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dmfuaoag.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3zxshwngs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3isgkdige.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ccfsobhb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ftmgnsmq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mmbclkht.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3budrgnmy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sxgndbdy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yhusdptf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wuxcklrc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3rhbeyjjl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jdatszjc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3uwuvajtg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bcokzedf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3aykrjaql.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tsmtkjxz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3bykdzcad.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dlxupklb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mciyxdwq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3hkaqfcdz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3awecnade.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3siuoxtfx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rwkstqfi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wdfzbihr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3acdfpdpw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vfopqhwb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kvromhkj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wmwyiaxd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gvvckfus.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3eidywxzh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3bcbzbebl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kpgpwivf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3lzlaxvgg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vphzztcy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3tmjlfdjt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3kfaynqbn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ufcuinwm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dfibjjlk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3rfnerhsu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3thduvruk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3rebohndh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3yfvmyjlr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ewipjsps.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3lcvzqlls.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3pmqizrcv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3nfjyizrs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3cfbwxbek.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ewflpuff.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tcsqotci.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qjfryqrs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pqtnafac.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3mmgbfqqf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cmqmkeee.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tninowah.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3cqeusuwa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ybxkelmc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3amawsakl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qsfesuiu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3pnhsudzh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yxbktbbn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3caksebjl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3engapajj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ujzrbqhc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zfnpslmk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jinjatzf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rogpgeai.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vssgckun.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ogrlqgfp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3byvdmpdq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xltlcsik.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gqinnsif.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mzmoflza.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3mqphrtzi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rduaaavk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zlqhvolw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3khhcerla.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ppslqseq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3prdikmam.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3owaqtmss.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3wxomaqnq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nubavlsn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kecxkwdn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sljljfes.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3stonkwci.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jrvbbkdt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xsikcoye.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jsvhmcol.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3srmjjssx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3cjrrvyvu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3nxigwcma.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3sflxzgkj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3adczlqpl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3iubtruks.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3gskhuvtx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3omjhtmfe.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3zgzkvlkf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fugstxgx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jcpydqel.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3jrxuwaeo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3tkxlnvyx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vfyzyxgt.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3gterhcjn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qgefbtgs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hjltyohk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3tesntvpb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hlcmxwlz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gkdkasxw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3luitsodb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3egskyzbx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ozwdhbfj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rqsoxlab.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wiwourud.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3xwuxxuqr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3oyasubcp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3pkvoygfk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nlgeuygb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3inaucxvb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jxgwlbtf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qjmfewdt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3seirwqvb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ajndvdbq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3plugevae.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ajohbhod.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3retnossr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gkygduhb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3omjyxxaf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hyhxksdv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ezbtfhpy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3furysbmu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3tjbmlnbp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hrbvfntc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3cvuopqun.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3cxzazoqu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gxsjuvvp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xpzmicwd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3cfpigskm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3huhfdhmg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3eltgsrlx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3utlziyrz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vthmhapf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fthxhnzg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3jkitbrxz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dhtdwaqm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3epyyqdbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kyhwndgd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3nxzztnui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixynvxrw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ixsdbsmk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3izfaqkhn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qzndloga.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ncwjypsa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3cpbxvxsa.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3dbqbfwww.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3iozgzrii.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xmmfbyhe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3scrofxzi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mqzdyall.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3egrjdhgr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nvqxahoj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cgslymlp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xtdkbdgx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3hecysjhk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3brijolkt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3kpjpbyuy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3knerfeqd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3nukssijp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gaqfljxp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3nqiirujd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jfohwgfi.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3pzbfhmxc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3exusegds.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wihlaqiq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3oyobyaoo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3oqirnjwm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wuhhzxpj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mejtilfv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fboesraz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cltjxagj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3bciglsyr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vcmxquux.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3txizjrmo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mqzahmee.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ccbkyzyn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3efiqcyhk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3rphiowzo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3nbqgijap.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tsnonjpu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zcacysrv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3udjvtczp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ircmvado.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3prprryyd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3nffsqpwz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3osppsntf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jzufhqkr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3prsvaljp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3heplrqmu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zcfbahgp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xrvqtpyp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3snvviykc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3quqlywlm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kizbgkiv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ctninmks.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jnuzuywx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zrixbanr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3korwqahj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jxbsmyuu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3waqbmwfb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3evufenfo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bqqfawym.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bwmgrqvp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ktorhtgq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wwkpdpvr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3mpjdnimx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtpiyymt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fzppymix.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ddrqpryy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ixeuruhe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fzgumqfk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3jtxtpbla.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3iyuraocr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3hwifwcjz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3kcsgyfvq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3kmfqxpbe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ijqsfjox.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ypcboxqr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3xhtmbesx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3gjwueswn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3upbfrtmf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3rflcufud.html


<!-- 参考信息 -->