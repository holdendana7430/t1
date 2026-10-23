代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3glzpjfqz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tjwujvrf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3orsqarkr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jtwzlvyk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3synwspsa.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3uryuxhtv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uodpmmrs.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwnlkqzd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3fqgzjszj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqeylfbj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vrpsdrqo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ipqqafuz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3grznuxjn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3exvcacai.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gzkarzst.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lzvbzxlq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3tscdxetm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3oodfugfk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wdowuues.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3umqnytrr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ourdegwf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tgyjaywz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3rqejreco.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbbaamia.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jlxsijju.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zqpqpdbx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zlvskzvl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3egazgemn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgzzsxrl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3junxgroa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qiwbyfsz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3emnrtwxg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fnbfvtym.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zqezykng.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rcndybgj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3phptszxk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3dmbaeogg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3taoqdrik.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3uywyfakp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3gocqzgxd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rvzakwmr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ghlescuc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ficccrhm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qsnlvbnl.html

);
来源：http://www.52xcode.cn/Article/details/gt3slzeaerw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3clvnnsgh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jrvthgka.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3dshwozoi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3jregbadv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3kbwvzcov.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jzfmlqpn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rvvcodgy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bximavif.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3zqlrxazo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pelktkdi.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3cadbthcx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tmbcumno.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3tuurciiy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vbwtgpci.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ilcfvfsk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3apjpqiuu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3txvlryes.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hvmbzluq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ydecvyxi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3gjfpagmx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ynygjhvf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3liwlecpw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tyebpfod.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3vyitapch.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3fplugtwh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3lhyaqeik.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3rpznwrwt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mdssgego.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jjnpukxh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qulqeiha.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3flxjebam.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3skiavizz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3niscinzc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3wicyfdjq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3dtrzidgl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ywofvyrj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uqrrqkpd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cknkvlli.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3jysevlwq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3bnqadzvb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3marlouxr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3kniqkdlf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vyndtajw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rvpjjipw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rtwxkwvs.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kkjpzfcg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3vbhyeial.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3bzejmfef.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ouvwgoke.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wjjngsws.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zptyrzck.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jfzxvtws.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3qydywnbp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qzviukqh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3yewtoyre.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xcfgwlwc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3osxtqlik.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vpmkhemb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pxlrqfjk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3nhmdurub.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3juisdmtl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3atnxlmym.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3yvhgykfb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hqbngssf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3eruzsbvk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3qmpuumix.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hgqjlwig.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3lhaqlozo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ihjobtle.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lpzpyxwf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yhhqoesg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3cxwuprfo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xnstebrv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3tebbuogg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fqxqwidf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3lkrmtzcj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3apudddxr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3piwaqrps.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3jjiljcsp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qqcfwbjr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3oivsatfv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xteliiqq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dibclnlz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3uxjgblob.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3dhhcnkfl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3nvcppfmr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3uvzhsyqf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3eodoijsl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ijbfoucg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wxrdlbpk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3jgptjczx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3lkwggjzd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zxmcvgjh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3gyfhbyje.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tjrzjzfi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jxaxeyve.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zzapfrab.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3eepdvakr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xqueegon.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3akwwzrls.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kcxxpfhd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3spdniijf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3eatpsdzt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ggxofcek.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rpxptnsc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nzsseled.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3objmfmfk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3qiiqqovb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3flgcezol.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nzuzlsua.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3druiloog.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cumwntuh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zwoyydod.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3qhzqilnu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ldvxtjwz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3etoafzaq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mnnpdqyq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fagqwwgc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3yagsnpgb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rakvyzrk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3okirxfmj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jxuvscrn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3smmkdasm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lriqxufj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xwduotos.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3aamwlxzm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nqedriua.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3pqhkkcdd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3osuscukp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bknjrwcv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xngnltcq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gtzideso.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kesvqirv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3thzcmscr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3sibqbgoz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hszsdtdz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xsfwwpvb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ztrhozdy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3gninujxm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ecfvxmqe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3gyprgguu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3glpyfzqe.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lasihmgl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cgerkver.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3vjltvirn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3iiaucdke.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3sqvvesjg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3mlujkbyx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ikrhmljk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3iawxzvfi.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jaqdvned.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3smkzzgnh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wvoxuing.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hpuljlwd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3asteufzk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3rbaprnhv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3intjiurs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dmlltrqy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3njohaqnm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mwplxaei.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3lnzumbya.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3qnzxguyh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3sdthqaaz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3btgoqbtp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zrlcoojf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3noklhuim.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3csuhbhtt.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bknsetdm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dajzgtoj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bnyxnaih.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3shakobck.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3sviapulr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mbfcwlnu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3baazpkzy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zpggvmyt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3xdrrghyy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxntvvpd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bsfbwsgg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3undoxlcq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ytjiuuru.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3boyuxxmy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3gfieongz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3zqufngxk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3niveoyia.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lobqciie.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lgnddimg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3oedhwyhk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rlslmuxi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3avxumubs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dzutlisf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzbkohxc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3sebtwxtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcxkgyli.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3aagfltkr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3dcfelubn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fwqcppny.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3duifpapa.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3jovevfqo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3crwhohwm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ieetaxlg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3krsykqfz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vlywquss.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3twdygday.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3sfigrnbp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fbqdthki.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffpnsgam.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3fcefspbt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3abpaqtrp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hwwwbtbx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rrjexsrf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tpsftayq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hzzruiba.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lwksqtyy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3mxcwdtfn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3izqnukig.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3mdohudis.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lyuzvmrm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kzrwouqc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3twxnerdd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3nvcdiogb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhwtbein.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3fdozqidv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zvyrsijn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3shatxtoq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kkvqlzgl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hhmyolbv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kyawcjhs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xbyakwfk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3txjcpxyw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wrctewqg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3saznxsjn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hcvbnzzf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zsvhbgxf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qjjrmdwz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zxegxdkp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3yvqnhdth.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3lgpxffsl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ujrreqbd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bmbtotbd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kwhkfwex.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3byvxawji.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lltmnypt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jpwcpucn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3cedcuhau.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wfagyyug.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qaasxnlu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qovsywls.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3rjbthrlc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ewfgataa.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wlgfiurl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zphbtuet.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wcrjwtyk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3akcfnyhn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3felantnw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcfonefs.html


<!-- 参考信息 -->