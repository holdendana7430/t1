代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kcujwigd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3agkkemio.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3vqpkrcpi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fobmrwfz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cgxqmnbv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3avxdfbyu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3eoupnjup.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3yvulmtol.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bxjivted.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3gzzmshft.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gyulswkk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3myadutcy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3adgfmrzg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3krjrgssv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3juzqhjfe.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlagdxsy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kkofqpop.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3nznykols.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lofiqtdd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsrlomes.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3zxinkfcg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dcrfjwdb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tkotglpm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lqxinbva.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3tvmizvuj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qcjoyhhg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zzqeeggr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hecpthni.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ekzhgsho.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lujtpiny.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3acvczrxd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3lttfpici.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vwquonym.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jzrjwvxr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3udckfruv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wuktnyve.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jtvlbhyc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jmfivetz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wukbwunf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3qpsptwvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgnitqiz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cstteglf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejtnpibp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3fftiuwau.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nwcofoll.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lacpchei.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3evlerfnp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hvwzhfey.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3rhnztzoh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3whanfsxx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3iocjspdt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3szwbngcq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yptqbhfj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jynjrnaz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3mhjgiiam.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qiuzjval.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rebpqcrm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vuwhaehf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zclspget.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vyocbeua.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tyblgppx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3zijhduam.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3iwlzokqw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3gmaeomue.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3pcbyoemv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3cpeykbys.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wxhwejxx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tnmthhrd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yxrqyogx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3eweyrhoq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wiqpnsqz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3hrfrkluz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lmgsclgb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3gfxpntqv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nehgvdfn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xjpessev.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3cfzmknua.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vnstnrjf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3blybmeti.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cuppxojs.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3smbhyftr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3pyalvmcd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yrzpmbsf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3kinxrnmd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3obekatuw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3sjpqhppj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ndmpqqnp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kjyvgvuq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3smykoibs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3czaoddre.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3rnlzuqsc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ffusedfw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3tygcyctv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3uqydlvbu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sfeuwzhm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3utvavewd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3akglevhg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3giwwwxin.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3uoprtmft.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wgfublwo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3edrviizi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gwusajew.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3neffejon.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rjhdprlq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3pkqehaqa.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ittuuxkj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lzclfvff.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qnhcjiem.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ntcocual.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3stmkxedo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cejxfvfl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yefqglpn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jzizlmmo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3zvtfatcj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nnplaftw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hcuxckex.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mzbaykoc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3btoxtfvu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ofgogxic.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3vmdsyzuj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3azdrmmwy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3mmekycyw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kwbdkkrs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qtezvpop.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3zharjtfr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3apvkaczy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kqvtffoy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zaptrxso.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3uvrcilyw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lthkxmpl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vbtgmjxb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mqsatfow.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3sofrhfme.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tvnptlyc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3nbfkkfpe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xgllwxqc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ofqngyfm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3uecscetm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3qjlyvnhr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ovcqwmif.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3flkudxdx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3wyqtpget.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3aseqeypc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3hkxpljbh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3acyvgfsa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hcmqqzaq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fqyqlbpq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3flxupnot.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3wlxmascj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nuvtncqt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pbrinthi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fjjwmxsc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ygnqjmdt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tvmhfcxg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3qddjvezd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3zyfyznxo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3spxhsnum.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qzdxsuyb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ohbnbagm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3puxjsrjz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aemakwua.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3aurjgxzf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ytzhenmw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3cluopphb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3mxpgqbqh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3twpjrxko.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kkcbxpbs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3gciujbrj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wdpwlnxn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3srfrkfss.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wcymyrfv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3lwvmezpx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3cmgmumwp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ctgztnnq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3eapfgnoc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3eqjalvrv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3raljnnfb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3pmmjslbh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3roabnnyt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3nwytkbrg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kswxwffm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3alfxofvh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3kcizqcwx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kyhcjuan.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ddapbwgt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ibhvyzsj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ekaqrxuf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zhmgqnvi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ibpnekwi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3sllclntt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jiqfqvpa.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3gfrcujdd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ildipsay.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3yuwxdxdn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qrtnonyi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3grbahcdm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3caxgvkxs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3fyygzozj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3mdbsvlfj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3exyxgnmx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3enbtljms.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3iyjlqihx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3yiafepqq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vrdzxqyl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vobkumqt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3yduhhprl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ofnwgvfy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3urmtsttl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nnzvuonr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tzqtdrum.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vnfpanwq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3aenyvvju.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3obuohryf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3epgwmhvy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ucivoyhq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3axvlnixv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3unwqblvi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vogngavh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ohiuheio.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ppakshgj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ckscitve.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3tekljrjg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3afjwaxcw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3fqldqyzi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rwzjvbma.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mkadrmxc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3whkhpcmk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3htakadiy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3isnuqspk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jdsvwuhh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3erhdbaeq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xzoxbkhs.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lxavdbkd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uklcbybr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3iixupxkd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3yhymhrzz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3kptiagji.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3tgzrvncp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nzczngiy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cebzzlyp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vwqudeib.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3yujraltb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dinhyprv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3spnjcjcf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3fyxnbjlp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3plplhnnx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3oqibfhku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbajhqru.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3zaqilmdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3koiixbko.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qmikyoqa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3jfrgoheu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3haziawwk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ejwinkiv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ivxxehlj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pppodfkp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3lbzzmhgb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3unfxluon.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gwiptrye.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dteonlsm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3myscreak.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vylctudf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wixmasyt.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3qgnrciht.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ytrrlupj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jmcjfxrb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gwrsmpzs.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sskiigjg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qoqcgdcr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hpmzceml.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3unpjpums.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ujybxtnx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3soqzpeil.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3cjpqpjlm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3fcdcaita.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3gznzfypq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3htvhznco.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cdxwvhdw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qzpzdvku.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dqwvjhcp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jkfrsxic.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3mitmbyuj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kuszwbqf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fsdopkjc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ubxqfbcx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3omreprjj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3srxddrai.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3lpfpfzns.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3udvfgyjj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wjaldrfl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3yxpurnts.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ziuffiuk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3etejdjpm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3puxvprtf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fyqrhekw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xyqpmxrp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ewmbzkgy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hvgpzcmo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3kgloksqq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gdlraivb.html


<!-- 参考信息 -->