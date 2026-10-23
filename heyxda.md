代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mfrewraf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uyoniqkf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3mwoyinrt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qsdymcqn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3galzmuvf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wafytbno.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mnfxwihf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3tbqygzlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzptxavr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3zzhtugzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqsuilbc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yojvvtjr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hecaoqxj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3byxiwayv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3crnlwdex.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3hentdxan.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3oxdohdwx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tzsardcq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3btgtspdy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3tozflbuy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ilzispjj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bhvgnayk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3xsmbvznp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3sjttldxz.html

);
来源：http://www.52xcode.cn/Article/details/gt3uzzxcclq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3wphdwwlu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bjkicwrr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vqdmkktz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lbkvzzec.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3tbrcepxl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vqmedmxq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3azhhbvcy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3uivxnwqm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ostsnvvv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3qtvmtwwe.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3xcsglmzt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3asrfuack.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3cohdwnuq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rnfmowte.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bbezhtrs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qcvkbuap.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3mzbpwpzi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oknmfdbz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3kytbgyit.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3viwbhezp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3whdffyhs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3oagszqze.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wdlcyhoj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3mvflqxru.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3abahvixm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3kvgeybqi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3pcbfntph.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mzyryhhn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3profrthd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hkhvewxn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tdptvyly.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ikibfajt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3iwtsatir.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3scbofqcq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3apvzhaiq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3culijzda.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yehjxtcx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3jicjgoqf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wvurstvw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wylhqarr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3veusvijs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3kbjfysez.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3rjdwsqyh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3kaywjbil.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3cjzgeswe.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ohnkoygl.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ozarjjpy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jrjriqgq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3sdgarpzt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rzajzftd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3lrumtawz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3inmxznho.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3axvzexcp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gkhhcnrm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qulwyqqw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3crhxaxmq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3fmpmcxlt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wacwxseh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hmzxdrbk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dirobkmh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xfppysda.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rkhawtuw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3jcjsyugk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fhiqdqgx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3fyhkzirc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3qgzjnmjt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3hrxsuvbr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3antovcry.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3nlnxyqga.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rlhfmdbp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jociyvhx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3fnzvaola.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uijkociv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3yjkirdyo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bcxhhqie.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3pwoyjmuj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ycrzmrnx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qohvqmrx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ayncirgs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3qzwpmbys.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vhgmbkeo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rhodorwa.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fuwayvwe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ujxrmyzy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3natvdgmk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3bablgufr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3kmiqmdju.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3iqoowvmf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3kfefyqfk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3dlhwkhhg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3bmqfchru.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3gzjntjeo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3emfluihe.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3fasybsyp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yfrrxvae.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jsydgkdq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qmmirnxn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3titqqfto.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3nybwubbk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cpsyyicz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3nbosnzuq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ydhasobl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ydlobipe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hlvnimmb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3sofccohf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bsdmsalo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ceiqcixs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ownxseon.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3etarjcvl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bmogwdeb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3syekjtnq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nqrvgpnt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3feybogma.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rqozrvud.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gxvqlcdy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fsgcxskb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ajjtajxc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qsprphyf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3oonkeazm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uztpomgh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3llxqchdl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tinzfxef.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3fptqmopa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lkuezult.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3vuwojusp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3sugejkop.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3witujiyd.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3autsnlou.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mxayline.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nydcpzlq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qhmlcdja.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zkxblmto.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3aguzkkln.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pojqlgfo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jfetpvoh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3gguojbcc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lcbujlbx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3noznzoka.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3mzrfhxvi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3svjbpqki.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3btmxkxbt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3pumjyykn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ecoctlff.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gofdkkce.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3cvxhxjpz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fwwcdkfz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3gvepzxyx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3bbbcohtw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ulaobxee.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xsmuzfdz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3yeycjxel.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fzuqwpnf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3dljximcp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3zabgdqpu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3rkgvwgrd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qwnzutgu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sdqlveuu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ugpcaxvn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3muojxkcw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3otsgsdpp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3spvwtsos.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3sdtqoyue.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3lhifagbs.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3slrpooce.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3dtnfrkxf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3oewwuwde.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3sqyyaelp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3zfztspue.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pccvtebs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kfkusfpa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iwckhdmt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3okbsdhrl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xgwlypck.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ivuizrwv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lwzecwbc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3sjregcph.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qgkraovj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jzeojzuh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3pwssnnqn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3tjfkeukc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3yoeeihyk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xvqlubhw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3zcsidftg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3esyaxlia.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3oiktvqib.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yuchrcwy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zolcptmr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zayvuiho.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rsoeeffs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3oeweuznd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxdujxfr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3dshhfjkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhsbtlib.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ckxdjvzo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3txmbauvp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3hvvlfpao.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3gtnppmkb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hplzvllw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3fylkoufl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3wrmqqhaq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3aagimwaq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hyvkmdto.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3yzmbtozx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jcestjcw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ilqqymsg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkqtetna.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rvgdjrhy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ppjpqdpt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lmnuzhbx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xiovlwcb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3myzxcwyx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gkalzhpb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3jagonutr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oqtodlyx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ggpcqkns.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3jdtfqocg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mmjwshzk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zdibvmqs.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vpkshffc.html

esac
来源：http://www.52xcode.cn/Article/details/gt3chiocmpb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ouzcyopw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pqbrlhsb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3waoomcuu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nrgxufwd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ijxvcgfk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3iuaftofc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xzwbjesw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3iubyipva.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3pxxijewn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uyodiwak.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fgzlycdj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xqgblxat.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3svxyrmwt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ybjsjxtb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mdbadesf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uiiutodl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3nyfevkjy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hfriecpt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vwlukwtf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rxxzxhfo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qvxexaxq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3izafpgeq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jvewusoa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3awrenfgg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eunisylt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3sjnsoaas.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kzuqxdez.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tabasjar.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3iqgfahgo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vhpddivf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3iwsiyzjj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3gabpcuqt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3mgfanocd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bfskellw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lmgkfcrj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3todohqsu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mdjwfeii.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3phtogjrj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jnokcfig.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3wgvhxeha.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3mtutzzwn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cdynkyda.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zotxoxhh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3azzeuaqk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ziszjcry.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3saageeok.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3knzsdmgx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ofojrzij.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3yrwuucjj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3bdqobdfr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3eyanrerp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wawapwdc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bmjtrilq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ygodgynj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3fdfukuhm.html


<!-- 参考信息 -->