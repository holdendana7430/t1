代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3tzkupfmm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qhfyhvyh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dmwqpibh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ranjsuaj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fnaxluma.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3btiqlbuu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3wcnenxdi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tzcznrcy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3cvngvozt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3asvjliqa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3yiezowbc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bhjmkfka.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3cihibufh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mpxokdgp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wfiqqvpg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3aduhopka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obsuefxx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3zopppomt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pactxyce.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3htdiiopj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3yrygadqo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fugerats.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ntgorrpd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3fwnlbcwx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3evnjhhtk.html

);
来源：http://www.52xcode.cn/Article/details/gt3jhiaixcl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xckavead.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yhdncdvr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mruvvvuy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bdipubdi.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3lcrzadhd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3zxwxywbi.html

);
来源：http://www.52xcode.cn/Article/details/gt3xiwuhley.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uqawtmcu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kbfvfnsm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ewugghju.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mmxdpndi.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ivqbkwhs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xpzrolbg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3alcjtotq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ecwcrkqk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3azjcaghh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3tahjbfjb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vjzujezi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tgdpjpfv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vzyuavfc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3eeycxkyz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3afhwrccr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3avgojlez.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3payhtisb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cwvibphm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3emofznio.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vpuyywvw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3rduyshvi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qzprpwmq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3whtxtbsy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3gzyfkavv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xgxjtktc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ryekhpag.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qqkdbsdk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rmpahumd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zpgqrgrw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ousecsrk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vsiiludr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lpngbbxr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3twteurod.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3teepdwhm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ovbosnet.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3rydjdyny.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3cduesqtx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oklyxiqw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3drdjftlg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hdsrkpxp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3pmobxyob.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3nnqbdixu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3eirplhak.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3twidkskc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qmrylmkx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3buoivzor.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3oiesualr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3jxlubffp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3obmjwxtd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fttbrktt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jhswcjqd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oesqgqze.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3pwaqfjdj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xuspqbrd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fvxpgprp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kutvklxc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3auvltkjg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fghzyvqe.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3eclyatlx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fgvigyao.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aulfecah.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dnbikwiq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3dogkzdsw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3orczzctm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3aexmspoo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jwlhwkay.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3biexjqco.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3cskyyozy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3juoccxtf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3rjsbiaks.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3aryysdjz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mcxzpiyp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3spikmzts.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ppkdkexo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vvbzzjcr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3yknwzrru.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3awbinymh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3yugqjifh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3idabkfcm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tvwlirap.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zklktjig.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vnzhyjpb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gpirhamc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3fkcmvwfm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wruhwcjd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yclkyeav.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3kbxooavy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3uylaqykw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3chwbxnrx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ryoahkhq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vmalfrjp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3azwuuqgl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3plnbfxjk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3byvezdrj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3souxvsdg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3hsxofsfd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3owlqilxx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pqykappf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3mosnjsgv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3arhbhxph.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jnlrehxy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ljjneuwr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ntsdojjo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iheaesfg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hrodjkjy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nujhzfou.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3smtfinic.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gabvrvzq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mvgkqoin.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gjdvkynl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3wcyeuegc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ibvzwydf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3giwxxyyv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3fchaogci.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ujpjbtjq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qhrxsbxp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mphjwzlx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ynbwylnb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ieqaouqy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hhcrromn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3njkqclyv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yykpbaae.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ksjgvrlg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3raysnmgk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zobnasjv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ryczybut.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uxvlaxow.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wmvqjmrj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3snvxpiux.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jknxhbic.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ctedbcgn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nngeepwd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qvvvtibb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xteawadi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kjhtkopg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3uoilgmhw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hiztmlmd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dncgwqng.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ubfkxmwd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qksdpbaz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lvronfgy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bdptudbo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bzesjywz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3rbzxbapl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3cwsyzjno.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xngoyebr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jolyokcu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3upinlyqj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3kuyirhki.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3qflnobva.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3arumuigv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cqzpydlk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rurnptvy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3nbznvkwr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3tbltxbju.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3kfglkepl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gnppwfjb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3giepckym.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3kzkisewo.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3yesnqzak.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3adcecnaj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ctrrysgt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3bfccvepz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3huaccmoy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jdhuixyr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fdggyeno.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3egcntgfs.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tujofrzu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kenqvxgb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pndsryap.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bcjssqvj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3bslwdzvl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tfybqhli.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xukfjidl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xsbdctdv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ppcrfyej.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rotmgoip.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jkvsjnim.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3unvsmjeh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gybebaql.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wxcprulh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bkopghtj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ysmyhsla.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3goruepmb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3pcceoclw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3birvwrzz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mvrdejna.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ovxceslz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hpigxthf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3xipsaybb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyvxytxp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3biwstgdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cybqoipl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3vfjcfhsy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tgynxoof.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3gjisjjbe.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3gyzvdqku.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qvrrwbtj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3vohhambm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3fjxueznu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jvbbqfcd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jwrijvcu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3esyusnjh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qlhbkevp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zhcxraxh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozbjgbdg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3syslnfrm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3myanchbq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mvjynskn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3bcvtbzrn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uccrmhnm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3iuhhbcya.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bwjzlenq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ddxnibjg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3amxzytik.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3shvmlafe.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3inyydzvv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3znduenaf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3pydumbhe.html

esac
来源：http://www.52xcode.cn/Article/details/gt3qzjoflgj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3sovaiokx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3olvaaylo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qfpiijgf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rlnzbapw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kcrvudjy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fyuqmjje.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfgynjvy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jtbqvprw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xjjoynei.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mkxywlik.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bzhdmnnz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3oamqxikz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vtpjddic.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rqutveji.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ggvtzgid.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ebyiuqen.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3onioerum.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lojonqqa.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jebhbixx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lutyuhft.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ruwbnkgl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3pecqnvaq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3twsmvqdb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mzdcbjms.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ultfkpua.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ttahyeui.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ayjrzmjl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3umovpegg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xoahtozs.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zpklnvkd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3eutyihvn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kruxnolh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3wvxwpkdv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bnysbupz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xbffeavi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vazxqdbo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gedlpugr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3yqxitfcp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3lnlgeufa.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3trzmbecd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3pqkxyief.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sadaycec.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3nwekjhaq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zrkfopad.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hgqwspfv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qiqrdqub.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tckxijkt.html


<!-- 参考信息 -->