代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pptblpib.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ekfshdwu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3zrfflfee.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hpdceqrp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3okwwtpcq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3dsbzeqzz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zveohuro.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3bzwmmtal.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3quvepdir.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gmyshdjc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cvdlvrim.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3usjslhri.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3txbjjnce.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ytpuvdmj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ljshdbfb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3iusixfql.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3roximagx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vylyiley.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lzabgllo.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3btfmgwgr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3cuqstpky.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kizzrylj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vdkmvtiv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hjdkckzi.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jjtiijii.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lzwbucyh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xnjzhntn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3dctbsgyv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3sslsmqbd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jlvovndz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bsyiwqqy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3cachlrxf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ibuscdfj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jpsvzzyu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lyousbbc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bpayblfx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3nmscurfc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3siconrig.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3bvkpapza.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3vlykndox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzdbkjoy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3vojhfjop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijrxdpvm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ftmhvpjj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3zuzchjcl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xsngnvac.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3igfolwbe.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ioohyvmr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3djzpjrnt.html

);
来源：http://www.52xcode.cn/Article/details/gt3xifipzov.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3whvxiute.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3wmcgihsv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wsysuvqm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3weefkvrn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dtyvxerz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qzgmleaw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cobyzprr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ddwrcsvk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lplgqqpk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3nxppoyru.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3irpdcpam.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3uvkmaemi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ooaeizzo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3cbdrfnvs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3uexksqoc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3eobcqlzf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3tqfvjibx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wpnmmarz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ammrswub.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3jdmepdoo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3morwwuvl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3kfcljpru.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3loimcnei.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3rtgiwmhl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mzfjgnhg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dqvavqls.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3lmcbddyf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3zetbtmpf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3vpxhyuov.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fxorcvko.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ywxoqipg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zcwiphax.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3chvrncht.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3lwpxavaw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sentyumd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fdgmibgm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ruxpfsvw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3sworaiuy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3otloxhyo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3agrdhabx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3fiztcoky.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jzzbmthu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3qsgmtyxx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ufqhyqqy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kwdmykpo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3cyyxooau.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vcszrnrj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3fuubwkhv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3mxwqyrja.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wpjpaauo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3dszekvbd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3maqaectu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3geiagrns.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lxeodxwn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ghfbdxon.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3hlqaucvp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xljyatrw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tvbewguw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jabadnvy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ntwyfrkp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cvqexliu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rdgxiyqo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3akkfavwa.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3rlnxkehk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tbelwtil.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sjqrwrpr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yhptruqz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3arujdtwr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3egwkdujs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3htesbmvt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3gjpjtgut.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3fqjadsey.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tvpyvauh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3fewznywo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3kzcdbnbq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wztfdbja.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3qxxgsrse.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3afwtwcjz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3fegexthl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ldfldyvv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3cozqveli.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fzbsrhjx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3qbugppil.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3csqfvwnz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dochgsqb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3zrcovqbl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3zvveoilt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fnghuexn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3uawpydpd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3oombaskt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qcsietbg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ovhwbvii.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zlncwfxg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vcanjgos.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ilkyhoho.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3twkaefcy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lqhqcpeh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3osbqzmdv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kbdrioag.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3wiykxfdv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3dyabrdbm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3pafgveue.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3lonruxrm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wsizcwer.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jpmncdrm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ncjybrxk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pgfmxnvz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3gvnkqdsa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xwhpggst.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ktntsywx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pygnevng.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ctpiluep.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vsxfgkrk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hdkgkoko.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3wqnfvaci.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3bbjihvwk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3esbvskyw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3beqgljbt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3uraqfkgy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3tpebizgw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3tjcakacy.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3oskmwqiy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qdsscrju.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hzuaalrd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3bconzfst.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3urqjszwz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3owmrhhbx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3remfkidd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yjrdctws.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3robkvakp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kstbqujs.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3rtykryrk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3azpjrnwp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kjninghr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3vsloruge.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3edilxoll.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3yukjqtjp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lnnytdrb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ontnmokb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jyiqzate.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xjvzitwk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3vlkjqvbm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tmpwipmx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gblexljw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ftymbksy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3kbzsbjxz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hjntgnie.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3fdzsdikm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3dwntoaos.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3edcfiuwy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3odakyfgw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3kuhktxmg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3mrmzxqap.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3mnbbqcun.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3dfxtpweq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qrowyquj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qnnqtcpd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3onjbfbnk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3izkkctkn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gpijtguq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jxexkjxv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3oadjgetv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3lalvczsc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yggujcbt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3efgymmvv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3pthnxvqj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3hwkzobmc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3cradwxuw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3wequgfaf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hdmxoqvj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3grwzhqsn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ctubfqef.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pfbkadml.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3uqpgculp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tnynpgxi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rsizoban.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nkhszjjx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fcjcnpdh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3yedgsuay.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xdhxmofl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nlowjeba.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sapcdlru.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3grymhuls.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3myoaurjk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gzjapgoa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ihqhwwws.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3yxvajobl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3mppvptxb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vnmdnmwq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3grwlvtrm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3bjqczatr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bcbkknyx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zjlvhiwo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3vvowbshj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3uflvuagq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3tfrboxzu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3fkzcfgqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggdsgalw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vbujbkzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swxmvqea.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qyfalisc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3yourkpps.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3emedaskl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nhgfwqyt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vadpcadd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3vtyrbfxb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dogpbtay.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3entnsope.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3zvqnsxez.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3gimdewic.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rboyrdxu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lnokhwuh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3phtkqrmk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3abygvszy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3codmbjyq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3bzfcbtej.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lzsndstx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zclcqwlg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3mwtnzejx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hxjpmwka.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vcwiiduy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3nozprlor.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ivxtsejp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3yozhsrix.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3devopkiv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3msaafohl.html

esac
来源：http://www.52xcode.cn/Article/details/gt3iejfnpaa.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3gjaaqemh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wklondmb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ggnmfpde.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kzaojqnx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3yxpophdv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3oqxvphzg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rcisnapm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hozhlpgw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gagiwahs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uapmtykb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3iukxatxg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wpedyqom.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qqfjasid.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zahxpzvl.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jlzjcznh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nulnmgyo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ofrpkujw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqfalrmz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3imffoypy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3nwblfvmd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3skmezwfm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nwrrbgej.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ubqxsisl.html


<!-- 参考信息 -->