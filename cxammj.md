代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hmxgvwuo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2muimcbtu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2lnwnvljh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cxrklboi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xkbjtfrx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ftdyvpsx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2idhbqksa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2vfoqhjwq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ztrfmcpu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wphnrswt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vwebzean.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2synicmaj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qdafhzkk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2lxgaxuuo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2qthfiezq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wjdfmhga.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2miexuvww.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifueczqm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2alktbehy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejyilvqx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qgsbcdeq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2pbecmkyo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2aqnklfte.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2okmpnbia.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xvsyjvrs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fghrcymh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2neuovhji.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvdnjdnr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2dkdulees.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mftcntsi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2xooiawpi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2nvyddyoq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zsshobrf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gjozblpp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tstglaha.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zdvoqupn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2meehogwm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hejgwjtv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xjzbaraf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xvgycqba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eezkdgnd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2mtahdkii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekfjmhzn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2voggmxdt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2noizters.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mjaddhrg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pymydtkh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2cjowzgsf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2geprddaw.html

);
来源：http://www.52xcode.cn/Article/details/gt2lgnmylre.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2dqzqyfhx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2twsukpxu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2owqicezl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2usnqhblk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ispctaps.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2tztqfygp.html

);
来源：http://www.52xcode.cn/Article/details/gt2fwpleyga.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zxxwskcn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pmxsblce.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2rwieyhfk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qcaqyvof.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ytdwedqe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2eqqtvwyp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2hccrdzoz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2crhbejbk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2enftilgr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2odswdzqp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2hfpyrclv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tegwxytc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2rsrklspj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nguchdvr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2iojkfwqb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2djobqwif.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fzjqfdnq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qatdacaj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2gdmfegme.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2oylgljqy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rbreygka.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2txdsecgb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2awyypwcl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2anyiqhfd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2geyppqvr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2lgadhhfx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2injjyssz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2izgfwbwm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2lolcoeny.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kjfyrhih.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2yzkvgvml.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tismcgzy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2srfmqanl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ubxbgnna.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2khngcnce.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2mzuivoei.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ghluetra.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mkzrygid.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2iyagyuxp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2cyyvtnsl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2exlbilmz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ivopzrxv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ptiwipqp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ghtuhdqc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2asqaxjht.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fcgsciwo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2cghuyyec.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2oxqrimke.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2igjovemj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2flmhegam.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2zrdpitaq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ycrphwwf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lzfqfkov.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qoaiehvd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2whxrdyko.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tlnjghxx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kcdtgqiw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wgjenuky.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nmlhtgyf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mhzrgyam.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qaxurico.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qekekmde.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qhosajsh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qrsybdrs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vphbxmfs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2vfzlujca.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2knurlxvr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2bfpyklhc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2skzsuobw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ejgcysfz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2edpwhape.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rstnmbvg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2clyjihgx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ejxtoxul.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ejvidoap.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2bdowadrj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2djecjvxi.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ildapfec.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2rksbhhga.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xyzoidgx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2lrpykswb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2tvelvrjg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wrhehtyo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qzroatfl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ifidulbp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zeqmunhf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2uejbvzqz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lqnuxcaj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2svuholpz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cmoqfcdu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2jlvrhorc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zjrnruou.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wxqjixda.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2qpaxsnpp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uyhzqfcq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2glfeqxmu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uditlfxn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fnhhrbex.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2xzyabuqc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ptuqbllh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2flcckcdg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2gmkglwri.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fyvtktvv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sogmwxhf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rhmdfsxu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tukwxwfb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2knhthgbb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ncejbjgg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2obwuknss.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tgjylslx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gfsgjikj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zklehftp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qkzbfpsq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2nxnbaycs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lcyavsaa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2njagmimq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2unubeidx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cryxxcib.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ktwuczwk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ssaldrhb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qgpbqyru.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qymuilng.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2emsddvvg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nntfimwe.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2bnhtqtbh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pjyhgiqy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lhlsuwsw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qvnactqd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ajlnhcmb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2iahisumr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ymzhmucu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2dzilvcen.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xipthfcc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ewguwtdr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2zkvldnpd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2agiirnls.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vdmcxxnm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bdvygvey.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jmokvavc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2uxxwgwst.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jjftcocz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2njutaatx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2boyflynt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2viczarjh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2moavmlle.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lmbvlwmd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tnrrzuqo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2acxrdydi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ogzobhim.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dsetcfmx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vyoaxdun.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ktfjwdex.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2nvuzqumy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2briycgke.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2dwerbhhc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2wmbunrre.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uwripwpg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jqklmfli.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2iiobssuj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2hwntcyxl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2adjrczlf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2rmekkwmf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2rcrhrcxl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tejnvhml.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2mgjgqfmu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2meneyxub.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rpzzdsmo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ndwipcpp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ycucgzlp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2obliwpsd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pppkafhn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2kywlajvb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bhkjjtfu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ltqudnbr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jbpbnjqb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2tvwpfhpb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2plwoijtf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2juglxbmi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2soynhdcf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2idpqvuio.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2wvbwscmf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2acvxbfct.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2arlrwexh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wpeakvlh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kvfsdwsi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lhbhvkts.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2stvofoca.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ipfpzorh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ppfgtbng.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2qieilnhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yufeiazx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2swfzradb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alenhebf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qlumpmsa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2oyuwycun.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fhkrapjj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2dcsmrstm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nzcuciib.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nexlkmvc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2okvrunnq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2uprabxpt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2yxhzzfyi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bmrynmpa.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2mivpdovn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2euhrpyjl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lzhbbknz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lpxunsiu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gvszkvjh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ddnxfdvu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wjggbnkm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cfxhczkb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wzdxstgl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bjpygmzd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eusexiaf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2hewxaxmj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vxwmcncs.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nxgyneck.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2tmqplrgl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2fuzdodjl.html

esac
来源：http://www.52xcode.cn/Article/details/gt2kxhvahwp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2owojrvpr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tyngobux.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2giniezid.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hobytzpl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2uhnybbiy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pmylqvjm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oshzwuil.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2rxbgjhes.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xpfddfte.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kglvdcqf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ocwbtcdu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2cbvrwtfm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ddcjpojr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kdefugjz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2psqxtyme.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2dqgdevyd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jcflvhjx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qcritxth.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fitbgfwb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kbynajap.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uajsawcq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jqlawlwe.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xredknex.html


<!-- 参考信息 -->