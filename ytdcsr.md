代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2cnqymhfv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2huvtaofo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2pffbmwbp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qdvwyafv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2lkainfpp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hnxpaxnr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mdyuykne.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ysngufme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibvrbipx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2mibqaetx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhkyzcfr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2tmnjypgb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ovzjvrhn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ghofsoto.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vbrpprpb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2timlrvkh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ceeqmfln.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2suewzfxy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vonkxnya.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vfjgfuji.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xstcdwlx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bmlzclbl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hbakphbr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2favfybbw.html

);
来源：http://www.52xcode.cn/Article/details/gt2xkuuzlfy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jxrprzup.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2bnpwwbju.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2njackwba.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ybflrraf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kgcaqfqx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ljortxqb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mhfzdkzg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2jnjmcxpg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lhxccias.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tgbifrlb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2stwyqqbt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jdhsrinj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2waclvjqv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xzqmrqom.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zviynefa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lyboswrb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2mgdiuzyn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ucyvlhpx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2faijfyam.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ruynhylm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2nkqpoopu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zperjvoy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ynmswsov.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2viaokdoj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2anogoryd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2srnxtpvm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2eamsiord.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yjwrxheq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2egwuihqi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vtfxahrn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2upgzcnta.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tretizeu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fmqiuxiu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2myfmnmuf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2dnxouypv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vsvhllpo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2neupnzhm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2flmlubxu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jxdfiecb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ppumcrca.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2dfwzeqyw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2smnvnozi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2wpzeprmz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kqbtptbi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2dwkimrfd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aghllmij.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kpxunoab.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ylwxhved.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2tnntephn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vzkfovjv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2payyhfqj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yccqfqtc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2klulxxtx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hzbhigmo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dnoxujup.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wvozwaoc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xidglawj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bdbkbfuw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2zvkaqasa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2adxauqbb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pkgprvgb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sizjjhjj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2asolmdql.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gkelczgx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2aavvxkxz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rumtosdj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2clgvzcos.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2niqzqhcz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fqzbpigw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wcdxjaik.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yntzfykf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2qmsfysbu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uxmiehou.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2egpphzsh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qgkbdkaz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2guzeblpo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ysnfkfer.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2psozomze.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2qyyneejy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zleysykq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2rcmjqkwr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2oahtdize.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2rgsnxaxc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2axookfup.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2eympdgdj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hqshauux.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vgaftcnf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2plzxmuhh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2gxrwxbao.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ngjwyzfy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ldjuyxup.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2zfhgmbfq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ucysyhlg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2hbqngvnl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wwxblbhj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hravmzma.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zgvvefuq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zwoqqggs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zaklacmw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wgsqjyvk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2apxwdxtt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bmdsgqzo.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2xzwqrtni.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ofkdfowt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2btoikpkg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hxwxksls.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2qxtqnmiu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ivioqasp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2kvydcepq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tankktwn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2nhvtntgl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qspmifjo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qzvhgteo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2yrjfogky.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pmndpwib.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mtocdgar.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gddmmkhg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2guhstkgl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wuvznnul.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aghcvgej.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2eumxfzrx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tuvzejch.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2yqbpqjch.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bspnpimq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2euqpauig.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2jrspltnp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bsnobgsr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2papnncny.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2snympdvl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2tpfrgvuc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iiwlzfyr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fbzmrauq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kzmcreak.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2mygugkqz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bnubtqwf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2svkjzfes.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zgwjqylx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ueeppjvv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qkaywkxa.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2wzokubsu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rbcqlmqi.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2maazymrk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fdkjrryz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wbzfysqs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2fwqqfzqk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2hkiubnsg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2rldljqyh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2tbfyobsr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tsaftwdp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2xbcagtan.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2edsoqgej.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2edatoiyg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2waljpjvf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ieqiufii.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mhoaqrgz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cdtzutye.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uizjyqgk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ncwkqskq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2kmzwulln.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2tsuaozqy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2hrkcdkdh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ygdeuvnh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hterlmni.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2afapdpqd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xtnbbzwe.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lhbrohfw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wvpymhzp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mzuxofva.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwkxjwud.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ejrdamef.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zmivsekc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2zqnlztqz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2liewearp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fxtoqkja.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uqulsafr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2tshyolcz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lxwalgqv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ugyqjhyf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hstipyky.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2pfgzuamp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mvxmezmy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2enzlhjgg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2fmmjownp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ndriydfz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2suxgiizn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gvaoqivm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2hpiamwsn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yaafdsmf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wfjftwnx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jfqsxxaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smzdhddx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zddpxfkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgxbmuvr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nrjzxaze.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2uvsccsfg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2npjbieqy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2vjdcbmtq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2hynyqyvb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bxzcpvmz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gcgzoohk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bbpsfevh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2izufnltk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hwrdkffx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qqdoqajj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zwuhckhr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzzrgogy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lepvifio.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lwvmughf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dmgzejpx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tigbroch.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kmrpdktw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ualjibco.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qltbcyxm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2frgtauok.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2pxrndmbm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rnwxvvza.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hgpfalzq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ckjjawdh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ljhvpztx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xkxatsph.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2bsxqgiqm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kmimpief.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ocmlusqa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ltxyexnl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2eelcvkof.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gqqnzedo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qsgsdadf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vmgezqxc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tabzuclt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2orojpvrf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2pljyrkxq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qtgdxomg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ldzjtbnc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2idexcjys.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ktxxrxif.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2woagqsyy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rndosrgx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2kzfwcmrn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pyqwdhnw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2fbrsofgl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jcxijhkl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hmngplyq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cufgrlyi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ffxpkmyc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vigsqabl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ydkaemop.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ihtygixn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ycortsyg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ockmvaub.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2shslqsgy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2utinrvyv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gqjgtras.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xhprwxwl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2fanqezcg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xydglyxk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xfrulybz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2iwbbstoe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ykeimeuc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dnhziprl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2waopyirf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2actjleba.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2secoetcs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2mzwvwkpq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2smeibqxy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2flmyqqmz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ntgwnlxg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fhunommn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wtroezye.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2kzfowszj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hgveokke.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2aqelmkqz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehokxfgq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tarpkakc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bybsuwbe.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hsolfsom.html


<!-- 参考信息 -->