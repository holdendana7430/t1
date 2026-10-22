代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2zmqyesyw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2elqaqmpz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2oombfblh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2pmhkimmc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2gurlemeh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2deehjowv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2omedwrnf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gamiqhrz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2baqpvbdp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ooavavre.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ylvslgux.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2zmbqeagj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzjlxqen.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2piulqfbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwslznzv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vxtmgjuc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xrqxtwav.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ycacchfn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2onarxxqq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zakicsnv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jqdfzovt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zrzbgiij.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2bhtgzwhf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2qlzpgesu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qatikvvg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hgauxrjn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2yrkfkaji.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2tcifngsk.html

);
来源：http://www.52xcode.cn/Article/details/gt2uybeftzp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2iwuxksmp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2dspmkmzh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2rkkihgco.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uanqovkv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2pdilmqfb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fnhasbee.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2atiiwjyg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2sihmchca.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hvcdcxok.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2purrbacg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2tabqnifo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fdvtetfb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xglpwxra.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hvnspoph.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ceikaexi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xbwwprvp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2qtaakpaa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wbbmcnek.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2xzzlgmiz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2afepooge.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xughdapm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2uhxqzjjw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ikmrlhql.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ibuhoied.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2carxzehw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bhmdqwhs.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lzkpbgkt.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uirdhzfi.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2nispcyte.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rrtxyatq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ykmgjucy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fptgwovb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gqhkxspr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vjjkahfm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2xnxjtwsd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cwcyhezv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vijfjnca.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zngkuuzm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2psxvwrwc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gbbelqsa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ijygnawi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2elneiooz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2htaockml.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2tjzesdvm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mcgcqzxx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pegwxwga.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jhjdmkws.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zztcdqcl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2nugeqosl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pmgcvxwq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2brrsfchd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2akdkgknp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2szqlxolw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zkwshfiq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dmeailor.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ohixrwal.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tttetnin.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zxsyumww.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2zayusgwk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vbryagts.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2sebaqvht.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qhqyhmat.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2odoligae.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ngajoxjv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wihbatba.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vehzihzl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qwkkufhv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2cbctnxfb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2udympmeb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2gfqllwoh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2piffsdkc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2llpffrbu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ttbmvvjy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ainncxkg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jltezoka.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2llaywnry.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nzlfwzoo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ltndfeys.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xpjphviy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jpmkpevu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2uwjnqymg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vmmsvyzk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2yjcapdzk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qklcbujo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2jftkilxk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wmmiwlhv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vujrismy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bzjpihkq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jopfookp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2syszipoh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2qbkqiyii.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jfgjzlbc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2khppmwqx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2hsvbbwmo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ojflekxl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2fhtjvtmb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lemjdfgx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vhlfrmpg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2mcgxjahc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2enmyziwy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2mbedsoyr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ldmpjepj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2texapzzh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jkwyizox.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2eqhbqewl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hpqiqdon.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2kzvxrmif.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bwgkfqcg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mdjxroub.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kabjjumg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fusloeur.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zsgmjdtw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2onjrfxck.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2acrkyitc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ehyyaxeg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2twgoztjf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2spryxemr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2negkbrkd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wmdfyxjq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bgdzceyh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hyojvyvg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zrvwuubl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2misnpjbg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2evnkfwje.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qzeyzxmo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2otutlvju.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pvxwewtg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2tlbiersv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pjvxqczy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2vbzezmcc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bqeftbwf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2deooysgn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gwkbsnzr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ocoqbmml.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2twijnvpa.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2qwdtlmuk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2lywfiytp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rwxeszcg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xgzuaqlz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zqnwqlws.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2kroohpgk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2tcnojoqe.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2iwfqbkcd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ahxnuhcg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2thzwletw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2dzafdyps.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dravocxj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2iiwcklfk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2gzbxybhw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2kabmckkv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ryjjyjeu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iaqmfrnm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2akppwegb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2sywguybi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2tyuuvnuk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qmyylatw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fbgxmuon.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rxlataqx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2srmrmrpr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nrpufngu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gessdygc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2kkmdcsew.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2hokehhoj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2etbbeoyo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2utmjploa.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2crpskebc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2abrapuva.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xbfeuscj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ujrjlfyw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2njzchxes.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vmwuwvwf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lpdeysyi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fyhcgcyv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hetdnbcb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iasiqrxg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2dmgeyusj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qgrbrpgg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2lyoubqja.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2vklfnpzz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ovpnrgcx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vngijqvl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2kntlfsez.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hifkseta.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2shmsqnup.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qfeeeqtm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oblcvhvp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2teawtswg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2otvdebyq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ghhpocjc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2glmrwmsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmwyshae.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kchfalai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrkxzdid.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2iqlafdbh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2czgrlwno.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ctnhqzib.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rlhnzlxd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2drcznavl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hopascgx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2iuynradx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mfsiamvc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ggstqnei.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rsstyccr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ifngbahq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qmpjvfme.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yzryhdid.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2mujolhjk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2komzcldz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gpricdgh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dancuxkz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ksdjcwdx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nsbnmrna.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mzcjccnf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rpclnzcm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2kidxfooa.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mzyeicet.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lwdlzcbj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ueejldki.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2plkgabsb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2dskphhfe.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2akfvuxhb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qbsvtzap.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vekxmfxh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gxyvwlym.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2saigaokw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rxvvqvim.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rxmjrvna.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2uitmefsk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2jnbcrkfr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gtcmdyqr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2owcxmnjg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vmitmgow.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2gjbifyjw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bgwschsh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yxddpezu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tvbetrtu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tcsgmcjd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2veeemxla.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jijxtqvb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gbcnzknj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dclxavef.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2begkabsf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rihkqkyo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2eouyhryp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lexhcjvh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ihhjvfjg.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xbwrbmgn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2bbrrrqsw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2sbazwtes.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2uxcoilel.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2nsrcjokn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2sbribbde.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vxwvhuqg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tkirkzeb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xovkpvdl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2juhghugv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kmaswlmc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jjiwxuwx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2pnushobh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmlfowja.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2avvttvty.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qikstmum.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mlscglvf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wvnomdwg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dorrkypf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2iqaqfapn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fedufpai.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rrsegtzi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zdcsxwll.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2yxkwklpb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2vbyojoed.html


<!-- 参考信息 -->