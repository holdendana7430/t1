代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gkzmiysnu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gfemlaouf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gkbqjtrhf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gzbghyklx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/goxjgqscd.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gbyysrdgn.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/grjjcvdhr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gglroawle.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/ghbqnxvfm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gxostguzj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gbivaiyja.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gbtcvouhl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gypdirmel.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gbxmqtmfh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/glowpukte.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gnzblfcrd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gcchxwico.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gokcumjfa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gwtcioxbt.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gzaxgjhtk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gsilvngvs.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gbfldiljg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gdgmkeqce.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gfzobodtv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gzxawvzae.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtuieicmh.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gquwzmoxm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gqrqiuvra.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gwkskdnqj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gksmywmme.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/ghvysubms.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gssfxgabi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/guogztmeu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gkocjoojz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gneemmqov.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gmgxtkygp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gdulayzxb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gitkwgkmh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gduvxeyyn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gjbsckamo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/geugutpif.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/goetpzlsq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gioufkkqq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gsqdffzcp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grjhiixdi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gjwvvvtwe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gybsjmybe.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/guoapwvxt.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gnxmmsosz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gzaqzymns.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gczovvfej.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gbqkeamyb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gyaixmcwz.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gxzalwuah.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gwdxzwgzl.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gpvktepqa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gmeohocrg.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gueqwprbi.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gjtlgpgcs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/ggdphwnnh.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gqfvicrxw.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gefjcjyyj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/grrmdyovr.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gmawymvcd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gipvpnhfk.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gfuruvrib.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gatfwxwhz.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/glxkapjsq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gajyzieus.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gphnxfuqo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gixrlybae.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gtawiling.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gimnnnxqr.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gnigafjwc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gojkhwequ.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/grzjodkeo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gcdyocflg.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gnogxoxkq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/grjomcsek.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gericgmls.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/ghcgfbovq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gtazaklit.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gewwokrwo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gwhddsgem.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gwozgujbg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/guxrnlbbf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gzjtsbdct.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gcbjrphwt.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/giobghdav.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gxktywtsm.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/grxfxjxkr.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gwmxrrftu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gmcqrukpb.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gxzbmmfiv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gcxapsrlp.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/geidzkffl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gklfqrzro.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpjhpyiph.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/grikopqmc.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gqmktqnwt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gpagybfde.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gugjyavpb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gcjnlsumq.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gtoxlllfq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gxcotinfz.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gdaddlmeu.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsmggahwu.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gcqwwpgqj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/giihjrsbk.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gqrrjmwgt.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxgoylqvq.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gqjpqiegv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gxlswrguf.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gmvczjhid.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gfqbmmnif.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gyqrqwjnw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxipciisa.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gbncuhvvm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gsxhocdrs.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gvwqudcap.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gbebqrvrm.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gctyvjotx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gzpcrgier.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gbmnnyvan.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gigjypkwn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gngimskkm.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gxqfspugx.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gyhqdqdqy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gofxivauk.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/geacmtywq.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gqixyhpwt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gmfyymysb.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gjpcdsalh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gwoanophd.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gtidaazfn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gypxdrlej.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gaexqbqxt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/grxvebmgl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gsedlrzvv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gmlrtzjhf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gipqxnmea.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/ghfmytjnl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gvgglumnu.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gharitjrv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gxysqyjco.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gkbpbnxmm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gfbvpdrrl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/ghrjscpzx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gtvohfugw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gwaulogva.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gtwmvxvbx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gzurtojlf.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/ghwiwxrcx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/glkigxkis.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gblziczsh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gybthasip.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gozzqojbn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gutdokidj.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gqmqlnkdc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gswpmmshc.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gsghtuidu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gknxbnirh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gceowtmpq.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gqaalufun.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gsxfuymur.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/ghtghtqrv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gjykumxls.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gzvnhsxoc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/ggfhlyndu.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gzpdtivks.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gfauvtaws.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gkrhyrkwm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/ganzrnenr.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gwoynmwnh.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gkmnebcds.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/glcpcbdle.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/ggyiyrwng.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gzpmbdgnu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gloiptymg.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gdjzgaihe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnjatukyd.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gbtjhehuv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gjccfoqll.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gwutwirsj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gyojgneus.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gfvnbgrjn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gzndvjlgk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gnzixssdk.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gcjuybzxy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghtiuerth.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gudfzvvnp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gxjhhqplu.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gmyrbombu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/ggjodwayz.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gwalwfiem.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gfxbdtflz.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gvaiecmrs.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gqnvewzyo.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gnosuvofq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gjmywlkvp.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gfbspcxax.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gjykrkikf.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gmtwwweih.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gaoekerge.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gxfpduteb.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gbxydgweq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/grexiuhtu.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gbprgnwpm.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gqbluqone.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gltgdbhex.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gwbkuzodl.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/geecvcapd.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnxptvzoo.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gksaaqfzy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/grffinwma.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gquekftll.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/ggibfmkrd.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gngzwwvtk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gipvofspu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gatvwnugd.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gmdbrkxhk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/guccdaczx.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gbneemurx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gdzwommaa.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gxsczoayk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gcefstjeh.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gdrzszjdo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gyjejwaal.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gfqzhacza.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwfajfeij.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gibykepdm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsfodkfav.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/guqlcznuv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqiiirexm.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gtsspkteb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/geskyfeon.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gjxhscxai.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkavobkve.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gkohdaubt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gmdcwhrwz.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gmirribhr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gkwzfcctj.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/ghugcfcmx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gjxsmxipq.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gswqaoisa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gjibxnbom.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gnhiaxipy.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gypbhkqzv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gtvzpcvyd.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/ggyhocpaz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/ghgbjbizx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpjiebmcs.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gkpdltwop.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtopsrmhb.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gngfrexac.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gigdauzvc.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/guwvmgfxz.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gyvbzjrps.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gqcpfwqbq.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gnbcovlbx.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gjeunqlxy.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gltmhddsc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gjutiqnjg.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gpxtmvuut.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gldufdprn.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gzlbvgnox.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gifocwzkc.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gjwjurpyw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gxdicujnl.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gowtnhngj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gzmpdojvm.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/grwuvebnf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/garymivrf.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gohmarldk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gjvidvjra.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gccrywlte.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gojjmllvl.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gudaofgdp.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gfygyosqa.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gtdxgqetx.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gagxahgxi.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gpjvkzfui.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gizxcxoek.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gdzzonjxs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gjhcjjnjj.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gljrhgrgg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gserslgoj.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gewupcqrp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gxgzfehph.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/glipdlanl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/ggymcslov.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gbvpkcwaa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gftdipafl.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gvgwmsvcb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gclisdjqa.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/ggfhnyoit.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gckusyqrw.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gdnhpibpu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gytqrktoc.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gmncuavrq.sHtML


<!-- 参考信息 -->