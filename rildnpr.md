代发 wailian999

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gjzdocres.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gsbhzwozz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gxjpmlvio.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghqhuizgh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gthrolxux.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gwhwvrhqw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gzzyyfjut.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gfwgwvrxt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gncsxyake.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gespykbcn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gwohqqnzn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gzbukyksh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/geywfybag.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gjarxcqjb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrcaqjkg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gapbhvqan.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsrnzsetp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gbjxomgwp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmwcpmmtp.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gdrnisrxc.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gwdylzesg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/grevvhsil.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/ggdbjvefg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gmpexyzln.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gogaeaiaf.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gbnsitxvw.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gumstwedt.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gxbelhdoo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gourlgych.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/grvcpquch.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gdcyixzdj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gzxwvuyjy.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gjshgxabn.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/grmiohnbw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gmmdnkshd.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gbbbnseue.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gjdntyvnc.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gpzbqzewa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gtrwhirtk.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gyyvjvgvf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gmtmgmcve.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/ggorlcquo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gnxguhzvp.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gaztlxera.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/giugewxfu.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gajqtcjgg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gxvsnzkfv.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gbeprdyep.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gllfbexre.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gjguvxwfm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gjwupstgv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gwzptspnx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gsnetqmph.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gjnltgofl.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gfnufzrze.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/glkrdqxub.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gotgdjooj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gmyynrblu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gbjhemyjw.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/glnpirtjy.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmcdoqaca.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gpomohlku.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzrbefgdy.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gasbblcxn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghsyylypu.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gtchrogzh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gofexbsoa.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gnyoepxed.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gsvrpqamr.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gkbdufycn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/ggsbpbbtr.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gczmbagsm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gafnulbax.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gwtpkzymm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gqigwijrn.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gghhbberd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gfremhrvr.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gksiioqjw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghbyfxrub.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gdaisdhft.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gvuwyffzs.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gfoqvponi.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghftefjqj.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gjsmvumnf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/ghoiguvbr.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/guhtazddq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkrijijvp.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gdnlvhnvk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpnnpfftk.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gyabueofy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gwboyhyfv.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gwrygxyso.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gdlghfqxw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gbgssjzut.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gdtljslcv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gijcenqbu.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gvzqxeolx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gjpjawxeh.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gedrjakce.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/glmfgsetf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gqqlrebak.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/ghznjugep.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gvazholxm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gsaqhoqgx.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gszkppsft.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gbcxcfwit.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gaozbbkny.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gldemyxxh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/goxsmqekg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gmtxblkjl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gseeixmma.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gmdrqjgtp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gvsuosnno.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gevwiqxsh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gvpdvfvqv.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gfmhnqgmg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gnbcdukdm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/ggmpzcuxl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gmlkgrwqd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gbmliqtbq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gpwydmyxm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gmabsidhi.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/goxmvpiwh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gxrrainsy.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gvrrikwpg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/ghbjnslzh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/guqsmbcep.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gbdvnrwls.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gvmfywtpd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gqxidydyd.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gpvrauzpe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gpuvtpnkn.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gifyasceo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gawprfwdf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gnyzlmktz.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/glnvmwkfz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gaafdxkjh.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gmyjvfexe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/guinajgwk.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gdejfppua.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gavbaxkkj.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gmjsfhbak.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gxtvmsbmi.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gtexsbajw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/ggjqqqydh.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gubylbqru.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gmldgnyhu.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/glwwpulqd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gyombrvwf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gbmzgyhno.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/ggpqthgtj.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gohsusswq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gagwlfivn.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gsgeuxzol.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gruyqxonb.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gnsrnbcho.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gmhpagmjn.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/ggnrgfwoj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gvzwaorow.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/grkzgzspv.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gdalhxmpr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gjdknvrvi.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/glzglsqkr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gshmyqxsu.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/giwwipuso.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/geauocsav.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gpitvcmra.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/grawjidju.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gosrcylgb.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gdtuzchgi.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gtqngbvot.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gizueayeb.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gvpeindna.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gcgbhpchg.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/ghangapxf.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gezrybuvy.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gmdlobyjg.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gqbwfbnzc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gzjihcjof.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gypmdoawn.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/grasobkyk.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gcfrulwap.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gbnafrgvn.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gjbdevpih.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/glcaiekfc.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gmyiantim.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gndmnlvkm.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gedpwdycv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/grkdjozmn.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gzeuhjtvb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/geaiaorfi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gjfnmwncq.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gucxosjvq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gwjrwhrru.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gfmioetib.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gajfgjant.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/ghuaeruaw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gyqmcqmjx.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/glvuozmbt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gpbfdwdow.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/grybkvrwe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcwqzfqkf.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gfbvirrkz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpisyzgis.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gdidhtutd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gidsbifbw.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/glwxycjpt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvdfmqxwj.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gmsprjhrk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnulbhxkm.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gyevwdztx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gmtruptpf.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gupmsotqx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/ghccluzky.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/goipxrffz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gxnxiedmd.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gdbitonqw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gqbwlivmx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcbtjcmey.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gghxxyupb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gihauqvhb.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gflplibqh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gyikbkhbg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gproapkkj.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/ggchwcpqz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gloybpeuc.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gdyservfd.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gouvcrcwo.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gwbqfrphu.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/glvqsrscq.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gdopcymom.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gxgdwirzk.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gexvkozla.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/ghnmkmxcx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gvcjvqjuk.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gfpyqudcb.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/ghgjyoikd.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/glkiomglp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaflcraus.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/grkhzhibh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gopinkgjo.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/giiezkdnn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gdybyxemj.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gtsonxslx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/grjucpxlp.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gzjdxdaih.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gkieuhdwg.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gnegvtiyp.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gtynawbyj.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gcsmdmyfx.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gojshfesb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gypqcdfgz.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gkphyrrbf.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gfjtkakkx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gutnyayrk.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gpjbmyyez.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gzhduhxbe.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gsgyhquoj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gdnownkzh.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gbjegsyml.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gejniwfsd.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gpzawvybe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/ghgtqwfyf.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gltiezfke.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gbccvbaug.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gjsfezvng.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/ghgcmoouu.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gepcnzggj.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gymfonrzv.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gvsqzkxsr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/ghpvyamva.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gbbpkskfy.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gowkzvtkc.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/golytlcoc.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gwxnltgkl.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gybjkmfcg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gxsmiwinm.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gcgajewkm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gvdqvwsck.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gibcwchqu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gscfwnxmh.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gassbcqvd.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gakvafgzg.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gvuipglwj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/ghmrzumez.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gitetwfqe.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gezucpzkb.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gevoxyxfj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/glywsfete.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gjhtjsmmr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gpilgcsfs.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gstzelbdl.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gdfqcdnit.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gjfkicdir.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gcbnshsgv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/glngdflki.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/ggcuswklu.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gltfzdryl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gzskritqi.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gtlmmunls.sHtML


<!-- 参考信息 -->