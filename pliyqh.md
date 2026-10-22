代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fvamzxok.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ewxwarqc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wcctckzh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ehwvwqnp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2amffjxli.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zdufholi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2knurssgq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ecujrxmn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2sadctojb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2zlpjqslb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lovatqvu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2cydhvntn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2twiuicnh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ioumzkxs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gtbmyaku.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yulqzewh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2stvkkqvf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fcijuooe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gnofiehq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2eldsyset.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2eypfhisu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btvwnzqf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2castwyqj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2othxkigw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xvlmkeuo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bdbpaltw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pxfsedvk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2oiyvaxqf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lvbavyug.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qlyiofcj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2lpnapvxe.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2gfiutiqy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jejrwuzf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fckzibqs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tyfoyeul.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2juglxyhm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ekmeraxb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jtgbwgtn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2sbwwqewo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2bffkqiid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqpsuogn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2unwlotwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fupiqwjf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2mfseezzp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2cwkoxeof.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pbtbopqv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2unyqajns.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2jwdumouc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gxdqtktt.html

);
来源：http://www.52xcode.cn/Article/details/gt2cgberxya.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xecfwxjh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ovlntxdd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2enrdzbif.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vppydidh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2fukgnkpj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2jllpunme.html

);
来源：http://www.52xcode.cn/Article/details/gt2iifuicxw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2vbcduipb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jeigapfl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2snbtxoiq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2brncxfcx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2okyvfdmw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2onogccsk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2mapmyhzm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2phykmgsr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2zzeqhhok.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2mtisopqk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mybcvoeu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2quauebjt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2qjzjeizg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vhuzzsxt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2yujebqfs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xqdnapzk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wqaoyusa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pjiovvyr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2nalnbave.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2gpqtlswa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2bdlovbgl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2gehtncwy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zoncinhx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2pmbtorhu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mirtjgks.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2qxdikqye.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lctwpszl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eusucpjl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2kctvfeyz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2juukrcwj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2gqppfipc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nzaxomae.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2efetgptx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2mlbtjrip.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2eaaywymm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ntykhseb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2mstuzomd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wyildpgv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xwdqluwm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2fahtpfct.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2azitruib.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2tpzmohbk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2vjvgftjo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vgujesyr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gfjsfqwt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nslolqys.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hvjzeoei.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2eytnwzkr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2imkqtxpq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mqpghegd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sbunpryo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kawpvebc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2azrrrjjw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dlogtfor.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ifavwppr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sktemwpo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mgygwbdl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2elwyemzz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jwetabjn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cqwjmcfw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lpdflxhi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ohxsntcf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2fqxjulto.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qreumnel.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2jyqewufe.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2azaozadk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hwuahgce.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2dodqgiyv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ekhyijhq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cmlnyzve.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zyvnijxi.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ipycejjf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tgymzczt.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2zziporsu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2raxkelcf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2kyhazric.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cvpiovyh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2kpyzoljw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jkffpecs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tjbuuehi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rvbrsuto.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2mvctpuhd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2eiwtxzdl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jtzebjyp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fucmxfsv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zszaowib.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wxxtrfbv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ucdqtvkc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hyendtzn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qbmxesmr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2kcvdtxdx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uuysxkdp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qwegrdhw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2aoiezyaj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2devkzehf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qowaqffs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jxadxldq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ghgqmfjl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vpjjybhb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pyrjahvy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2emtaaoef.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kfqdqlty.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yweeiyeo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bngjcats.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wmtzmncs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hyyirbkb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2cscwvzeb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hmybiyoa.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2yikdlxwx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lvtcazbe.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qujnpnja.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mnklcppa.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2eibrbbke.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2bnpadvqn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hrjyoqrn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ftzvpzwt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2emjenggg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vayvwgju.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2neqftnaa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2byjmwmom.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bdbjcjcx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lfkxhukl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2imzdmusj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tyaerjvv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2pwiujjwz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2bkmivukj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2swaoirzh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2bpellfwc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nynlsscx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jbxeegje.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qmkbbgiu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2yovlqylu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2imqqfien.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nmguotzw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jqswqing.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2rodwwxvm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2execjxhu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2bcplizvn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2kuvntvgf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ltawzlrb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kfavaccs.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2dmduwwfz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dwdjplis.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2vqjvjwxf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2somabqkn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yjavggae.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wkawsqya.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2iedwttei.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tlcefwlj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mbrkfiks.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2pviavjxx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ouzglymt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2pzadahip.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ohtlswkf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2edtiniqu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2fmqylehf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xmldrcqn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ezjxykmo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2oogurxeu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2bgwibhit.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2rtmivqdf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2yyvkviej.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2uclbbdvu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xxtyzmnr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2obljygho.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fvpflpvm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2znphvdxi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2irqugmwn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2stdfmwvd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ekaeepti.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2smbshtnx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xipmqxfg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fmfzffvh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pzzkzldi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qdjhnmgt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2fezwflqy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xaxrimkw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2cwxjvdqi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dybiamoe.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2flihmxdc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ksnboxjz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xkwfnihh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2moijinrd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2cjmtfnvg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jabargxk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rnfsktqm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jvpfqyln.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bkcjicfx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wdrsdrgd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2iyzynaiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lerrpqpu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zgiamada.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nguhxezz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xgerpgya.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2wsaflkdj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2guavjegp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2hmhqctrc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zordacxo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2njffxhmv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zelkxbxk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ozqjylce.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qsktcwfn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ehashqow.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2zaaksfrn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yjgfglmo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zroxhcuw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ergfxtax.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2thoxswze.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2uscutqua.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hdoeyecs.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2diogyhky.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zrrwggww.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ldjrjtca.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2cfpmrlrj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2qjhtunin.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mukhhpdn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mpnxppbn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ulayghix.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ffywecln.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xsjqjzbb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2tsozihvh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ogdzjodq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2owusqlbe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2liwyxewd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ihjkxsdd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wwveyblj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ykqvoeve.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2pxebmean.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2iknqgydp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sibgokox.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2kseaiiot.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qiobnpbf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2sgjyghqm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qxttawrv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iiufuzea.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tuhrwlwg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2vbrdmnwo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rabvnryy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fleobunb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2dcfijgtl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yzxlxisv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bbmpwxxg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fphwhczs.html


<!-- 参考信息 -->