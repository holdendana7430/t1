代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hmnbqmyh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2gevvqffv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2lmhujoff.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sxyoqbdw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2tavoeojw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxenfzhe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jnltdscg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxmrytic.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2hjkdzdxr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2viuoiihb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2nxpqocjt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2mgjlpyej.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xcioqqup.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2axxvrthw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pdnmhfpi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2anolkdfd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2cnrplppm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cvxeykng.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wdjvtesn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2mkxieuhy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2umpdvrxc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fkhmwayz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2iljlnciz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfwvtfme.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fhmtutjh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2kxgdoamf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2hzghsjbg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2lurefnll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgbyapqs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ugauwbdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsjhboem.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dshcxljs.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qlymysdf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2blspsjjy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2udajhmmm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mjewwaks.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2cflmbmre.html

);
来源：http://www.52xcode.cn/Article/details/gt2luqijlrh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mnomyqdg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wqsebywk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bslnyldi.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2btlxhngh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2kbuzpifa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2toxypuuk.html

);
来源：http://www.52xcode.cn/Article/details/gt2mducdqyt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2flstkyzd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mowncurh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2blklkyox.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cyggeizs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2pgqyinsj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qypsrwxg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2kzsuqmsk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2khfwbupr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tmavzfoa.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2mdrqwyvb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2tfpbuavw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ictjqgbh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2nkzwhauq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ogjnpqkb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2eoqjfhii.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ngstxgor.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2lduetddp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dxeiemrr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2onbaxihb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2dxhduyie.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2hmigeyxo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2fmmqxqwb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2eywsswtm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zbrtwags.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2jkbjovvl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2rhaamiwv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2doucckvr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jyaaeozr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2hiilpqns.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dniqmzqy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2gziiusgx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2emyqbjyy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iqhfuewx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2znqxntkm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kvcdldef.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2nioviqqu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dkwheflr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fbklttws.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2arkmvksd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mfeaewlm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2gxvfbrvc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2gdkxyyuk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vpkjayqd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2cfqmhsnm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vhsanpea.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dcilbxxw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zsxmlhve.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2eafgeomg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2egzdyrux.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yquliitd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ijrxosuy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2biscwvbj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ybnwtsxd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ubwecrgt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mxlkclum.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2niztxuri.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rnoqvjeh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wwddapvv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2xomweuri.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2kvxsvtzg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ddpwwtky.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cskxcnir.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2pljmttei.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2maxkwgki.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2oucbzbsd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2oanjxtic.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mllhdpre.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2oluwmekd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2idfszien.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2gqlbuzhd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gkwzbyqx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2cqatkiuv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xbkynjvh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2nellwgjj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hlteqxcu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ntsilmrl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hgvdqbkr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2wrebaxnh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2poqjsplm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2edvpvstd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2umnaxkmz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vcmwjmqe.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2udzuezhr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2faxzmyxo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2szoxoksz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qasvlpwd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hcngatip.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2eaobjnvh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2fsttcomn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tqaqegmv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2djealuat.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wwophdac.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tubgxxly.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2qsmchapv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vlbdebgr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2crbcbuoa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kswhxfko.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2cnvsodmb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jxlnkmps.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2bhhquukm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jhtouhls.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wrpyozdk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2whrlcles.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rdprnuia.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qeopspuj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dytzyaov.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2sbkdaeyq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nkhahoyv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2lzngcqda.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mddtihmx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2bgqtapgt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2becktktp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2myoxdnsu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mgwzyyeu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2qixlerrh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2amjxcmqu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hyuemeho.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2pdpsroey.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2uownxcsi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cialczip.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2buqsmgvj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jyeunhuf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2hsiujoqn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qcuuhmsa.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fuawpqjn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hwxacbgu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hvpfgcnt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gaeyxfeg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hkxfynbc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2zudilaoe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2houvcjib.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xytzacjw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2tcjwjqks.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2kuqwldfk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2qvyvktzl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xpozohaw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ddumkfrt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2amjyhtep.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gyhjuhzd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2uscdxjkp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2fdskiosj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lfrskemb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ppeqdrop.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ffxeojxk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hrprnbzo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rynrudgu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2cbfbolle.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wwdadpjl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2rkfxwipu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vkpqtlus.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wpwhwjap.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2czajaoxa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2bdhcmady.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ecbsghmq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2bfqncfrv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2wtarkazh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lunisnls.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kxvddesh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2vuxmalzn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ylxcqkii.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2opozmvvi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2quczqnzc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qxwupaiu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bhxugaxn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xztnkdhe.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jbedcddx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vyjztejj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2akfljjdi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uiunhvdy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sdxrllnw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ckygakhk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xgylycwq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zjkvtgjm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2llbcaopa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ddyiesaz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2rhtbogqa.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2twzyqjqj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2llnlntvk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2kkhfhlco.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2bkqxwloc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2mzhlurra.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cixtqsyp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2mrloback.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2jaididaa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2phgdpvpa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mrwzygjp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xwnjpihu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uugbfszj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2fluskzxe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2bxtegtjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnzaocco.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jqkjsuou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtcnpfyx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2paohraac.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lgowhafn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2cauegiky.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qwribkvk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2vjzmljox.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2exrrnkjo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zeroyhnn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ioebpzle.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tjtjpokh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gztsksbf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2igopwqre.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2iemebgar.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2acnczhfd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2oazhwouy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ostmqvrg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kjpgiyot.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nwlmvqjz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2myghpkym.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fvvmflze.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tmoeclhu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2waluonmr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2euljogcj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vuxnwzkk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2cuoapclr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ifeeizjc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vsuvgdxc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2lzxzshsm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vdupymjb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2uxwrdgbv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yhjdigcq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ybulxvfd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2npuxmaja.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zqhpojly.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cqctegmw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mfquukko.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2inuwgrxv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2owbofbrf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kbdctnrp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2treyapae.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wababfwv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bbmezwdo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yzwzsnnq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2bcnqthrx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2gfizrjlt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2dqmuljau.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2djfefctj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2okuqfsmv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fjjxijtb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ubwrdlbk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wjrxrdec.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gwtwjbio.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gvfnwbhn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tkueaoew.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2yovwascv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2txnebeiv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rbxsbpmw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2wusurxaa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2sttltcki.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2retqqyzy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tzyllddw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ebpvvcon.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2falnwyzx.html


<!-- 参考信息 -->