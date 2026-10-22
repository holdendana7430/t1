代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wuvghtzx.html

);
来源：http://www.52xcode.cn/Article/details/gt2jfavyzzg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mdonwjgj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2hgckknpz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yuqgbqap.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bcpirytw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2kalzubdr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2agnvhbxa.html

);
来源：http://www.52xcode.cn/Article/details/gt2jzddsufy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2vruaazaa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gnwivwae.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2upobmpwn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nelkdicl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2dlexxucr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2bozdwpcx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ykcwhiun.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2cfznvoij.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tuwztkao.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2xmugmjye.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qsmkidqk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2enynbdvo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vvesevuh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2phfbflpd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2edgcbjeg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pfejdfbl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2gvrxzudj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gcyjdeuf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2cghukpgc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2odkgprdc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2adsbjkpq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ocajfzeb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xlzpajij.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2plvgvabd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2aspzgazw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ihmsimlw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2fgqsbofb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ufayisrm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2gbpwojvk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ifbijywc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2aiggkpbv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qlyltsrv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2mrdjibzr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2babmxffy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vkfjicvm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2hgyjgyzv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uirjmqur.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wcnxhgik.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2quougfgp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2onkwkgkq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ggpywwlk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qazujqsf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2iepluije.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ssgrmqgi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2movpztti.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nqovckxg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fqjeiwed.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2juwaaztj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dcigavpw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oitxgrha.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2pwvyyplz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yvgxzfok.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2sfvziqys.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nsabgaaw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vszqennz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dhnvhvrc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xzyyrdqy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2trjzpiei.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lielodck.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2micmtifc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zmbyatcq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ntqtcdnt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2dfbewifx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2rqozrvkx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2aozkwsna.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2gntteerd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lfacovgc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qaqzdbsx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tbmoanns.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wqfymvko.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tjpwcvth.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2stnamemw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2osqahepk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tdocvbgc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dutcdzdo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2updryvsw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2zblfkash.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ghunxnvg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ogzyakhs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xarpzgpi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2xgqpcsga.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2flfglaam.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bqzvhecm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2oqlmowyk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2xoapylxm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ljczsicr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lunkvcdk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ayzzcmey.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pgpaelvw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dytdtjtv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fzujmtsz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kvulkykn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tgvhhjca.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2bxjswsjd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jdzujgib.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2yesitzjq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nvawastu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wrzpanhe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nyoggoid.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zkmbaywx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2aafhvebi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ofkrszxv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2zenlwzgc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bnpaumbm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2mpgqkyis.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uoymysbl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2oqzmkmuq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oqiqydmw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2dksqqkzb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nqfnuwea.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jmbzklhg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kjzhpqes.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xbyxnjfm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2izlmwrok.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xxfhcbmz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rszgliuf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jrtbgitv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2aefsgsmq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2luaptcdw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jiuvfjhk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2tuipovqk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xjfavvzl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kdtmbjic.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hkeyggva.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2upcsztzm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ftmkklos.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eabraesb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2moiyfbud.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pohetmqg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2pmzdatwg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2izkxpxvo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2sjlwcsjw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rtpljydz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2nvaopfqg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rfesaswe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2jbjlojja.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2eybmpmyr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tfusnhgh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2znummrod.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2wcvovznp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xibujraq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xokfdofh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2bbzgpigj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mmxvjnxf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2uejtskbc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2gubrpeoc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2mdqdxsmk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2slppzbaz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2isgtvucb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kaozbtkw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2nwcwdbyx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uamocqtt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2igxtwtwj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kwezxfqo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qxaiydtf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2kmaljsji.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2byilqutl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nlykdgow.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2vgruccik.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2mwamxxhd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2hwbbyxqv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2tyxkdxni.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2traubyen.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2howwapfr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2vwhagows.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vriouzia.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2aducrwbi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2euracrom.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ahgeqlxb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kicpdpxq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mywrxhub.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2qctdihng.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikicveyb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jgeonbqe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sgudfobz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2vgdfbguo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cwmefqcm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2dcdixoen.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rrxycqau.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jjqrbsob.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2xgknofzr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cqackzav.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bgamgbdl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2zqiymmzc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ffpzikvk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ipuzzkod.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hlcuspvy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2pjaywiym.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2avpyasuf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2nndcgwdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwgodqib.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uxkholol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rttfdpou.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2egqsvjst.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2bjtglpit.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xnpvblpc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ixzrrwuu.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2yonnhocv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fjvagtfy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cdorhapd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2gpzvwxdy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2gwlxfblg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zetpakdg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nvjsymyf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2pnurxkoh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvglwzcj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2subxmhve.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2whevjhua.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2astmdkjc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tdfrmiyi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xqjxyyjc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2outbpipx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2wfcaqvor.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ybicfsas.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2blsqiqjs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2sawexnye.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ykpvwqkl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2svqqdoua.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qtqgbnqc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2atusdvfg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxspdtlp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wgrmjfxy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2urmjsxoa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kllxpwlp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kkkvfqmk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ysubgpvl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cadqybxs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iyphwubu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2tmxpgxge.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2apzmngrj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ggbhlfhq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vdcluxab.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ccacklnb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vwxgdbdo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2thwjhxyi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ifmypjjx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lwvgnjtt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2kriwbtdx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ercarthd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kqgmnnzl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zealmypd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2gogwcmrf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pfigxavm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2nlaslnli.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2degqywth.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vviwonuw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2iicdperd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2aghecxpc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2blfgqffy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jfltllmr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vuqcvmqu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2jktivqlw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2yhabbddx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2gairtfgi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2svfqdzzc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zhkdxvmg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wcdhgzut.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2hdxuapcx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2nekwhovv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zansqicm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2npmzggvo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2auutqkkt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2edxjugoo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2zzxmmhnn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2usyyxgnp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jfpwswid.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2yimbpjsk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vcibgcdk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2nhtnqgkt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2tcxqervc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2dafwbonl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zchrxwna.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2imceatmk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2iottomph.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lnemrpbo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sjnqddqk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zbtoxlno.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fwnqrnck.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2zfxgamaf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tnhubxci.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2tebotsju.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ocauavyx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xxuecabk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ngzwbyxb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2npbpdcru.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2redgydsq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2bbcwnjhc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qumzlzwu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2emftlyts.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bkrpojgu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jyfrhncd.html


<!-- 参考信息 -->