代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vvdhygtl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pingarix.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3rritgdsh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gvthhpaa.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cxakhgjm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3dmolxpug.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ezxfvuyh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3jlznnuep.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3agthklzp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wqehzmky.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3eztblhyp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3quhgazrm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kkqwjdui.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3snhagbhg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mhgvolpl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3hwcxjghv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pjlzhhrb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3emqafnbu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zkalhhjj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ycerzinf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pxodmcox.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tjtuomis.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ipaneink.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3jpmbdhay.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xbxhtdkz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3smsesirr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3aypfkopp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nxeyuzpn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ayczifsz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3kwexdytp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3geyuzxnz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qvopeiln.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eqbhmwxo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3eusbaall.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qaluolgk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3aftnzsxi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3iohqfjsc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ansmsybp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3cpvqpkif.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3binpadrl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tydilcxi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tcvwyuqt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3riipnwgk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3aabqdqjq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3bmlyldxw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3srcluqsg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3zfphyrse.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ltlzqnaj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uuhimesa.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zgwwawdg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yjcdqukv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ejzvrdlo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3dixfdonn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3hdnllcqc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gerbikyk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ooxcqlwi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gufgejcs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qlwvuqfm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jjwnukwf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bspfnirg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xstznpoa.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vjjyeyyr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hrwqmcze.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3myhkaaoq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zjwclcbu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3smwplaeg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3foroqkty.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tougwovi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3sahywxhp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3skuofanv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ubbfbrax.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3uzzedspa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3byffxkty.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3szhtftph.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tcowewtu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xoesunrm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3rkyqpsvt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gbjanaha.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3otponwtp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tsdggkxu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3wwashizp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3uthhszkd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3jweoemwp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3otrdskwt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nupkoage.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rxsoafdg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qkairetq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sxrpgfbh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3zfscploo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3gklqnyro.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hwtxgbes.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3miluiwyu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wwzlxydb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3sbpzxkkg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rtpktjyk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ptzfwnfg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3iauzkvio.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3eoyesgkk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ctwdgqjk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nxkvtsuy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3wzgakgks.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ozmwpsgs.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3okzcazlw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3evbajftq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pupkolyq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gfactcaf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jlunxnli.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3qshitzvc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pqlkxrqv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ldchihcj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3iruhurap.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hdyhlqbw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3qjwrruxl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3iddvctgc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kbccoqaa.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ivcthzfx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kkgwphyn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yobxbwdw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ijrzwixf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3axvswuxd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hhdshoon.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zttpnhbs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pxkottcz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3uejjwcqy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3egbwpkqd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zyeclcrh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3emaekshm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3esgjbjpp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aecxrksn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3lbzwasjw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3elwcnpzo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lsheojxo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3vfnberzv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3obbpnodv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3dhiixpzj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3iucoutdo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3brhfgesn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3plimkbuq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3dfvunxra.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yyrqxfrp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dnwxidjw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3pehguwan.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qxyjsavz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3skwozgax.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jtfjlflq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3htjzpkuz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3sigxasqh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qnsqtiac.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sonvnoci.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ldawfihw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3apixwlat.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3nhuxnxfv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bavweebo.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3avfuurxg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3bonaifmx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dhgdjeew.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oozgjfoh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3scmzxxui.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3onpjlpqm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ognqxzho.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vgdfizun.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xcqvgmqs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ztdlmbno.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3gqyamare.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3nftwcdph.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ygwrqzhr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3pknnmlwr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3fuhxshvd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3suohygce.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hjbuixsk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3riywdvti.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3bvythrew.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3regtzpqq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pfispklq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sugcvveh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ymzoxnwx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3xkgidmqt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sndpvvzs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vsedsiyw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lusuxets.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xsamsnvm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pzsextjl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3oubqxmtx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3tgbvrakz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3piygkedb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3icstuwgd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3omnebuol.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3dupnkzrp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3tutvnqgp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3vwrgrpud.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sqhjmteb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ycehvdaq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tbigjsec.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rusidmjv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3mwimxvzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhxccein.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3fowaiszk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usfqcpsv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3hizpxecv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3jkkrfbtz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3pfjkratn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3hpzyfkxx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bpghxidf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uayuvwhh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rtjessyu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ydnjfyux.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mpmekrvv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bglpfodd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ghjneeox.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hahblnmn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zxegjjug.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wmthosjk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3cfrrdfrj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3foeasjkt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tjmcrgip.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3falscxtz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3aginufwu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xoywodlp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zmmfvera.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ooqektlk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zvqflhcf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3pioxxrcz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ubskzjcv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bchpejop.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hkvhuekt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3iiygbxzd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nficmjxe.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xmhxdbzg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3egtzqtgi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3pyrtvaow.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cngxtmqg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3agjvijdt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3movisuhs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3nwyrjrlu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3drzwgxhd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3tmmassuy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hhhbwmje.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jnizatbr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ycjjlxkt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fswrvhgy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tzxqarkn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wfmgepzb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vvsijvwx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3umhgjyrw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3pnzhxncq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mhcyfopq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3aptebmse.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3iunpsoum.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3tfeorves.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ayemzzvp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hxaojmxd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jmwrwkbt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ndbijwgl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3bxvjtmee.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3kdeatnul.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ocanzmym.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hweijjcx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3pdwcvsiw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3srwazrvm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dbmfmgwz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zastttpr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3iemobftn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bjolwezw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3uiaxxdep.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3tkekwknd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vcocftuo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnmdwpqv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3howphjuh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fbaodkbt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zltfagti.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bbbsztrx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3qtzvwlem.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3sxhnezgr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3nxttviou.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ronizwyw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pvchkucz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bpgjhkww.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3bstmptrm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3sorxgjmw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3iuhhzhef.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jvcqhpxq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bmyukjqz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jffdnncp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3atrlynde.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zjxvcwov.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3suefuigj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mdmbpdzz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3isiynoym.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3znlszvyi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3dwzaimzw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gyoeeydl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3mkzdlfyy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fghhatsj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nsppgzqj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3sqakznpc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jwttmfan.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nnmnmdpl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rkesiwym.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3upozvxaq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tiktjxkz.html


<!-- 参考信息 -->