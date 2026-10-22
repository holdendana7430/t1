代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yyvmszap.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wsqoolxw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mwnrycmp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2jxqrgsog.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ezsddepz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qqbgrjgw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sflaelcj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2drdkunoo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tkcrgmvs.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qnjzsbwh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qytlenjn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2pdjluvum.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2zwgaanzb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tpjgfcnv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xmjqlgev.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2nnduoghv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uqrcqums.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2nejhahyz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bouxxmpa.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hmfqctml.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lmytlgkk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wwgjshrr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vdlhyqps.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hkocvbhm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2awpcsxwg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2lbirqgno.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2irtiblde.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kvphwmqe.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2yucpqfvw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2lmkpkuna.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2elmskuok.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2rflwoqcm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2llnonvvd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lneaifsv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2saenvfcf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ikhbkzjb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gymoznls.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2flmvutrz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2eairgmlw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wpgbxasu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jcwbzwzv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ckuhdsed.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dbrvlugv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2pmtrczpz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2haquijmz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xrjsctbe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ydiyynlr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2obixozcj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2nhuicwzf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2yrhnbyks.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bdrbtaho.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2nkqxkixq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nvpaqxvr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ikdsgrkn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ohcbnhdb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2drgloeck.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kodigune.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2goomytpt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2htwrbepx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vjltuzbd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2alqixzjs.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2priokprf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iirpactn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mjwhemyi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dkllsalv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ozjtezzy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aazkjejh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2gncbgvye.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mjtbgrkc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2orotzwfx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2fmisbiqk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2dbotsgxw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2sjqfbluv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vukvlxhj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dgsrvpex.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nmvapjrc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xnjgmtun.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bjekekoa.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2exdpvhih.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xvhnsbnu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ckvlaqgk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zcoodykt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2eezumfno.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2uakaydep.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nypjwolh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2oshzpbag.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2irllnfyy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2byevgyda.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2rlpqbjbl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2bnilnune.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hzpiybek.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pftapldl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2omayyqgm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2krtkddxn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tdwijcgd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2lurjvvgd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hpufldpm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ddpqiamu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ovfsfdbb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2osucriex.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ovirgmtk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nspkblta.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nlskdhch.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pbkcyxpw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2tbszpzqf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2neuyxwep.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2tckjzopl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2aozfoxhe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jcgkgxri.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2udilvjps.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2smlhsbzx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bvgjsovb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eguwujrz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2csshnikq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pcoobpqc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hawpfbih.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qzttrppn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wjcpjvkd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2sgszcrjt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2oruqqtpg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fqezrmht.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2owysflqm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2iqkjpfhz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2sgoiiope.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kbkznqtd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2fubbshtf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dnvtdvkg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xzdlemzq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ednbvyky.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kemrrswp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2eylupbsm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wisvwbut.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ztvibdxp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lmqwxhrq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jlpyahde.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2htioqwnq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2sdinmoww.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2woiamvwl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gfhbfabz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lfqikaxe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ehmazlbi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2gcqbcqoi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bxspbsct.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2yuyqfvgg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2szevojhj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ptwbzzgf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2zgvedpuz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2dqhsmqtn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2luubsflr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2liojldel.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xivxipzk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2pvaweohk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2cftzutia.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yzyfqvnn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qkutmcem.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qunlvrrl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wedzhakl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2bnpkieop.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pyrpgklu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2jhzcohqy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gxhymyds.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wnizhsvz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uohruoqt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2amkwmdgg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ppfaffes.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ohjlmotc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2gmgwstds.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2wxpqbhpi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jpkgskwj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2khksibww.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bwezwvxr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2yxqpkddo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2gqidomvn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qxxbrsst.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pmutegsx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fevxgusx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2oizivuts.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fkcdjktw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hkllekjc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iqzxxnlc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zpdtqdnr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2adflomxs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2xcvacqrd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ufssuxpz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gpeshvnt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2aqpivfzg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2krvkmgys.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2jcgcpsqx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2kjiqxfnv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2zerfmqri.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mxltsagj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nvgzkros.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2evhqdkdy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2nslrasjx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2njifavce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjpgtdtv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uarmqzkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fimlmpok.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ealgdljs.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2liwhcmxg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2bnaoafom.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2compwtih.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gttpgvbk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xzgcsgra.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rmjujszu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ytxwlvxv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2uacybpmt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rovxeomi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2grurvtmf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gdizpnqu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2efvsallt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gtcpubbn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fzcnojol.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wnpctrgs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2aqmlfyrh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ilwveadp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qazxclxx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iwzungjw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ingfypkd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2oftlelmd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mdhscqez.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2adqoewyw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2stoqydmb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2onsospjg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2uqgetbpn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wohtmksv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rllstggc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fuoiewag.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ijostkxx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2zfnlffru.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ugvjnrzu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2enbmusmx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gsprqetd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2sdwhuhaq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jvxbfvhy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jxymphpb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hjudsxes.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2spurwecq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2viuatwoa.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cmksjeun.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hfrvewbx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ijwlupsu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bhuazxpb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ovrdxnlc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bkeximxf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tyqnawsp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2sfdjyups.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ntaqvydb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cubqzlzy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vrhrnixa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2htqcguwz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xzfyhhzn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lqzzlilp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2rvnqnbea.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2lxwrikub.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2yvlqelnd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2twjxwghf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gtdghqdm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nngxzfqf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2egyqiyvu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gooivanm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bppcqgbj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2azrtgvuf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pnjvhbjk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwngbunl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hfuvgayd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipffqryq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2khizjzxf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2csvfwelv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ukugdufb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yrrccwdc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2aiktnqhc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ibzfqizf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rjswgeoc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2velzwrlh.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2vnmdzqfw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vcbgdpbb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mfmuegsk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jxdasvcd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2xelniykx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zrjurhzh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mdkrstfd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xrfittfh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2xcpfheng.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gakrwxuz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hsmpwqza.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2mpitytfi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2pbgkotdn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2mejyadzi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2uloofvdj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dzlqapno.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ebhzwqkx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qbabbwrd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ajpldtji.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pdpjhedr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kztcyuad.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hbjjntsf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kgjacpwf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2osixlrgb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2iolfhkfu.html


<!-- 参考信息 -->