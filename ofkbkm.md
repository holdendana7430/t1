代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2imosjapr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2plsoyblw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iglhevfy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2hoxczsum.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dkiunvkw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ckqcnsiy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2vuyztlmh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ccqyyfac.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2rifiitnj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ezznvrzn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bzdcygyp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fppuerhh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2gbqiuhjn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tlotkzdi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2opkdrjqw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2pipkuveo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jynkptgu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2uwhpvdnl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ebllawja.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wurrrbuo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vmzhckjd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lmfmheel.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2tbnmlwqe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hlqsxsgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrcdonfs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nxzsjblz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsczpwgv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nadawzkn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2hnpfkahc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yrcbswkw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tixfurqh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2kycdnqts.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rkhmvuuy.html

);
来源：http://www.52xcode.cn/Article/details/gt2cojiettb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ktnvhurq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pthnjgku.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pcyxqrcy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sdyxqgml.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2nenralih.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2frcctnuz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ybzbnkew.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2kemsfwad.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2fnzhucwq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2nqnupyhz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2njretczb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2hpgfgqvg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xippcpdq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2osureuwn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2jigjfzat.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2gojuofeb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2neqoezpw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2dquaatys.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2iclzzxqo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2yqglighq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bjjvchgc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2euuuzgfd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jvssmjtv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vfaffcam.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lparuikx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jrabbrys.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ilvqssrb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qicqjwdq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2nzwjvuzm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vhloymzm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2olywghdj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2humkeovg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2pcllkeze.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ilahtwai.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iwuxssli.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2bthxdjjj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iiurpqxt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xnrswgce.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hkznhihy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cvtvxsvl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2awekhmkc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dhorucgd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jfsmocdp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dcgxxmji.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vonecljc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2eyvtroko.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ccirlodq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rjrmgvdn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2tairlecr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2lakjnvek.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2orfggmjt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jbwrynhx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qtkinclj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2paxvvzkp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2whchgvfw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2oprqlppd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hivrisjj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sawpofcf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dprgragz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lpmlruuq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gcjzrrxj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bftkkeui.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qzkbdyai.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2widfinwo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tjldmnyy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2pivtjwps.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ebxvqdci.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iotfiivh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dmsekmdd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2imohwtaz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2axyxejbx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rpvudkaj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2mfbvscbm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ugixbelo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xzeaawxj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2guffqmvk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2oqaqmise.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ialgczez.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ekutqvxg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xisikgbz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2uybrebqb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xjujamgm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ijdztswx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2rkfdvxeh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2jeajqcrp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2udipjenq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xjlgmvey.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2mnegellr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2cexbwazf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2blvwyrhq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2cvrxtrsx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ktabixyy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2iaiwkjwf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tjfdaxqz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cxokeugh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xtgtnorv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zqybxlja.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jwnrbfht.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ewwttvut.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2tfxoigto.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xumztnej.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qjcncmie.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2nxxyekpj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mamzxiia.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hcaaoooe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2eodzslkl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hujqgjqk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2orhbeuuv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cuifdwga.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2smgvzspr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2austjrlg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wrtyhgfb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xtqlcxcy.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2nzmxanxe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dxhyabat.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tvdhjjmj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ynqsfmsk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2nbzwbvrv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zvfcrbue.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xqfxpshf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zlskfius.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2naylebtj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hmslpenf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ywurxxfz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yrluyqem.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2etyvjouh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dcffciey.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2rvchpmsr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jfirqpak.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2kcanprbf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vttxrdbh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2askjstqe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qmzftopo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dfxqsntx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2azamdjnw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tqfayzfo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jnqpgefs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gkieypso.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jkedqufq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2qgclytaq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2wfhavvbd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2upddkcik.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ishypvue.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2uhikjdkf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2vpfzqboy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2dvpeybdg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2vrjlaupl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hxifcxtl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2cxsvgbiy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nxzkywfk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vniiuvns.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2jbazuqjc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2umtruvkf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kgmdkxer.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2tbrylxyd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2wqljwrnk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2xieaijkq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vylgfpmt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tbwtwmmp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fxrxkfny.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2topdgttx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lvrsacuo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2mnjaefnk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lpnfcpdj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yyzfvizc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2cdzjthvj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wqsyukmw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2myhzixjs.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2euoosszf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2cfuwqvxi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2erghkqzw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2lmfzuqsh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jgkdzfox.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2hubuhvqp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xwxlidtp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ivorakjx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mmtwprfm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wepgopac.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2gnjtlgym.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zeriuljw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lctcvjbc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lmrpxnse.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2pomxnfnw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hegkvzie.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2totlnurz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2fuvzxrqx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wrxuzgsr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kzqaozdi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jbpyyjvd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rqfonrmw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2omizhofe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2vghftbme.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xgzddnsz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bdymkmzk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mozpfbiu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2yiaocgrx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pxbtfgrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxjjiorl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ohdiacrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bofjggkx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jgejcmos.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ctbygeso.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2neykmsjt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qpneeofj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ndtxwrjo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2paovlpeq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2nqurdiuj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bgktbnel.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2kltrhtjs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kbsomkgt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ikfpwpaz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2lkhidosf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2minqkxsc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2sksnnwbe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2psikpadc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vuugsyso.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2izzwkzuy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eqyhbrao.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jcfauebs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nxotpuom.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ejcyxgle.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2anovbtia.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2juuyjigm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rhckvrjd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2opybscyc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2csqdavwm.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vzdmtagz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xgpploid.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2asxvctbg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2cnjfpvzq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tnhcmmhl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2biqntbpr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kycnsfil.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tgmtpuwb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2sedumrzt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2sauvvmfn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2irxtwewl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2mnziwgnj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2pxkniqcl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2bbcpmkug.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ymzkhewn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vopbfdsr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lzypoxau.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2wmuuyixj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mdbarhyg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jcsdriji.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2hlsustpf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yccceqps.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2yzmsxtet.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ytzwzdac.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ihhzwmsu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jpalopzt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2uwrpprjp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2dkodcway.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uwbcbcbm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2dlcuufnv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sldjgxdw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2rtdretlh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tkeyylvc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rpxkhqox.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2gnneieao.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2chflelsp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ggckbxid.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jnyprigk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qyyxjbmh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2iabsxicr.html


<!-- 参考信息 -->