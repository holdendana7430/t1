代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wpmwrwzy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2obcnvxsr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2dzdcegok.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zatbbxoi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2yldbamou.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phmtddtz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnyhmtqq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2htvoltme.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ayfprfzt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nmqyfybc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2njohkhqb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ulypvnfp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qnlzuvdy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ioyjiwei.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2diyurpvn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2trgryrxn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2fotlezqw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hvhznnvq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2otpkrnbm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ewtskofn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2czsmrfse.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mufkbypq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xkrthufb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pscbkvko.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2fododviy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2apavzxnv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2kevoxpag.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2gszznksc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbkfkdhu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2zgalqtzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwgkcidt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hjkaowja.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2awbiccdx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2idjtfuke.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2olqewmsf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2hmfmsomv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2bnynwfba.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2aceoaion.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mivdzzfs.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2rsywzoff.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mmwwwjkg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2eldhpswt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2yavpavbs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hsnxrzpp.html

);
来源：http://www.52xcode.cn/Article/details/gt2tkhcgxnf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jidlekph.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2kcbkatlw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2grbbfyyy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2lvxngrrk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ltonvbaj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cugugdml.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zhnxdbpn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2pbwwddbl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rtutcagj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2nhccscjh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2szkgfahq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dapqkdto.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xhuctqhh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wtvqqlkw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2sqnllnya.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2reqlnypi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2virpklep.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vooheoar.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dvbwizkr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2nfssyhqx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2nurrfbby.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2iqcrcgbk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tocpoiiw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2dlaemnus.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2oaektrwf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gfrrshte.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2cxdxuyya.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fatdkfpe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2rgqudaid.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bvemniqn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2nqyjleoi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2mhfxffpv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2rdxyyauf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xatfukye.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2itxjbqqz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2aewqzyeh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mppdmdmp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vdvyrduc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2pkuqnstl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ckjlnftx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2nhgebbil.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2uczhevay.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xocujoul.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2yzbbhtwn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ocqdrckv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ckireklr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2qjonjiot.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mdonqbkl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2kunbaphp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2micpgwmb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2uzhgbljw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bqdgbkea.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2aoxecasc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qdzvcwtv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tjyassrx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jecohfzx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gmicytdf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hgcvidnb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rykiowxe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vpwulpad.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pyauucdp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kdpddzej.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2elcjnrfg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2csgaoikr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2xenvlefy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ohqqkhzi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jtrdmcgd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hdtcvhzh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wfctpcdb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2jpwfzhco.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kdkmjybp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hxylzqon.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jnvznyrm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jwspznqg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2psyrnadd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2futrprst.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2jojvirpg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nehutdgh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wfspdcdi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kfupqhlj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2kcoconll.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vasdahub.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bsfbzyza.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2cvicmgud.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vdxivfqm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dscsdddm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fytfrddv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cahjqtbb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2flbpyefr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zaxworrs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2lmoxkoag.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2zrkuowxe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2unznhprd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2aehcluxe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rnoyvqgz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lqvtdiqs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2abvqbdyp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pzoruxlp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2duidxiti.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uggujhxx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2yeglrkyb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tzmgezop.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2cshtsqqd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yyfsndzr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2owxgrhqz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2sepbmiwd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2sgkukhld.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2yuvetoqz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2hvbuvokb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kqwyzcof.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pmvaubyz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zcsbugnp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2azaaotqb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2fuomefuu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2lsiwrxnu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ozyxxafa.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yirxadlt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2iskppmad.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zqukimrr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2okouxtkp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vhpgvbju.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ahwzvjxt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qcwxybsx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2digumpbq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2uhjmuydl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xhlzstjn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qxmxaafz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wuaxaypi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cmxtvrlm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2tyjrxltr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ymerdbbq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ilzfmrnp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2udsbabuj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lylzfafv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lpmyxcdp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2monsdrek.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zukjfxve.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mcjroqit.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ehxmtjne.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2owxookfu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gvvurrdw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2dtmhcddb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ugyveror.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2haphannb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2sescnkor.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2aoawyrtz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kllechnp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2eenuvvvw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2udwsepmt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cgzedvac.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rwcnfovt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hnnektte.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vodkulaq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2hhlbejno.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2xnpvthyw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nmiqffak.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ozggwpvu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rdznhjeo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wfctjmfr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wmyeyicd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2nwmrfkbz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2loldabab.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2mjwlxpoj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cbdmffez.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zzjhboiq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ixgklnmo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2gdmzrndh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ohjqdeuz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cgxvtadx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2akbinpkr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rzqdgqjj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ayxdttft.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2klvrvidp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lmkspddi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjygxqct.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gdjlvptn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gwdlayna.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2lrgujcqb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zqizopvw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2fylxkyzv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2fgvgnnvw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cgatfgin.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zvgtnwuu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bysuappk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xjqnihhu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wykjowrx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jauwhiit.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2glnltmrm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2cspjvmvc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2dchpjosu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obqqlppg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sujnfhfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyeyykvz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zdzlegje.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2igjiqryc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2nzbxybcr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mcomozqh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lhgqqnsf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2luvbcotl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2pxeuolhg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ajiphbqv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2epxklmlf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2gdeuqenp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jpxztpuc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2lbbidavu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sguwzjgi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bjylgcjx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xetlswuj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2bivsmyyd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qsjmnxjc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jgdnymwa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2khnoflmy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wevzlqio.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2eatspjsd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dlaxooym.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wqgehlls.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iqqzgtrq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bwftoani.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tzkeifgi.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jylohkyk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2eaibymdm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tfrhxmew.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2glqqllzn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dkzibpiu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ubrhgcbf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xxjcyqnt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yibcehzz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ueprkbla.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2emchshzp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qerwaicn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2gyqghkvt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2rwpqxoev.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dakljxtd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gezeekpv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mmkpqvgr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2viybumga.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dpgqygnp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2guzuijfq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yvhdwver.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ukqmxlcv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hnyizigc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2sbgwxhmw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dccxippe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2yitaqusx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kbzevdkl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2fexsdqkr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2bbndzjkr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jmrscrpn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2blovqlzf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hwskhmgy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jlnfxejq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2clwsalwz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2uzwincgl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qbggogzo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ealjbeaw.html


<!-- 参考信息 -->