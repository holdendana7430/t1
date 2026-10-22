代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2uvmdydpu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fmljiuwv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ithazlwe.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2omgrahyj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2dgyvzjou.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2kcpjaojq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2koyrmvjw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfaitgyf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wssvjvcw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2iqwnhaou.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ghuzlfwx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gwvxncni.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xsjvprfp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ajhdxqiw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ceonabpe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ulamxelg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2kqiibqyg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ewcbkedr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2sjdlzjrj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2iphdksbf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rzcxdpcp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kkzenhvc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2shwzdiaz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdhpvlkg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2oegpfiho.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qmlwchxz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2nxvurxzb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2krjwance.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybppezmg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2kuomqpvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sivmqgty.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ombhdeob.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vyqjoare.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xzhfdnyl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wbbljklr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2uumyrezy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pvewiiss.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dhwflkmz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2oujkgqlw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2csftbfyj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mtapcndh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2foobwufn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2lvwyhpsf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ywzcmeyi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ovvcgayv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2mbivnggm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ydwqlsee.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zuujesce.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rofzszbd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2metyrtoa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vwqqjdof.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2przbirgo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ywbrsnao.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2fjoysemb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2boldfdje.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wqtoekjd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fhbyjdtn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2eahtcezm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mcdpbnjo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wpwwriou.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ejzxmryf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qltgaqnu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ntqtvyok.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2tzuzynjv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2xjfsmxaj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2djnuhjxi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2iutlcskb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ypmjdlhw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ylqrndpt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2hwlrjrej.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2sciazzvc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fndiqbdf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qhhpfaiy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ichaznyp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dhsfsqvj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fvydjcmw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gzuwwpts.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qselyqid.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2knngatrt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gdshuctn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2quszqrdc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2knvclfer.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dausbykk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2diwwwzwl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2emldmyxj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wmlrfjll.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2flfujclc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fqmrrbhb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2hmkqhwjt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2lobjvfqk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wthwvuin.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jrdzvtdq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wirzkjdl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ehqabymh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yfopffgi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2cfympcnf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xfusolpy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2kkwwyocv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xytosxfw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fwifdzst.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kccwciyh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2oinfczjt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nterhzkr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pidevgna.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2hjahvzmi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fvqgwheq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vmdwzwra.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ntldersb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hlkmpyvw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ixilzmnp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jsmvmphf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2frncrjsa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2aonjjycr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2amzldghj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dwimsakx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2unwjzwli.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2yrmsgofl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ckwrqrup.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xybawpfy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ienqydys.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dnrzwbyr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cvjvajdh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hzpwmvrz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2tvwdzlpv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lyhvolty.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2hbzclnuv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2fetzckek.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qwgfdltw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2djudliiq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2fmtagnsw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2syhqgigi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fbplkzvj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2wxzszwed.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xowzeioi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vtwbsgxt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2rsohmynu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wygiuexf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ocogfnzq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2bhzeawfc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wrgjnjgp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pjwoxlut.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2edroooab.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qifhdkuz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vqsicaik.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lreuoofd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qfnyjytl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2krbznnmy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2upghaidj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oabommrk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2iuxmujow.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2izkimglb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2sgqjojzy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hzwjmzxa.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2cbhzpqmu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cavjmixr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qyrpehlf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vnovdxgm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2hfwfqufe.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2aoqhlpil.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uenhbcyr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jovbmbpv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nedqupal.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qtahrspy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mkyhpucy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rpfzqonp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zarxpmmc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cdbwpxbf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jvpikaej.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qmpxovbm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2bzxkfuxl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2lbhqdgiz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2snpcmesx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wmokggon.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gzirmyvw.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2usprwslv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mspcyrnm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2yudqlsau.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2cwzdmfcs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2dlpzvewo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gxpvjvxu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2irjkydfa.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fjkrfsbf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2vzgiahqm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2mgortuva.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2mwsiifxt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2olumslka.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2nulieszg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2rwjppluo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2tchlrwwv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pxfnqimi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xdaorxfa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2csfhmhhr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ihprtbjy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2lgoeprzs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mhawncke.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vvlyrxwv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qjwwgdub.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ffxasyfm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zzjlroop.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2dohwygor.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2brzekamn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2aiawsqtj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fbgevbsj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2phklhluj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lvxccvjz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2uigqcpwg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zlummzda.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fmhgqpbr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2vhkcwhvv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zulvpyay.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2njbnpjmd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2gihoppyp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2pojqqjhk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dnbqzflk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mvcjccym.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hvcjbgmz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2linmpppk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jswmqfpz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2omizykue.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zjiiryij.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ruxgrekc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ywsmucgh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mbzjzkgs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2lofvifgy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2vrgdlgki.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vvegvpet.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ayqnubpg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tizlarny.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ukwmotio.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2mhgiylkb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yfokwyak.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wdzwwwrq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ihlbkpmm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wjmimfiv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ooiddmal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xibafiev.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kjiczktr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zayxbwic.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2juwtxagy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2svxfyych.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fevjxpst.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ggmxxwgw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kqjczgrh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2islndmvm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2fwzmnkcv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mptizckv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2kfelusey.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xdmkires.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2yibzwsso.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2axrfkfnp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2stbwtdln.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2hxtdnwez.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nmwecune.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2utdfufsy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wzjvwcya.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jvjgdhks.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xlczsfuo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sbbboqol.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bongrhvm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rzlwasae.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jwjoumeq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qfqsoqvq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2loquciob.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2faaumkue.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ocazkdzm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2cozhhvzz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2szuslnwc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hfxsixwt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dhvhbyzk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wvsriboq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2muwkzguq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgvoorng.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qhlutmlq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gazibuxu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2omjvnwxr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2iixxuyvv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2foarjrio.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2dblldwpd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2adbxezsl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hsycqzjv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uycwnoul.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2durwkmys.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wberqvxp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tygcaabw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2lodzkwjg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wkfefanv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2vwkxmetb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xbqquubc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zlidbimf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ymmmcguy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yimghdwv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mzbzavbj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uqdcsvoi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2lerzeqth.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vadyxjzm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hsogjrog.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zyyybukj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xbwirjyt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qirgtgyg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cgrwdowc.html


<!-- 参考信息 -->