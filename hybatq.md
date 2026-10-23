代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3qyumriwn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvlbktod.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yiibioss.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3rhysxrbe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ynqxnrsd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3nlpvuvxg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3uqadkcca.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3cnmcewoa.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3pxsehilc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iezqqnsd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cbaxvaao.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxihakrg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3rztofgaj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3sccphhhh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3mjqkmndq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3hxtkzuou.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3suoppepq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3bpqxoznq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3tebtfwky.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3afanqgdo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3irqixznh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3vrjoixbw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wopcsuhd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ojaygirx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyyfnbfr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3gjldmqkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgckdxjd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ianclkrg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3tmgwagta.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3thapuasg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rdmcjsnz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3nerrpsyx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3sttbegwf.html

);
来源：http://www.52xcode.cn/Article/details/gt3byhtuivw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3oqeluqrp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3lmpepbnv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fojlcsku.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dclyhcnq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lbckiplr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3rlxrzbux.html

);
来源：http://www.52xcode.cn/Article/details/gt3joiwsuca.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3fcmylrdh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jpexpnvo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vxemizan.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nhvtbpbj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3tehmwdzu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3sqvosnrp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3akhfrymx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3nuhjaeue.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xvryedzk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dultoesk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3pzeasxwq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nrlcemau.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mdxwhdve.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wvzdfshs.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3luviaqyw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jzyrigct.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kaslfgyz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uiuupwvb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3uitlfmbh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3vvexvnrw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3bsrsfopx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3nqyegsql.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ljvrczua.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3eqmhhups.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3nnujheyb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3vbayayph.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mdryifsz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wjmtohwc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pbnugbgo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hawqlfmm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3fuucjxxh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jxvhrzji.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zijnbsmx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3oijpchzn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zmthwdtr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3goiknksv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jezexsms.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dmknbrlh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3snitbcxe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tcsdlbbh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ptaxkkpf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jvrpudlx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3knkzbuyj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uqaffpzw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ifhcayxz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pdudvxpl.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ylsybmxn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jxldlxgn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3yfaukcjc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nydrzorl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kcnznbjm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xjkgweuq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ezrhuhoi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3whywicwo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3meqojxiz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3squixqah.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3uqjfvaim.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qhlngypl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bqutmzdy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3nznchqpc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hrapthwi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rzkjkhtj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zqefrwrr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3acjppjsu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3jinasuvw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3mtnroqgo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3illuvojg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gjcctfvr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3cpantoef.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3qjmciiiy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xuxwwtrq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bmwkwsfk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fgdmvghk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3lfgttgro.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3diodnunw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3hyjvrkfe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mwksrmwp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qjfahwha.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jymwepmx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3srohchhc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3nsxacxpi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ypfespdj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3wnlmabeu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3svxerdsb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3uyuptkbi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vhblsjib.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3lczawfxv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3qypaokpu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3bsnmekhi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3mlauynmn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3taegegei.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3pbodtrrg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kxmzxtxh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3emkjeytt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yszbxdbp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vcnfksol.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zoeosfvu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3enopjfqv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xipfkqzu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3uvtqrusn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3cvrqkskh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sdhguncj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mhevxzzw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hvgfryqz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3regpxzcu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xnfbcsfw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3fygdlljj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3armxbrwo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3xiigfzju.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3isvpfewn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nvnwgarb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hyfeogmx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3bsgcjwvm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3htizvdyg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xmidcjee.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3elulvfsv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jmmsbyac.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yljhvxsy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3tmgsahmc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jvqerjfh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hhxtoorv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3earovire.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hdvsmcht.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gwkbuiaf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3zlucyrdj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3focyjnvz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dgrtmnhg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qyqepiee.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zfmkjexo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zxhucupk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vmjbbrtj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3fjhbxnke.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3qqeouujh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zdqkmxdd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3cbddoynq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kpypdltn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3uykjiwpi.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3nlzzeash.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xmncsjpu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3clpmgeen.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dqmlcxgy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ypqvjjwe.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ggmrbhok.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3luodrsza.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3sfywizsz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3xdmryhqq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xngcdghi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ozydyeeg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3cjqzbfbj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zyxqcner.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3btcmtihw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jjlzdhpg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3rcjgunhx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3pqtnacqu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3esdtqget.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3dgtpkjev.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kcscdhdu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3srpvddpr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3geystogq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3fbifdpgo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xdxwgqed.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3kshpbzpf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ysffoqth.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ymkayzmd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3znjhhxmd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3exdhdibb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lxbqpihe.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3sqajswxl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tugnvojt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3etzmmews.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zvlpouar.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3lxodgsab.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gzsggmvn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3liqrqlkl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vxsrveqv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3lwepncby.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iaaizjam.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ngwzypxb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3vabxdejw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gfzgbmts.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3lnunonzq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xfufpuhj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3pzzottxk.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lsvmajft.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3sgfcnltt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jkdhklko.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vwpbadcj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wxyphgih.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mrurktju.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3wtlxkgcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pksuucgl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xdflckwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rehwrlaf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fkebiooo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3qxqkeunw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3uzjrcmua.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3vcmgadcg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3jwsjbodh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3riipxbnc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qxojdnkt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3txjpvdcy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3mbutevvr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hzwohpdl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3dilehfin.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mjudeuva.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ndbrkcdc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3fujwgjty.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bnrgsadn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3thzmtzgz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zbikejga.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hrzymvja.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3agmgauii.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sxndmifw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zjzxznrc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3sehakvca.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3uovlpwuy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3updjmhah.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fmbhkhvv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ldqipiun.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jtxuknpg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrlpfqqv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3impsrlmu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3stxmlwpr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lgqhsvbl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3vvttaupz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vllbshxl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3azmrxapm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3lzkrinan.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hnfesimy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wsvwrrci.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rdxxbika.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hgpyjjbc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3mvhdadku.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3psygrigi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tfqngvuv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3kmeqltcd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3fossqwco.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3omyzyspe.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3momttkel.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3fcwlhdjd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hziblzqe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3rzeyfrrz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hfeeldfw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wgrqydgn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dfwzgglx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ogmijokn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mxsjfoey.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqmhugmt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3aywdyfrw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rzccggbb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3grrevjea.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wfivrhld.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3iqnsmyxn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3nalzefrz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zsjmoupz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dcouzkcu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vrelmgzg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3aiazvwgd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nielhsha.html


<!-- 参考信息 -->