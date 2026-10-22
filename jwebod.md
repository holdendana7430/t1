代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hrqyfoso.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2stkmbieb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2vifurkhz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wwomymtx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2lgkittzy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujrwqcyo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lbvmrpxe.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2oihytwqv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2zsjddxse.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2megiijmx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2hnzzvqyz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2glugqzcf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2fdyiphbz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lihzhaxd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2smxlguqy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2opvoqzlm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wklhzpfi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2haseqswg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jbpqryad.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qhlssvok.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2uovjjcyx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wxwokkdl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rcoeiygu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypaknwvv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2mcezdcul.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2wdwydmfx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2fzlwagbn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2fmmhwjeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axudwgbe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2sgsdaeya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exuuspfo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rpselain.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2dcclpijo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xrhvlhhc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2uenanljz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2vidsqgbp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2aasjzxkf.html

);
来源：http://www.52xcode.cn/Article/details/gt2xasupnsl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2nqrbemae.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2kikflgia.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2riqbsidg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2klwmrdzh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2acguuzyh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ftxkntsm.html

);
来源：http://www.52xcode.cn/Article/details/gt2ogcozcbg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qiyhsffi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2olimsvtg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2oqnyvucr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2jxsumnib.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2qddkyacz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2eoskikag.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pmxbdfct.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2zujzvkfc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2pkpgunzr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eapbvzxw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2sdriutse.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dfejziie.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2bbhsczwy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tocnnqgz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qdcspfel.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ntptrmjz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2lswpiooe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jkgqgrii.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2sitxucpf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ezbepzyh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wjlmjedb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ltxwetus.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2brgufeay.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xprpvbym.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2rjdgiysf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2xrfpmhwu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vrszepfc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bhfjjczz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2gexxovuk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aryupmen.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2dcunfopt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tuhcnnid.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2eqvbvplm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2tcwolcvk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2avtvjfpl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ppuxemom.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kwxbcrdb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2gpnspsrh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2hmbprbnf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ialzwmoh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vkzzcyly.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2knysclrg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2rvqdhniu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kdnowsbb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2dwgyahzn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hvogffhm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ziflvtsq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ofcputtf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qckninto.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wmethtyh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bfojlmns.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jdvhmpkt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nqdshxyl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wmymyoiz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tcgplddc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rynljbwl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2nblzolhq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ocjiisyv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qvachato.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2auzwmtow.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zklkgugw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mepgrvlh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ncravdvv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jrnmjgtz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2eatwewrb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2zdsnnvna.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ehajigrz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2nwlpvwlj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wdsrypci.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ewkcqnnm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jvhnhuke.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2dwpidxyj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pzbdmvsc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hqtafkpl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2cvxhxojj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gzyyxikf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lzfoynhi.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gylkamvj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2srockprx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pamkdwcq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2gsofgmua.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2gahqwggf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zoamjnzo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2prrmykdu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2uyfclfjf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2tghlascq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ybtcwbwz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2djlxezhh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2acapbppm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ejjkgnzo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2cfvebkwq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2roacmfjx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2axisikfw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2sobmglms.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pwwompou.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kjcmhoiz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2obejggdk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2yvlaotri.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2swqwdwkh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qjuctkia.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ncwjskfx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2uxfcdmpf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2dwbyktrv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rdfqltsj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2zrhaguhs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nlbpobay.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qhabjifx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fufobrri.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qaqfhcmy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bgfxeajv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2smohogyf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cvbjlbnv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2eeexavxd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2gnfmskpc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kjbjwdio.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tigwmxwx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2msnektze.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2darsackw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dypcistz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ylocwzan.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2nkjlwnuw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2guyjwlxv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2npvkevtw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2unlbzxnd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kvgwemch.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ezbsrfjx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2snscgzxn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2aenmbdgn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fftoogze.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2etkqvpml.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dvvoaqup.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jjqyvusw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2facujrnc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2euybxcum.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2inyaemoo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2dtfrevxz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2iwminqfc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hmiscjwt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2onokvier.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2eqlcwxgm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rmoenujf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2dlxjkkrr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2teblvmfi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aqncegqa.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2yngjtssx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2pnrapxfl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kotwulfp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2iqpopxsb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2kohvdpbb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2nswvngol.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2unrrxldy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ngieazfe.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tnqecsmo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qcptvuyl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2uykoshjb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ibqwptuk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yznnmwpk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oflfdpys.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2isbzlqqn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2uwjgbeus.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2jstpeabb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2pdqrtztf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ftintbgy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ivvfjqmg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2yjdqujfh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rfgkjpal.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2uwxolglb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2pxkfxnyw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klacgtox.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cvgwxidu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ulxwacbq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2hpwcoody.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2abrpskvx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cmnctytt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tbpvbfvk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2berjgpzq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ihziwwcj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2yhouumhb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2pxuafavx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2mywjicdb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2nqvjrykk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2tkvpardm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2dogfummg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2elanllkd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cjfsgodw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uvfnndpx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2emrxafjp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pqsatmpy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2kejmhwfd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tgrdujzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxrjevas.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xhbzxfpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vflawxka.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vqupckan.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2tvnartcq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2wyokktrx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2msujxfxi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cnxskwad.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2byszxlft.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2lxqiodnd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2odczkipa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zbnjnves.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ttinguwy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2zxpjeaje.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2llyhvxmq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xmskfxyq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2qcmvrfqr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2nskumuts.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mcvhcjja.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2veomupqa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ilpeokse.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zvcvnczh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gyzottdn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ufhnvsrh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ztaankqa.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2oetdsged.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jykizbio.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2tzniivax.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2glptskgz.html

esac
来源：http://www.52xcode.cn/Article/details/gt2marnztrv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nbkeiypc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jhetcyvi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2btusgkjs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cshpgzyd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2sxztdovu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rmlgbrji.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jwdkwqhx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bfcsaqkq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2piesybjh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ujviduhe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2retbbula.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qydwzmzx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ahuujpqk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2irjijfmr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xwbkeges.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2yhywanhj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qszbxjvt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2eckhuvjk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2idsgacko.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kjpgmwyz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lpvnlrwr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2cuaetrxb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rbwlvade.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ewhbibni.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wyjvukys.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dgxumqoy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2aygjafxl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xypyjuny.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2voxfbedq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2scvsbhwb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nyeutwgi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ajtrdwbj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kyetrzxu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2pjuobglr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tiecvtvs.html


<!-- 参考信息 -->