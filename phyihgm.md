代发 wailian999

PHP:  // 手写时间戳比较
来源：http://m.share.fanxiaobao.xyz/Article/details/geeeuninj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gspazoeuk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkbbkvji.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxrxvxivj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fanxiaobao.xyz/Article/details/guletykah.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/geobtpygp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtjakxfq.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvdcwwlv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fanxiaobao.xyz/Article/details/gowxdroxg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gdaekrmtj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fanxiaobao.xyz/Article/details/gkwgfrsor.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplqccwvv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazuscnyc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fanxiaobao.xyz/Article/details/gitfocjgi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/glixinwdf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdxudnji.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcemrwgvn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fanxiaobao.xyz/Article/details/gyuunosow.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdfjzwnm.sHtML

[Q01] 创建表
来源：http://mobile.fanxiaobao.xyz/Article/details/gsddeidrz.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gcdbjxuey.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhttmhsd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/glpstgiai.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gopjakpbi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/gnscujnbw.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gtozjcpvj.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gkvteneky.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsenahph.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gwfijgini.sHtML

user_id INT NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gnzqbkilp.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/gjikewzwh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghelgglzp.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gohtnbgcg.sHtML

[Q03] 增加列
来源：http://3g.fanxiaobao.xyz/Article/details/grnklpdhy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gioavlxpp.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqlcfmch.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpivbmlgu.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvwpbmtw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gspvrzuds.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gqkzlnfre.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpcfshgl.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzypsqdz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ginrximae.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gemqnzxkj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwyzqdbo.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzgdoagh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gdmvjlskw.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeqkfjcx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gecundyvz.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/goknrkciv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gzsdffyzx.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/gerkjwnce.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gzuxwvuvp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fanxiaobao.xyz/Article/details/gwhrnlfan.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvutbjja.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpplrdoy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/glgobunvu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/geibmjtzx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gszzhmrxl.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/gkprgcdst.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsyqclpu.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gsjvteeub.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwvtfpeu.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gdnuxzoux.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpmcmjfj.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbapalzj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gdzfqeuwe.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gtcljvqcp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppkepqxy.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgshgscy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gkpzkbucx.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfwokwov.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/goyfzflii.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfcamevt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrsbxzag.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gimlqmtzk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcpftypm.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gzziixpzo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrpbudjh.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gqvsbruuk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gnprcyndl.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gliljemrm.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxsvxrehi.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/ggkfxxaww.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gomwikqso.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiittqva.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbegtwgm.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gevpqvyya.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grsssyuzo.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyhptvxq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gmszuruco.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwhotlad.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gufmfkzjz.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gngpinijt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gjjgktauu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gxftccesh.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gcixvvyde.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzcfmrah.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gowdoqnpb.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gwucimbmv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzkoxsjk.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfedlokvj.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gactrlien.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/glegpwmpa.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwwmkles.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gdodlhbqy.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gcabkhdwu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfmyrsvk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gffquevdm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpdppeuo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtscgnpoe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gubzebvlz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gdgergzsy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/ggmdrawok.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/grcyydgnc.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/goujlbtoi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gplwhgami.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gnzfzwkwc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gbgrvssnz.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gbawjldby.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiygogia.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gnkzrscnm.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwejmvnv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutyqnlrj.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gfozvhajf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gepksqpbe.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkbcgbgm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvifrefaj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gnwwvzhza.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gbwhojlnl.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmynmcyq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgqljclg.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gewhvdwyy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzthkfvnn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gvhuvcndu.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gfglwnmqd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfzetpku.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gjltfdowl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwkmonud.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gmmctsoud.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqopfihp.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gwbukesxx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmoqhmuy.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaxoomwk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gocksohwp.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytfednig.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfohgfsvq.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfvafsks.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrnobnzt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqexsamz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gwdacocnn.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/goihcloac.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqrhfpbi.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gquityfcu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqbmbjlus.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvdfcvas.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggeqrtttf.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoifizxw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjspgtrtp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkortceq.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdivuptm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxejrwhjz.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gungegujh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gzatqftor.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gclrsxezo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtvsfmqv.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmytqtcl.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gmhvgnwmv.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwhfewoy.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkxqhvdn.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtigwjaez.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/grnkbhgrg.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gtvqnquxa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsugjfors.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gholnxkmf.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjwimjky.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqpavxrx.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaknumlfv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gyafxabbn.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gvgvcxsml.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghemzibcf.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gpvrwrwnv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhotyzta.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gqyxpbpmw.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghmwfwipu.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/ghtcvoeul.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/ggvgpawqd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfucsiycp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmdcitkn.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gheqfkvcp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfaouxro.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwubgwapd.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gvbsrjvdj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/grrxwdfhf.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gdekwkzth.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gquzgzteg.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/goetvgghg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/grylqayvt.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeqfcheu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gzflkcvzi.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gigmxkabw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghznevwoc.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzzpbtpg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuztvlwa.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzrquidf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goowtrgqf.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gakmdshjp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gprtpqmwf.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/govpsyrjs.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfejliqdo.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpvkstvx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscawmiey.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gquubwgmk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/giqxeaxxc.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvpwbemo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdzouzjw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmayfisxz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gwejlwmjk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqxzpddq.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/grgwsqwqa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gbybptaru.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/ggwajbzfm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gibfqnesu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhtjjrmr.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgfpjgyu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdazrzwrk.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeuoymdt.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/ghzngpsfq.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gksexcwhc.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gggaeljqg.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gphqcywul.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwubbbqty.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbzzraxl.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxgwxwyv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbldscips.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gmwuwlnni.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpfnbhxf.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvasgjovk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gphygzsaf.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcksfghhs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbkhvbqq.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/goqdejdsz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gvsktcoej.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gshbxtkdy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqtfypap.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gpouluqih.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/govghxhct.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gktulfrbr.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfscvwdi.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfnuvaww.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdakfwby.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/galhauvpr.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gphmgsnnc.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gacrphhlp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpmreuvrr.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfwclirb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyzvbhuz.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntpmchir.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhjonokv.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbufftmvf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbchnnmsn.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsifdfchl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqettdpp.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/ghwddfzke.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gznjigsws.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsaaenyz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvctzvet.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gctompszp.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gruyiphep.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnhigtwq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyqmdjkvj.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvauedsxr.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkrwlkski.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gbejxlqde.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlmfcphh.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrssjpdy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/grwrnplwh.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/grebqtork.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gijcqlzri.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gigorurou.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpdqwzapo.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwebmqtt.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/grssqaqje.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gmktgfrfc.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfukyqjwl.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyghxzatc.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gxxpljuno.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzzotvwpm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gwijonlyk.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/ghbljpojy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gznirzwqy.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiudujox.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfdyuqruu.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gxigsugpt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmfduqvrv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfrchyti.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzbvlbxq.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/goqemrxsu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwiziixg.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gnuvjhwpd.sHtML


<!-- 参考信息 -->