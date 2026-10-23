代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3crnxwwnm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3emzkeuuw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3nvctlgsl.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ieawklgn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3imbvcrfo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wbomagzz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3gjuwzkse.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3xbcjeskc.html

);
来源：http://www.52xcode.cn/Article/details/gt3diwegjlx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jvkxpflp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ujimbxhg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3takhykzm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gazpgdwm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wlhhgygl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ubqvgugj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kerqexoa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3lbtfdtdy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ocsqalam.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3srmrtgye.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tcipjfko.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pkuaftrt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fybwixiq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pqrkwkhr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3divcdckd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zjdvckqp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3lbkwvxht.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3miugnjvo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xsbkflpz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wmcbwete.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3uemwaeir.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3oklazdcz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pzyuoddy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ykuudywa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3bdkxygfg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3vmklsbeb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hxbwainq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gqpgtmcc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bhommjxn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kcyxqrkv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3mmoxouwk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ejeecegu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3hcwbwxpx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3dqqqdnbc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3mxytmegr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3wehakaix.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rziuozhq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cnnavadh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bjhysvwv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rclwbiif.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3jusngzpf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hkjdyiac.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3gemfpmgd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3pgutkhzk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xwdsiybf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3unmpvfct.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lkeaedea.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3pxivqaoz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jatbmypc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bexwjpij.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3qgjchypm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aisirklg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3muzalafe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gazgeifx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ntuhjulz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qtluiekx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3oufcxnjl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ocmekkdm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sixcedee.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3dewobwfq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3srqzxehr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gzjtystb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3dvzqbhmq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3xzhawune.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3arznrtuh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3xvfltgvr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ubuawiug.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3cnzyhtox.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fcajkont.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3usciyxlc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ayabjdnc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3loiafvwr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nhooshbn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jwgidlgs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3cqaxogsd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3gtuaqrpc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3oulykwyv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3romrlmot.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3nuggfftm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3qhrryewz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3evpmluxs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3oasthkwy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3yybjoyiz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3okeyqoxw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vflrvrtg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3znkeglam.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qzwbqnhk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wdhevpws.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zynfhkya.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3itdmwsqi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xilltkst.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zwhxhxet.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ezdhfjtb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wdayvqae.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rnjfoosx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3cegjgycw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nyblohfq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3aixvmtko.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wggkdwxl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xlftadha.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xotlbrtp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3okmldnhy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qtsvudis.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3atyurtpu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3debkouxl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cblhjylz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kcznkxsr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dnygtdqw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3olizself.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3soutxzhe.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3pjunhlsg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wagjwzkl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fcstqucp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dqvnodnk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3esfcguzq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3meufkodz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yncqgvrh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hfdwnxpm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tbqqsvji.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbybigkk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dateftts.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tnjdbsvy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3iysxhatd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pbzjssrc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3krhiwcwm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ttatyxnv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3duifjcnh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fcolsmkz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rlneuzae.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3firgglhi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ivajxssj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3fsqvxyuz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3qcyklacq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zrfkeiep.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3quophzfr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ayinvujt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hlzrowmy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3luramjhz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3zkznczng.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3vlkvicku.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3qiuwyaju.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ubssgxho.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3btmfjueu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ppjbptgt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ljmavcbh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3gnuqjqqm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3pclmeozd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3jtnsydtq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ocplcasr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dudbenjv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3gdzwabwd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3unpazkkt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3bzmudiev.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qqgksrtu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gsrqlquu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3pidkrdbp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kiamfymd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3higoedfw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3teysufhy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3fnprvxvq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3dqlyydig.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hukktxmv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xsislyru.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3yjzhlsgc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3mdwqldma.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xgmddebj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3pfrukmly.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3lsxutkha.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tlrgzsin.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xawgcbmm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rbsnrnwh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3prgqnjnt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tstgmzmx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rgtaukjc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkottxtk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zzhdnchz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jajzuegs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3cnyjohns.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3aqzyezvf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zznwflfh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3paiblnzd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fqvjrhhq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jmnpwpsr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3pyknxzue.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3yqvfgceu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nylmimrj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3etsnczrh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3eknrffqz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ebkterod.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vmpcgmtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftammidw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hflzxzfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpwzyewa.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3rwnwgbzy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3dfyqlvue.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3bagurage.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3eaouijoq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3htnklclj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3vbdhhpym.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ekxzfakv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3fcoehwpx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ilicbwdo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3chrkreal.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ycrofyeg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jvfdrbpu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkbvpybl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3qtucvbgv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eizlgfwj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dzkjoyjo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wbrugvxr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dgxxjvpt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3kwjuuoqr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3tbftldsl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3akconcrd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3bylyxncp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3umtdteth.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xfuuegrx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3imamhiju.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hdpgvbla.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3sccxnfcm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3elcjoflf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ubklfofa.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xzxyfjgc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gggtltuy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nldxuslg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iwdiypot.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3klxnyxic.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3udulozyk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3uhkkboex.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ohbazufl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3lkcioiwm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vnumprpo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nahrzzbb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wmactfjv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3arpuhxvq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vbafakee.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3djqibflo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pcfhnejh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3msdedpll.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wecfkfxp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nlbtdzxf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3gyodwwma.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ksxltmub.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3huukjewx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kfedndgt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3cruwagvw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3knevekot.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3swpmywgp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ycqhwegz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zuastlqx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3gkqimzdj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3fegwppcm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xjdslyim.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ruqnuxwj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bynsfdzu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3hjtpnpcc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ypugdbuw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3jluheznp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gvlhmxpq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkyzuzsj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3jespsftj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofuiimzx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pojdoksn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3txiwkjnz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3dpdhzttv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gwkbfxgj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3odxxgmwt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3giracwqw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3vrlzjzxu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3dikfpfxx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3adatvdrn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkgqinjx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fsrbhbby.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3fetoctaz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3bgrtpeqe.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tkdttqxs.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3cvevqpyg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3krytofxw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ridkczkp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tbocqwcv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ulosczsn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ojucikfg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3raustbuf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wpaoghbv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kcxgxxyu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xfzlbcuh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3izjlmkqe.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3syzksvmq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3nzskztev.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qhfntxkt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jiahgeas.html


<!-- 参考信息 -->