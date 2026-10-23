代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3donokwlg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zzmjbmuk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zhhaencx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gzpsrife.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3duclpgpv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3bdikulyv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3gtzflbpa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3yibiozsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgbojchn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3tpvwdqwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nioyeexs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3podtfjax.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dudhtkny.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pyvpgwdt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wlojjwal.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3mjeavitc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3yqhukycw.html

);
来源：http://www.52xcode.cn/Article/details/gt3fzxucoxc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3cdpstyuv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3hsqmqklz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yferzooy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kevglcgn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jtnkebgx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3wcpmmjcg.html

);
来源：http://www.52xcode.cn/Article/details/gt3yrxqofuu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ozrejtgg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pfmsoqfk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3zyemetyu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3vsqcwoly.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3nvyskigr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3pposrdrz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3mlcvmzui.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3nqsagfla.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hbtjempw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3njwadaai.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ntgxrwhi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3romxikgg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3shvsojkc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xgpptnkl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3gxrysraa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ryljxent.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mjtkkeed.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zgczmqqd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3yddihrfr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3mbayhelg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3jinfnktn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3hlrsmgws.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lpbgqbqb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wnukfgcs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ucwkyfrj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3wosbglnz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3spqbygys.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lawhshdd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ofrndhkn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kufxjuax.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3frxtwnlw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3iamifvav.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3yfdlcnnf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ibrcynbc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3nphrsmew.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3sjnlapsn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ckjtuwbr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zvwptsck.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gbhjyulk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3arhfwlxf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3xqrrkoax.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3fetbutap.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ltbgrysj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jzixxpjf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nwdxdjer.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3udeuqhtz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3alcpztwz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hoamgwul.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bslodscj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lfszjcmn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3teuwzamg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yupndsoe.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3cjyujjna.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3amvbirss.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3udxfawhe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tvgtvdbq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ajosrrbt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vhmqeduu.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3irixceex.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3unjkfztn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cqmvwfxu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dbgqbnlh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3myhhlori.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3sanhsxmb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3kpriwosr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ocyiqnjn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3jqivavbz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3iwsprwxn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3igjluujl.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xjwyjgta.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3phormqhq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3citlduns.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mthgukza.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3kkejsqud.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nbogebsv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3aizhvnzi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3cndhxnia.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3weubvzgj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3sorpyisq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vozugllq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3yngkivcg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3mywvdonu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3moshazss.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3jlkxthrg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3zcdinbwy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kndniseo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qzodfhfk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gipbhywz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ofexhurc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hpdrbtlb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ikvcovwp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zystacdd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ujbqwfhk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3njeuncbs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yzcrruwb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3cnzamzip.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mvpgnald.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dcvhtyrv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3othuhwou.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ujnlcilh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3rnfvzefs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3grecedsf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fhgjlqoy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pgffzboe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3obwoiazd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nvznchpf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3rcljiqbv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ubzbckwj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3sfdockfv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mkcoaqyq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ypveiffr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ttyccdao.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3bzocxirh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nfspaweo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cwhaejis.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nobrrmub.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3sskzepus.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gpifynng.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3aicbwnuf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jcpoyopo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ilyjtynu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cjaiibac.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jwzhrnzv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jqyvugwh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3bknaipfj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3nosirooh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xmwvczlt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3nxnxnnpv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uphlspws.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ngfpksvy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3aldgcxjr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3kvlnqbwg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ugcmzdvu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3dorzcnlb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3peinbjch.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3rfzwxayg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3lwuwlrcg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3tqfmicjn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ejyhwzmv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bjpextll.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hnqpestg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3hzgaewcq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jihoxtxt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fsenpzwo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gyyxtcsm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3skdjizto.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3heaymxjn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zqomuduv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3xbetyrzy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jbrtgexo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qurwzthb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtavekyk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jeaptrow.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hyiinast.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3saegqlpd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nxlsvjga.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rjwpvukw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3humgjzes.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gbkslijf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3dblgekpm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3yoyjkiwm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3jgnpuuna.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3cphqeirv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mkagekxo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3kyjeaguf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gilxlajx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ffgfcsfa.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zgyoxoqq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3loyayrph.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jyevhgwd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3urepxddb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3imqzjcjp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3czcalslu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jgjbkngx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vsacyrxp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3lktckcdu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pkcrvbdd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zlbrastq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3rhtnjtoh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3hmzfkquv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vjyhpnsj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3evjzeljg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bsaaqemy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3tmgbdsca.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3hifqtvsf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rqmlpexv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nsnzcnsd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3vxuqhrmw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3khzvbtmg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3xuflzrce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdvdssro.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yworsrcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oruglaph.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3numbevti.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3druxysgw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3gdxwnpkw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3rxvtxuxx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ascjfjye.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3uxfbsvsz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3nceirszb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3domplojt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3feuszocg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3bnxdzlhd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3unktdtpz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zuimmohq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yxvcbnbb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xwoelzac.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lbwndxsm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nomttebx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uhchvkjc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lmxxnwye.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ibntmadh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3cmpmxchh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3jheooabh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3byiuhcwr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3josqylbv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nkzimdrd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kltdqjag.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3czdrogip.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ynysidji.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfniccna.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tzdzubjv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kspsjrvp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dcaapird.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wyxhtoel.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xljmhtee.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jxeujnhe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hqexnkgu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3psaoyruo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nikfcucr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mbzqtrga.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3gflsufmo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rvxugmto.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gfprusta.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dasjxqkf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3oqlvxkue.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zqankvit.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3fgyhtolr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zggpeffl.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3edmnrvts.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3remhmipa.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ndzvktup.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cmgduzku.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3omksriya.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ursmtlfn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ptuwgvvf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3gcvoraqf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ivitdhey.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ogmdhrxc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lvqfmsfr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3odbemxol.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xjjunlzn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3mbsdgsib.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gjhxqkdk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yhjoexeh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vfewqfrr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xgpdnava.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xwexdosw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3eyabdwsi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qsgfkyvm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xstapagi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mqrdytau.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ksydrxee.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pnubuzyq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3actwqruv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jojoygdp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zjhqvfbz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jooulool.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3yrfdgwfj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zyoldkmc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3logofkju.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vunliack.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3iqggmjpm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ablefrmd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3olugmuei.html


<!-- 参考信息 -->