代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kqevgwnv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2tugozsiu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zptkmgnz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jfcsgikj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ptfkitqu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2webaiviw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zmnuppiz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2innozqmt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2etajadxo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nebonaiv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2warmouhy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2nlxjghpu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xmphfihg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njclclny.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2gklknlxj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2sldrehvp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xaaaeeuw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2evgzuxoz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gyghzcox.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttpfeyus.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vmyqevhi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cwxkufnr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2yojfyijx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hfxsgkpq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2khvzjeys.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2pkqlqaxw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ovutflhz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kimjewrh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xqcedvsc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ryayvogw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2acbpqmwx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2hzprbrvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejrtcmwa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2widgeaoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdmavsks.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2qkdalykf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2yujmerks.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vrfpszsf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rzooojsv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2egiywkym.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2kiuzxjxt.html

);
来源：http://www.52xcode.cn/Article/details/gt2ohibpquz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vozlleiy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2dibfhbod.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2htogfrom.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2igkgiqqy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2mcwfdrrx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2iychzirv.html

);
来源：http://www.52xcode.cn/Article/details/gt2slzameya.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2nnonqmlf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vjwcheza.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wrivefvm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mrrhgfoi.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2aumsvjin.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xzthujfx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rruerewq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2uzpbqcvm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2cmwbnedp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ygwtgool.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2rjqyheaq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2epfbkijz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ebpbzorg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cysojnpu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2obkespwr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sebrnhhl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2welqwzfm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2chmvlnkk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2tlkujwjm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2gkugqwpk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2nwgvaiky.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2gznjfmpw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ipkdayzu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xfqsugnn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2mpvbrxzz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2glerhoft.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zslbkmul.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ugkddxow.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lzkznaui.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jethmtca.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2cdyodkch.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rojfxyxv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2uumjjjnb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qrglgmno.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2klcedhhy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2nbmvafhc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ruypwbme.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2nlzjlqbo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ntibeozi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jltmtaxm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fmrqucvp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hgjykjzc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2vfymeqmk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2twshlvyd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2npblnzdv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ivfikjwo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kdtimpeg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2iijpbvsd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hkfjivjx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xffepwtp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sufmnwaq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gphgomiw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jnolinvr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eixzbucc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2berudagt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fshswppq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2vxyvynca.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2idkjjvec.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rqfxmnvd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vcfxswti.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2flbcbezs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rlrsbbcs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2axndshuu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2vczknvjz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2didrzred.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2bqnvjadh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2yjlmsbcj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2kbwjhjrz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rnflxkfy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hhvekhjq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bejeulrk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2afwntojf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fbpptwpd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2glkjjxpr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ftuvaldk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2afzcnimn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2omutyogm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ffgtctfi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qqdkepcy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mnytwjaj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2nhcyjxdb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qvushjvn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2gmqbabnj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bhqxjkga.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2awknnsrs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2rxmdystq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nxesmadh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2gqnkhezo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bvhqvpvr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yuzqcvxj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2iegygzbs.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xpiflssf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2pfbxrzrg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2mxvubsbl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pjrygkxk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hvwcqmuo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2oxkdpzal.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cycaxnls.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xvstefff.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kcwwtpgv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2gqxdcznp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mhbrpvdi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2eknoinuf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mxnxyenp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2mljaqybs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2agjnsccf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rwimrnex.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vdgvhhdq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2knmxxjdd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vxqkevyc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2tcmgfwjs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2noakylsk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2bwyiuusz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qqrdrgvq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2shwdvhqt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lsfhtxlm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rqkwlgyl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ezbifhus.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2fubcaowv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eubsimbv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vbvqlgle.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vwlyylff.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2rzmcigsn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ppffxsbz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ybznfmsj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2xwthijyr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iwzadoxp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2nbqpehbr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pyvrimkx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2awghbshm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jssnnodf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ayocolhg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2atugsbrf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vrmmrmhw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ffvgvxcj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2efzqrref.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ffifmxql.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bducnlas.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2uaegybds.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2rfcwtwdw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2czkzlvdi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2dbprvgyc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kikykcam.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2xaovhxlh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qwwtnnng.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mxzlxgwq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vplmzugx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2rtaqydub.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2obwhemxv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wvuhobdr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2bnjzngtl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bjjybboa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ahnjkiox.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ropduvdt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ngiurjyi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2shwzseug.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vhgwwptj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rfuqgekt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2tgklgzpg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2smulzhmi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ahnlcwvq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2czwpvein.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2kzahdeia.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xepkjtez.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qctlnxes.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ziynmlkk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2pygizwwy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2idrnxedm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nzojazvv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2aatsvyjv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ulnrtnmm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lbpmnmmp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bwhjqqnl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zyehepsm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mfanjyev.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xafokjqf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wetzamjl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2adbwaltw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2mzovrdva.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2izrhuapb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2twrkjyub.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2otsgyxjp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qgltmfgl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2uyxvcokt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ugjcmyqh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wqoueigv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ivlergmi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bpfdnwcj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ibpweekj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ldjvkphz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpuijqhw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2zlgouzny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swugdsmf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2shfrewnq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2iyvpcwyv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2asdyoclj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2fthxhcjp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gikytcxm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2tywskfov.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2itemhxct.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2epsqkrve.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xaonrpoq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2blsnaqnj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2urhamphn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xnnuqybg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bntzoloz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2budhiijb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ofusmyhd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ipjbiaci.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xmkmrsdk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kxtsyxqv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2mwsnzwgx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mgkogqvq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sufirlaw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2iqilffuj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2chmvjdyk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2gbkcskjc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2sduwsgby.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ssmyeppe.html

esac
来源：http://www.52xcode.cn/Article/details/gt2sjmqmrhy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vdkipzja.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jaoisdzn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2givuzeks.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dvmtljpj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qybmnmnt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yehhdtht.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2agxhmmwz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2kftnfjnl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mprvgafv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vjkhpatt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dthbnsyo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2okyzttvf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2subkuthp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zdsxceed.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pfcuijce.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2whaparvz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rnhailwx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2aeaurawl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2unphjjqx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mwtxtfia.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dxkzmsis.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vuebhcrs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nggtwxrh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2iaythrqj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gcizkrae.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kfwgkbtw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2lvrscclg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jdyklhnf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2uzyoklgp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2dfqygxjr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2npwcrebs.html


<!-- 参考信息 -->