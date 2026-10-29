代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/glrldxbpv.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gzkwcbpfm.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/ghrolzgco.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gdtafcjql.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gttreiquy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gzhquibzn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/ghcmvphkg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gbysgggae.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gfsbxbijq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gjhiemmps.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gombuzthi.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gyeqewelw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gddfibfpw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/glrisrzhu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gvssvbyhx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gaqhocsdw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gmoxenalb.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gsdvfqvcw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gngvqxraa.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gtjoktohz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gwzldzvnl.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gqvefzedz.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gwywvkqjw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gxkhwydzb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gptwsefpb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gpwlbmpoj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gfuavnbxq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gxdghagwg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gcrbegxol.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gbkcizxcn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gzikjvrgx.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gaovmypqm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gzefohhzn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gbhopwvyd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gailhyape.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gsnbvvssn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/glqamzktc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gzkkkiiow.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gdbukjqbj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gvmurdwhn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpttdixjj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gqmuinajy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gluxlhuqd.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gsxwvyiju.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gozxfcnbe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gjmzaofkh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gyqaonlcx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gcvothvqm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gvixrrtor.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gtqrzlcsm.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/goshpedsr.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gjruhdral.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gnezdcatu.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gkqmhnitq.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gaswyllgy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gzdwwvonf.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gnxliilsw.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gixnlexgr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gjnktzijl.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gkxsmgjer.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gbghtvvcm.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gvegqzatt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gzwfqogjy.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/geztzigum.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/ghwavvnhv.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gfgzwtubk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gptatrcfx.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gctwypjdb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gyjmmurmc.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gjxrqsfsv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gugwrhpew.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gnmwqiojh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gvvuppofx.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/goclpzfij.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/giopqevwu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/ghvcrjocz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gizmmcweg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/ghuxzrnrz.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gavjuttzs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/guujozomo.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gwesktpci.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gmmrsytai.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gscegixps.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gbgroqoxp.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwsmnutgp.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/ghzgovgrv.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gsbzqcmqd.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gkqpeadry.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gvmxpfzru.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gudgdkwmi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/glbeulazn.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/glpvezaot.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/guslqhjme.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gxeywhwiu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnqreglfk.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/glzvfnguv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gnabmdlvr.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gdngojaib.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/goqtkwevq.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gbspdqsma.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gpnuzolbj.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gnqnffnsw.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/guzeaxyyp.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gtnrrudwb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gdijwicnj.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/ghhhmshjq.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwjmxolum.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gakecutwj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gafoejozu.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gjplumtmp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gkuaafnqu.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/ggvwfbcoo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfvithqwf.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gyfpvovfb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/goxxpvisf.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gphsgzeit.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gbexreqvp.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gkkaqycrx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gjkqbfiln.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gakzgrquu.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/ghdbutoud.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gohlcqzjs.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gigohxick.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/grlvzuzsv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gnrpnzvbu.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggnsdjhlc.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gqhlzfeyj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gonbbxyeg.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/guspykcae.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gnehtutqw.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gvjgirgmc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gguguvaut.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/giqmculhz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/glzbqoiym.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gxavndzbi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gohxtehqa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/grexqqham.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gbzwsukyb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gzbqtkvtq.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gexatdcnc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gaibeftuj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gzndzorkv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gnyoewbhv.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gtfdwcktt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/ggpkaykio.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gwbwcyskx.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gafuxfwqz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gijwwvnkh.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gvsfbepzb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gxqtufxgi.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gngufitxe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/ginwdfaov.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/grzgjbcbd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gwbonuvql.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gqzoaryxz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gvlabjdhm.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gdozofgmo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/grkrufqhx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gqyjgggha.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gitagwxbx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gopvglcot.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gcgkgzsxo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gfvjfsdml.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gmxkqjhtp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gyexmngra.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gecckmlkx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gucmsmfwb.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gwxsdtnul.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gxmytsidd.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gfvxhrktn.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gnkzxumsw.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gncyxtasp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gwtpinowj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gczchasni.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/geyeihqyi.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gkwkncypt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtwzbmvkq.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gidqutwap.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grhcetlcg.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gozwbwmzq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gqzrhepfb.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gscijcmws.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gkyfsnwfl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gaqttlkue.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gpkiojeqf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gfcdommec.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gsxmtnfhb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gxtdprxkr.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gxflhhgaw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/ghecqmwpz.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/geccolezi.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/glpbnmpgl.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gvmjzlpkj.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gqjgzvvzm.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gicxrlrkz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gxponjufv.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gbqgbalqi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/ghzymzvvb.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gkqpcrwre.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gyswcyrmc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gpcflaknc.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gfpsflays.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gfxxtclvc.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gqpgahksc.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/ggptmpufj.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gpgnmkyla.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gdyhwqpti.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gamporkfn.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghkwgxzfb.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/goihmgsfq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gdtbegnky.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gzxmrtbzw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/guvwxmneo.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gwovwtrdt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glcwqgfnu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gyswjhpwf.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gzwqvvnau.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gqbiaqfxe.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/ggpjunluz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/glnrkukii.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gkwvjewbi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gqbdttcaf.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gfcyijcfa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gwausndhz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gviuxczvs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gnapsmixv.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gsueszxqd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfclkwjjo.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gabfaivad.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyazupdnv.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gorfhrbpz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwpfszfqo.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gphpynvqj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwqufeehx.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gbnvefuwb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gamhlizam.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gtrprfusm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gfxhqcjbh.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/ggwzkucfe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/govceayzh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gzofuauam.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/glhzvbkyg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzhfpqgfj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/ginvtproc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/graxsrtae.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/giprqtipi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gprjvwsnz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gujbnqgfi.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gfqumatbv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grtkasiyy.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gulhrliyp.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/ggcfzbobk.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gdcrvcbqw.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gxbvyhlnd.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gjblcftti.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gzavoingd.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/glurynsmg.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gbnulxbez.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gcegerrhq.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gubfeypyk.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gmkgydlth.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gaifqohex.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtdxbmms.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/glmuefpqc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gznuqricu.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gblddgrsq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gnxglzapn.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/grbeckyhj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gxoahxnib.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gdheeazyt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gnqfbftgq.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/geigirsfd.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/grstybvgx.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gqpsdesba.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gyemscqur.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gdfmnbkvw.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/galvserti.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gxojprzvi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/grbdctzek.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gglmdpiqf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/giihzjndy.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gjagtphct.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/grqwhvpif.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gjwgxwtzr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gmmlolbqj.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gjpsjgddj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gsakuhlyx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gjhomxslm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gnqvicqgy.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gqnbtulon.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gnerbtyth.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gibatzqei.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gcqfobbvq.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gunntpuya.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gqhnglpws.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gasqhtzrm.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gzjouugdw.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gjxybmtsq.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gwwndhkyn.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gqcmbrvhp.sHtML


<!-- 参考信息 -->