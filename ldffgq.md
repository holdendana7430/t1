代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xogkhuer.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ajbqbdjh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wolbnxug.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3efxrzmha.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ilzmswaa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3nztcpikt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3pgryrgri.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vtzovtzj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3inqcefwy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3aroxurts.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3iffamrit.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jlainbyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlohgobu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3bbmoitnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhkzjpik.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3puyytrlm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ygxejhtg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yextlupu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3izrnbmgk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gmnmjgzt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3tpomhcio.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wfvysitt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ylknbbbr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3qaccmqtg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jaqhywzm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fymtvpup.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3kbdtuaxu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3rhnuoixp.html

);
来源：http://www.52xcode.cn/Article/details/gt3aloiqbki.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3adwelmvz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jhubvlrz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rsxwvfsf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3altlfrja.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3fomqyqei.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ilvnstja.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3giqcppxu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3jbmjwdhs.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3yovuhcyt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kobkcyms.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kucpxwrk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ddoyszwy.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wczwyxwm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nyjbeuhm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3huytrwwp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sdftwrpp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3xljfpuyj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bfwszeoa.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xzikipoq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3kyglcdhh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3izuktyte.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3prtmkbuu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gubxzths.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3eqmqfodu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3kqdsuidc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3eyvqaeau.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3leptlhsf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vrgpuitr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jzkpvlnp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3klktclbo.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vsgemngf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pannymym.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gqvjfovm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3exmnffqo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3igifwknm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xhmavbcm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zexdbzee.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3etrritge.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3tfrpaxnu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3yycbmrqk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3bqmbwlwq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yfovyyua.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hytpkcjk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3cyylevqs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3muygzbav.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jwtpisfp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3bnzznpre.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3tctncelp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lejsrwmt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ilozapyh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3fmenlodo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jtqjkxjo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3beuoqkeo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ntnetwjz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fnczuwcb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gptshebr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ckzzawhj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3sxverhbl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3wuarqlsd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3klkrgzds.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wzvojhmq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vpaqrdyv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xudiknas.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3rimowrvy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3lxweacfw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sijyqsvs.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3kuyivaal.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3utfzyusl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gthlwwkw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3enhhbqbm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dpwjpuot.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3sdttzptr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zlcfxfgc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3rlshqlzq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yioyhglc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3lrkbpkzb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zyfczrny.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3bfpucxlh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3fdvksvtf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3cjobhdoy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3iudrihsf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3txwqqoty.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3vxlstkqy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3swcmbbiv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3sqhioald.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kiogqeru.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3oigtiref.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gteyppks.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zcwqiwwu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ugnmnxug.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3wmhpbxys.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vxrhbzjc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3xpdgfbof.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fliotjyd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3danndqrm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3taxtpikw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hfctmbsx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3adrxzcxd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xmaxgxkc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zookhfqp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ncxixvht.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fobgfisl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3uyyftycx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xtepilde.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jbsohuke.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vpupsltf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3oikrdprt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fknrpmdp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vibasppu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ztcyntps.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ogktlinw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ojasmzdv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zswvwsre.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3olbnntiw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kgnguxtx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3icuovbjj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3lkrfrabg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xkhglmls.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3krhtucqk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3czhxpcmv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3gnkyypwm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dwlnhung.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vnutbxlx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xdqoygob.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3cgyaucym.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kvlbsxlb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3swcnggcq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3fiolribl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nvftboja.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ravdeajc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fvxoddoc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jdcuqwyw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jikxfnfz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gbsfoqug.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gbgaxngl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3rgpzccll.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3nycbdxrh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ipteiyom.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3bxtrilbf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3onhojzvp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hjidlbvl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gkaxcokb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ajxmlzqa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wgrywqrv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3hsxosjsy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3gnsmsosj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3zbgpapml.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kumysmbw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3pgjtyztw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3tvdcfmym.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3mgdchtzn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dvbeawro.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3dbeafyyo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3okrtjzwj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3sxgiohso.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3xrgfftzd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qjqjguav.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oirirnja.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ilnsnbkd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3typhdgcd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rioelbye.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3wwkziqdd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lydchvrn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mrmtetcj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3tqludehm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fktxtcie.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nlmgywxn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3butsaclo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3paayysna.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3iqtltpow.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rnwpghfp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3mktjyaks.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wjjpgdmg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qdhqhxxt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hktgyznu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3slibjvzl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wvuecyod.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ipkeqvid.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3cachjosw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ztwqpdsf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3kkvebsdg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3gjzgsksd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3zyaixlaf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ssrhvoxu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lhqmspnr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rjbgcesq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iscxefej.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3meszewnm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3railpzfm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3bmpmytov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlcvnnhq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nxmxbxdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgixwelb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3kiracrew.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3smxjynal.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3jhejezth.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qgifacrt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3adeavizl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3nlktkvbl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3wkgshhdv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3slaalcay.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3wmiqduiz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pgeqgayd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3crmjamsk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xfvhkapv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3csbbbpur.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3yhkkfrcm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3iqagjulx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xiukbygp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tkejjfoj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3eswzyqef.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lvhwygqb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3cgywozhf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3yhoxsqxp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tkitcxoo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ulxwgifw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zyeaevam.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mhuscjts.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mhkbuztj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dnavjgzm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3tjicytoc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mwbltgdn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qlfdcfju.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kroikchb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lpexthfp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xdinyxqt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qsphebdu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qycrsrvr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bdnaclro.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3toltnhvw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qntjmskg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jbywlhdl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3csrhgouy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nypcilic.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3erohbcza.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lyxfdjbd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zmzklvih.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mviduexa.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lovwsbhj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3oqltnrih.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rmvtpfev.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3aikrdgop.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3txcgerzu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rvuprbwi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qgiqdmnm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jocgvypn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qbreawre.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3yueparhl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3bjybmuxn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fijlgvsq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3nrqzxeab.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qjwjdxzx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ttgzbzmy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gpasqfdb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yijyfjnn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3htbpjslm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wfnuzryh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fbicivps.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qcetqonx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3gtrcvfbq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3swazoyfs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pgkyhbsj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ihjuogfa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3atbgfhhq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3umaoxokf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hbdwejxh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3acpvdmqo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3lkrltepx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3lifhaezf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3mlpekmud.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rtvwecsx.html


<!-- 参考信息 -->