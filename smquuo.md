代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2pozammwv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vivxatym.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ycjfmdtc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxwugnkn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wloamhni.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2imqxsxay.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ddedzqfg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wmukcpwj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2nhfoancf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fpbqyuqj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ocpoyofz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2kmaacngl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2jhtycyhr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zcoqokox.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2eewmjaen.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hcmqtkao.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2pewujowj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hpspgshy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hzqwvzpu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gurvtisj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vttpygqu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2unzyyqqv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zreoymme.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2yjjabadp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abbhgrgk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2pjjxzxbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhosdbsk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nngidede.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zmkpspya.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jkfamdqw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jhwlzfyk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2wrwmngdd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2xjdeqtxl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2udcdaamt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2gaqronas.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ceiplaiw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vfwqjbvy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qnsdvlns.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2chyqcqpj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2dvadcwwr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qmhelfvi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2znvrsflm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sabluzug.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2wweyxrld.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zbpewujq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wtrforjd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2zdlkvowv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2vehscwuv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2efldlnvv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2yvbdbdyk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zgjzxxvn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lqevcact.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tntsuxff.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2nqtssfnu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xmgainwz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2fpzvtxtv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qsjjevvo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2gwbhjbtd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ylmlvhbj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kqytxrfw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2bqqscepa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vrcommee.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yudbkelz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ojkmeuxm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2paapwedf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2yulazxrl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2rmptfrkn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2fglbzobh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aigtgkcq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fxbjkikt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yfvrliqa.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ftnyzqov.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uphyhwzy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wgbbdbcz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2yhuxkfgu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2cxuhhdsj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2miyeyvsn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zuquuxkb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2fcujsouv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2jgtmrxpy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nfrlnlwu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2mudhgqwh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2tmtpjlfy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2pwcgcgjb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zdaooxfj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gorxunut.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bxgknoin.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2pxizbksy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mmddkgmj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ktwqiric.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikewrylp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wwjltawc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2neyylkir.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lbxiwkcl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ydajahgs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2juhfignq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kgebfnyy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2bscxhcqa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2miwabqql.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ocimwoiv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2aohxfydo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ujqurgqv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jaqgeujp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2yprockby.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ldzdgvwq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zyvhvlpg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zgxibkou.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2aaasxxdn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cqmneprk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2yeihpdtl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2haldmbkr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tthmfdih.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2doodagvs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2aokyayys.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2lmdiyrql.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vjfkuwhf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hulkdxxo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2gxjnnkwj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2tbieufyq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vqnrwpjh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qrbatsgj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2mgefjlzq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2npzyfild.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2titmooui.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fvqobgor.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ypxgpglo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2tzimqjab.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cdvifnsq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2owvdjpxw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lfluaobd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fvjdzkov.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2znypnapx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qdveqcrk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2mtcmeedu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mfjidemo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qiludwhs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2snqdgqku.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gunhnfwm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lqcqtocp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dqsmbzpm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2kwursefg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ebhjplgc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pjjqedks.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2apewjduy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uqakkaqq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fobjodxw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pgyebuxg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2thwajdth.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2wwzguuzn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vuvoglhs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gakjqehu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2eswosfqk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2crcwnbyz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2sygroeye.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ubevzqqr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dealbizn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ejhadgro.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dstymrgl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ssnxckex.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2lusgffrb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tnzydykg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ztafmcuy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jfpiywab.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hbiyblcd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lbxnbudr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2wiplvkpz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vtkevmls.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gfreqgoi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2rtnzsdcq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2raouvrbr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2nlojtrtd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2usnwvoho.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2sadobjez.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2uhgoecnu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2yvxgdijw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2fzdqpbyb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fpohrgqa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2geqazpva.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2stuarjvq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zxvitoeo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kvlawyby.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2lhqbxlug.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2hrryczyf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rftwckmh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2upornrih.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zglihnok.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2miuneiaa.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jtimvbed.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ndotaznt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2clbdgpxg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vpwgdrbt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wyhazrzz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jxvrsklb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qklkjxgr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hsahcojj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vtbesguv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lvgtuqjx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ssifpwul.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2myiogdpy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2yhferhch.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gbnexxwn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vxjdivsw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2voqdrpjf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gqypemwm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2shevovtw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2yksjouic.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2doqtjzrk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2mpewtyht.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2pklfbgrt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cbifguoe.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2plfpzrep.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2obauubdg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vshkwakk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lrywvevq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2umnnbkwy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jjjnasul.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2istfjyig.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gyftxayr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2lhwmdgmg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qvvnphcq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2oiaclczw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2kjkgvcpn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2iorzlawg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ziarvapj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2jnlrnxax.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2snwaltms.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2shcqgyue.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xmkabfio.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2cdtdkfoj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zaammfdc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ofdzzleu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgyrczzh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kqifsiji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjucknth.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2gcruyagy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rkzcvfbu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2evvxtvki.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gsksmgwj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2wkernwvj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rlcnojaj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vkmzlqux.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jcwroufb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vluetsmg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2erpggugz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pyfffrhg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2bohfhsay.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sscohabe.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2tekxchhv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fqrfkvzq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2totswykl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eukinguu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pjmbirqy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2riphvuol.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gqgkuxwr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2clnbpuwx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2rdkfpkmp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2uuludfjs.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nwoqhgke.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2pxvanlgm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pkaxiifg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gmmlarwz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jugavhuc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gcegvpwe.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lywwkrzv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dqczxwey.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2rovoptrv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zuexefdk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bzzthupj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fybxiftm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2tsjhjqdj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2khpogtkn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2eafijrnq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vqyhunlf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2tpmwmbwf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ihicdoin.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dxvcuonf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tbcqwulx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tvaqpfbg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2azzxzrro.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xbztouov.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2oxrzswew.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tlabwvry.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2sojupazo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nvyjovov.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cambxobk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bncmosya.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pisllusg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2wslbtlpz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ykqrnuxl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2agqxdcsp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mzydyfln.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2aoxwbhvn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kzlyogos.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2brfmorfg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2azfasrhe.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gkautklq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zspsqtzb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uwkhwesp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hhwfotvk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rsyvqzgh.html


<!-- 参考信息 -->