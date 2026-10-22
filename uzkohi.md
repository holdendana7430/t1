代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ljkvovbw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jsmsmydc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ienuqaft.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ydyzgfuz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ccitoeqy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2lebhlfdo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zgvdrqhz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vliepvil.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qkqgglma.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ryfnfsba.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2enqqqxpx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zxskpkds.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2rpjzhnvz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2iuybjgbv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xarawtpm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2boevmqwo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2rdvwzcaa.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqsjftua.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zxeauwkj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2mwxuikbj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2lzdvfzxv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsolarus.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2yjtifqkl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2wvmhkxnl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2hpqpvlkf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rcpqmgyp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eaxbqzst.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecjdweyf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2obpvlhvc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2sssyzpwu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2nhhzvjzz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mtycaevp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2sloclprl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yukkesca.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2onpapplz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qyjyijrq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2mwogmqqw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2uzmeobli.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2uzelelgw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2mbivaask.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxitvqvw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ggdgpwfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jeavrhdv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2obvctekr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2beajwhef.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2atzkyhjz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gbawczpx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2djngtcmy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2cstusrii.html

);
来源：http://www.52xcode.cn/Article/details/gt2jvhedlql.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2jqaeqkpa.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wiiiynpz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zrwvilwm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gdezfodj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2qnkvkuuf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmbggur.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ybwjgxbt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vilwpvcx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2totjykex.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2nanmdzdb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vizhturr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2xhmtcblq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2axrrngdj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2oigeygll.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ukawzzjv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2auwhepuh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2pzgryzul.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mdjelmiu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yeexpxbe.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kwaxyjyv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xcxwbkkd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pfqsodji.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ullanvze.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2myducopu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2azlapffd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ksxgeiwr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dfionqdf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zzhfbfkw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jnozcvpj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xjcxphwa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ovglfldr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2lfefwvzb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2tyxhhqsz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2rtiyyken.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qrkohaex.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mnuznvjl.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ahqgmhrq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tojvjewo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wrglpbzf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2apdzztxw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2knkbgmnf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kjxpuhcx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zskcyknb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ijhmvrnd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2svyzdtrx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qhtypaeu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gevtfibt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rfqfxkge.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hwgpcfoj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mcgtjokk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ymupcgup.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cqjcotmj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qlfizpwr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fptiwznj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2njnalwea.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xosfauog.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2guzivpwx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2snrpjema.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lrcpaqrq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2asldwzaw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fqlaftlj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2etnzxybx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nuuobxgu.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2owfiswqw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2axdetlmm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gzzvgygy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nkhxeumo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dviywfam.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rwpqsrtr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2sxlitlzk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ttflvvjc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ucvcibxo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jmmcobhy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2rygcypin.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2usjsskth.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eatibujj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2veiotspc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fulcsayr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2otwduvke.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vtolbtmj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qflkqwro.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wjyqpmvk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2omdtqhis.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2hyxzgawa.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zbalnetl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2tpnqxkdf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nzrdczgc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hkwddzkl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2flhfhlco.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bgyxqzrl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2krtqdiok.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2addejura.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2emaolpkr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2drscinxc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2mfqxkxup.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2uwpvbdzp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ualfidle.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kqruimvd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ufgmsqac.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2xmimmuwe.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2pvfiihim.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kjrxwlyv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ihylstlh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xkyjdqag.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2napaqgyc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zwuogjdf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kkdxvnma.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2fmtyycib.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pyxsmmib.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2zewkckdv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hrpeyecj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wmhhhnlr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2egpmerjv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ilaqajhz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2grtoehsk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2nkzoetiv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vyttoamj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2dmxhbmoy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nsnnpfqj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2clzpphgc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2oqkebliu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rahdcvhp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yxjlovil.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ybmysgfq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ggptblun.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2cfrahpjm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xfgguhma.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2mhjyesgm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2swkdjnhv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ufvwxhvy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2delkjhts.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2tzfqctzg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2fvsbauzt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ksaclflf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qbyupvaj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pppqrcfj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2utyfzxeb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2grqeeqsj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ttzgzykg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ittnejbp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2twrunnlm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2tlaogdoi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uxrlbico.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2sfjkqzra.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2lnvkpjjn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qvzmzgtj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2voevnknh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2hjdinvrf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2dddjqhuq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vyllcmvn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2iuocbruk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rtnldzdx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2clmfyovy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2sbjgwpwy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2adtxtenk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2saozghvd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ajoiyrex.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rxfripsa.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qleariio.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2siwfgeyp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lyiftbdx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ilrfxjzu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2tsxiriwq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zbvwrkjf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rymuwkex.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2jeitouul.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gkdjtibx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2giisohbh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ygmkcaxr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mghjsqoi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2poxafncb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2asmxhcpg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2aavwkrnc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2yazdinyr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2dmwssjxi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ghubtfbe.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bgvrejrw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dhsyuqva.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2tlnratew.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ojeusnsq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bihfjdak.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvamepuu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2vejkvkxp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gpuobqdr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xdgjslew.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hyzpmrek.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2edqbesph.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jkitpwgg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xrogmkdj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dsuvhwng.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2yigbrvos.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2nkdccbbl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kqahdbyj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ruxiaavp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yprigqno.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ahkrmayl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pyqwftfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzygunix.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ksgqbqdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuqesnjt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2zbdcdeho.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2zeluifmk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fzewchrs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pdfqmqmp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kyazsusc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2gdoahgdm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2nlgsswim.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2grdvfmdk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2gccfvxel.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2eatbwsfg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vnqyncwa.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2qbnegdvb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2egfqayzt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jvpvpinu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2rqxfgbmy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hitxjkjh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2dpvszybn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sgbwaqpn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2alveoasc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qvxccfzs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tqlpvjny.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2bciuidib.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2zfcxhvvd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2yshrvxji.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gynrxbmy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2wwhgaici.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2imlsrzhq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzcicojd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wvulphwt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qemnkmbf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rjditeey.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ulmvwqzn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mdiyyuob.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2upceipqx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yznqbzdj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2hoikemmj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2obgmblni.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ucbokzyg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qzzvtfda.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2iyxmfmlx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ylxgyuww.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ixvzwawu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mrqnumlp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2nqrwtlvd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dlpnimdi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vyookwap.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pcvtyigv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hufoijys.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2uvhkuxyn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2iahuvwec.html


<!-- 参考信息 -->