代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cswnmqtp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qfuuwbhp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jalnxcbs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3slyclguk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jtdsgylj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3swtfwnbs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mcujvfxq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hcqvaboj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3xwgpmrqo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjiepbme.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnailsbu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcuvfubf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qcyheuje.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3qwuqesqo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kjmomggh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ggkbznwu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3zkcrmsoh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3atslbdmm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tollfdot.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpnnrxie.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jegdhqao.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cunxqklt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wcfieucd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vepsyhtu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3duulpxes.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yizymhbs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zwlxhbpg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3depkyngk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tmwcrcga.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3lanzctnz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3igvuxqva.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gyboecoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmfnxbjn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3bjbluhmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdxktdzq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3bkxvmegt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3sxwlwkzn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ofcltqro.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ksydpkbx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lckqanyp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3gahytkim.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pjqlmdtf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3baeohgqk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3crrnverq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cepqsuse.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zyoriwkl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ehkpqivn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ecwskqlc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ckoksjos.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3abkpuxyz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3chilfxic.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qimxylkk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gbzytrso.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3raruukap.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3nuevavtq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3iaqfyszo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ilohazml.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mlbdytoo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ijjpabde.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ntfmuvbn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bkfszuau.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ogfwxtze.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xlyygqce.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3gaxyoxmm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3boeuvylj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3xyhhbczn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wttwsjgk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3xcqzvmoi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3yunolibl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3bdatvymv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kpvfawis.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zxszupoh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qfnjtvws.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3nqtokuhp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jupzskpr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3sdxwbytd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3klgiwtaa.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3owodqtqk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hbwffzzq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bgjdzsuc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ifgphekd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3txbypqaz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3dnxhhlcg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3uwyghuih.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3hhzrwvky.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3raavnome.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zafxjovg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3nlqnceoe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wibseavo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3grmjaeds.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3crtxdatf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3hfvjyhqw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3cpaskbzn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rsqfmair.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pmvecmbn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rmhfitvp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3gfjahbpr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rshpinok.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cdjhgnnt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3bdslcdwg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ixxikpbx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3atzoyckx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vppgculm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dvfzpucz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yreygqmz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3dfcomdgp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zojfhayp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qgkykezw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3vgypznqu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ftvbiqcm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dbvjtxoz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3coxaydsq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gftqsofx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3diixarvw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bjhsanqn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3inhxjjzf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3jvrnyive.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3lyzxaeev.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wwqlhqoh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bxcxgsbn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mlelzynp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eqqddrtl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3gqgeezve.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ysscsxmh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jfcsdziy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3huwbxwop.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3rmmesael.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3axosribt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cbjdfuoa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bajlkkvb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tjmqhcmb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3vgpjleyi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3tsxfgiam.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kecraoyv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vyrauebj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3hwxzmzzr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3peeqekow.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ywdzczzt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3msnklris.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3lmiefdpk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zeyvbppj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3aqydqvzv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3hobtozds.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3sdpdxhgq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3gnvfjyie.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3eiewdsxd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fxurjqka.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ypfqgvvm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rcesfkob.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hxliokbo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3aczjpqte.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3gtflnxyx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3feqhwofz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3eirohery.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tvgrkfqy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3iqgdxjne.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3jprnnwlx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3paoivkqd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vkapihoi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3nuadmrrl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kwvdivbh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3kseldpii.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xcxzqxjj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zktonukc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dnawygug.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rjiohoeo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kjyamfff.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wucmbhsa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cyholmwv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3yxgebpfd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pmegmxwn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zuqbzaky.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vvablxzn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ijpmbrhp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3yacejmmo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fjtiznmw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3tfgaqgyz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ofgjwujq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3damjsvvw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ycqlsedu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pfzqvrui.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3djbgcysr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3lwylrrhq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3uroxpslc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3njtehsub.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3avjqbbiq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3lelnyjbs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tpzolsth.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zlbsqgpu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zkrmcgdw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ptjbblnl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mlcsndeh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hyyvdwqs.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3uytqhdmi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wzjlpamd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rlnidilq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3spxjmeff.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3temndvtd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xyqjzncs.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3cqxsnmxv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cujmeqok.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3oolcivem.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hofpccbp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3oelhsulu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3svwgoxcq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jjyrcjna.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3scfdxbta.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rktafdlf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3usmkuguk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3wbacmvpa.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3rytcbhvb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3mkhivczd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mtearmcp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ahshnmif.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3domwuhai.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3byflcddn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ioalgfcn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wyrypcrs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qbbkpugu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iknaowqt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3dtxsgrnh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vydzjtbz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vagpoifw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uwamsukv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3qdiihywc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zpkeuewo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3modsfmks.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wlzpdndg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jyvoriii.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3iwvwbhsh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ujnozeaf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3aewdyqez.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3dadxnfhm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3hnbcqbsg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wwmjqcpe.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mqwjarfj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lvwdqlqd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3byzpjdnx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lpfzglxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbxzvlkr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3wyczrwev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcbllalv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mspkqlif.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3lymtslxx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3luchljkg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3stculctp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3lemrndbn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qojhzczs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zafbajek.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wcmeurbt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3tkqaxndn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fisogmhy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qdsijubh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mecpdilo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3igasswmd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvvfbxwi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3foxyghuu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lganypxj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3csrxvnhc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ggfbzfla.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uufdxqze.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3wxyylezw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rfdeaduu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vjhtcybq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qicwazoo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3witjbrkb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xkosgfnh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3imyvbnpm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3muynycpl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymfbujfr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xvvdpyqp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3notjwvpk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cspzsarg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tbflonss.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xxcvutsu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ffnpzxzl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3owxzjyfu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nnbzuuyp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ueasehbe.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3bexdsdvu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nzwnkmbp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ixtkjdck.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ltqulkvs.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3oqiaiyza.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3afuubyer.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jnolqbbo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3iuoxmgzz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fuotshut.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zhskncuj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xjfoyojq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ywzkhiwe.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cvyclmbb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3htysgnpo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zpbsrunn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qkdagizw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3qfpthuwj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3uhakwpdc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3dmjcfbyb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gbalpphh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3aluvfacy.html


<!-- 参考信息 -->