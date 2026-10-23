代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3agshaetu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3veztebph.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3uhnwdfwz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3exdlnxnh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3etgcgpml.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uhgxenmh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zorvyqto.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3uwbjvgbw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kpotufix.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3uipaqkrv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3avbnguow.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ekypgebc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3efejkvrk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3rnxsccil.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qzmdsatz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3lgxmluhh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zggjdrad.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vacunitv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rakmfckf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3fjktblzb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vyspziae.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kvgdysmm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gosqewgu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dlvbdqkd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3tjkzucrz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3rlodlukq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ulvteiwn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cpiixtxh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3tlpfgyug.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3pnbhvpuq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3uxpmponl.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ndzkkavo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dronwqxw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3etvjkbvl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3igdudviq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3vrrundjg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ozxarene.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3wtazrlux.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3uyibzfmo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3trafstsf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kfqqxppl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wdwobpwz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zhvpfxaq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3mbjyedpa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xkppgzxm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rjxemjxw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3rvzthjcn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qnxhieil.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3adeinkdw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3tzuusaup.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3corquxxy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3aazwexek.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3emcbfvcy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zabpocqm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xbxgtkwn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3zbbwpsxy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xmyirhbl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3nhozyute.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3loradwiz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gmixzgzj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3omtppdcd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3asvgbqmj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3witmebbu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3kqtwacvd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jgkiifnh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3recgfitc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zoutystt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ppuvtask.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gcldjqsx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3gkrsdsmc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3rcpxkvae.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3raheubub.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3sclkyuum.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3comicafv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lnvhuttc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nlftksme.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3inezpgbp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jwzcytob.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3rkbgngag.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3mngplouh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ulxnswju.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3dqkfucpk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3sznvnaxd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ayxgkfsm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3gyifsqsv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mczqvvao.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3uatginwv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jgmimvzf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bbnlemgs.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3solcdagt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pykouohs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rygrqxwe.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3kuhhtpdm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gzpbuijy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3guxwzvrs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ctxxoxpg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cvumdema.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kfaivwjm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3boayhezd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fwbvsrwk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ssrfdznt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lepftxye.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ogzzmenu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xjeslkba.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3izrcxcth.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3idfmrctg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ejnmwxtf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3pkqgpkva.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tfugqisc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zoqltgby.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3juoadycy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nfcxiemc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bjctmphh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3bkpwirat.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gukdepbj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cthgguuh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fzpzxbpe.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3bvtndtqx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ngnjwecu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3xdasylgv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rcnwognl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3aprqeedn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3cflyzsie.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3oifzhtym.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3auruqhqq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hcpwfevz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hpxifing.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3gfavzzne.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3egwgobuh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3cbxsbrzs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ragrxngc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3phpjgxxf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3rxtiexsj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dbcchonc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tnuoyxar.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gjefvynz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3mgaknclq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jhbqqhop.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xxyipmxd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3fsuewsmz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3itejorho.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3iuvhcrus.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bhcwnrmd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3wapvsfyh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ahvalmvp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qcfimnjd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gchwwwnk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gnxmrguf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3lxpercry.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3cgobmsfm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zygrupcq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3zwvxnlzk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bmcpilir.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3gnlvinbh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qgqwhskd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ausdxzrk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3foyneidg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ohlduemb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bchokcen.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3zctqprki.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3akfzxahm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3klrtmbbw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sjmdrgqu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fbdhszth.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wutgrlbb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3kfpqfvnx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fdejsije.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3eivvobfe.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3oukkctln.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3nhraxuku.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vqjuaohm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3couecpux.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lxmpvcqb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jujjnsrs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3avotiqlq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eimybpxh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3klbxprrh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sjqbssqv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3heohqptt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cpymgoyl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qzktzoyn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3edlqpgks.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fpbzhvzo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zjsbwivk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3caumrcyq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3pnzuorkx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3idmtuthu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3nvbwgvmu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3abeerwdp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qddstppv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sgwxmqjt.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3alexbpwm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ikzktkmg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3bvhoopcc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kdjexsft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wktarliz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yvgcdqfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvfwsswo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3loctzczg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zxqtrwjm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3abfbeoso.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jfukwjgn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ixhunptd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ckohfvsm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3smckhpfd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jxzmyljn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ecdicisr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hqxmbruz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3eomfvdoh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3abtiopmv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zvyjsapf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wqmhclis.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kxdahvwx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3snqhasna.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tmszptli.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yrlephfn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dmpzqgag.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ujdmbqrx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3xaduojnf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3mnrehhxa.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3emxjmqxy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ahgqdhpu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rzsrrigi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uyhujfuu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3euyqdagh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3gnwtlxxa.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rgdqjzcg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lofamaky.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3muvkfokr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3qkqrodtx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hevoirrh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3puyxfjjj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3igtnjdwp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vipfggii.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3onjatiqk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3zhvwchnu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3benmcmtk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3bwdsqhll.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wqgiewxo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vxyfjfho.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sgdjvhhg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3mufbgfna.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3cdzhltbj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pwanypni.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wdqpgwnf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zjjqpguh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3bomjakra.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3llnterqn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3joqwqdei.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xnrwmfuf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mmasrcxp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ucqzjjld.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3njihwbux.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ebkivizx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3yhxmcqcg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lsldsvcj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3mzpquemq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xbpyzvay.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jxyghuuq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3txybwbji.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hasvtuhd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3laupfran.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3dejmfezu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xjrpidxm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rajkbmwx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hrkrdijd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3akchveth.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3lohvlrex.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mgqclbzt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ytrpztgg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xhsfxuca.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qaqejmgo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3russyjmw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3osyisddn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dcyehdig.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ezstcvgo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbsahmkh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3gewglcuo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3aaptqzss.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3zxjxoeuk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ailzjbmo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3plmzodxe.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xywfqnvj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3opqbgpxt.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xsxaenay.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ywjkkhhf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3luvvsjta.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvyoplhv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ckgysfrh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3wnmwytmz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3sikryzof.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zarhfpaa.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3flswxhwd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xjhdgras.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ctldxnal.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zrectbtb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vyvqybam.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rujwxhxj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3utllfbyf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mlacsnqp.html


<!-- 参考信息 -->