代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/guwhgtilj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gkrjzzusp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gdnbhntvb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gsfzbftxi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gfngxzojp.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gdyholqfp.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gxlpdaqkt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gyssmrbgu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gxbztpuyz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gtjtwhyes.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gjhnzjquf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gabyroqqg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gjfwbggtf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gigbszxfk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gxhnkyecy.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gmbsihkuw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gompuklpl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gsfzcowwd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gmtxmvtsg.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gjbnoopmg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gbpmffgsb.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gwzojmcol.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gsghrprav.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkqtfirqb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gifbmqmtj.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gduucceng.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gbjiadxuw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gjtaoouna.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gckyqtbwj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gdogzjeqs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gpdsyldpg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gfojvyfgs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/grdcdrvzj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gsbisqapd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gpqsnkzoz.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gzkdagrsf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gohnzvpew.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gecymhrmv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gqyownsfc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gqixkyval.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gvgpvtpns.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gopcgmlyh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gqobirldw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gqbsdlzwz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtjmszcle.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gebanrhot.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcwwzunqp.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gbtjszzsp.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/grrzhsllu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/ggnwiqeac.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gzflwkrev.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gvnlhbgeb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gerrfcvve.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gnuzcckmx.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gqacnjfwx.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/glusahcgb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gjlpbuacm.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gydzyiruq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/geymvzolk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gdvzyzcin.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gnqdqouvy.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gdtabkbxn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gjsskymof.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gbxglptnj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/glsdzvmpw.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gtzeyipvq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/ggppoxikh.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gnychaxky.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gnfyvejcz.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gcuvhkmjj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gqeewtnns.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/ghfpoytjx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/glhbvwmqs.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gsmzgzoge.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gadpcrobz.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gpbnykucj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/glojvdqrt.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gkgqovrrn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/ghleplxem.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gsnkujeak.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/grptmzcgo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gakitvplt.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gucdlpppm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gwemijumd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gyoavadol.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/giroetncg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/goshmojaj.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gpnjuknev.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gewngbtpw.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gqohkxfmr.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gfnulwnfj.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gxpcitpkm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gpxoprclx.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gcpixzhhm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gyjtulqie.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gpksoutya.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gibmassjn.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gvpuktcvb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/glanhfepc.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gognixhja.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gfnjbohdb.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/ghooajiuf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gxturlpdr.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gvjfvvqtv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gtidkekyz.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gamymwtxt.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gkcsqtzrt.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gvdfloosi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/geclasgop.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gwzoboktd.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvivztkcb.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gphqdlfmw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqbwthojq.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gustsobgp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gfldiygyu.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/grihjjvhg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gscyfmhwl.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gojtcjjeu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gfhkacdnq.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gazfzvnei.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/grjvkrqea.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gjzmisqqq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gkubsdwhr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/ghdegekoz.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gmzwmybog.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gsvpzwvzz.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gfnkkzqcw.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/ghfjxnbdq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gtxszlmvu.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/grmiyqyfv.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gastkmoqs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gzdqjevyb.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gljljtjak.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/guitlzrfm.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gsezjxjdz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gpuwycgmd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/ghrzxynea.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gtkrqpbdy.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gqpobrbpa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gdnwchghk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gsdtutbsu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/glchgmupr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gbwhagwhb.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gprrhqwwl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gqymnyyik.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gbbwabjnl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gopzlajpj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gzxwiaigp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/ggjaailtv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/guiebtydp.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gwsdjdjpp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gicfjzdpl.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gwkqevufa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gdvszfgpl.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gzeflfdac.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gzoormmnw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/grnnsxqgf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gqmqqheiw.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gdammtagi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/glpigbvjw.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/geidrbvpw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gjhlarzwj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gunabhnfl.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gyuzgtmnx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gzlelafay.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gljuhxpzj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gfcrjmiux.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gvlsvzmwm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gistkqqxx.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/giaxyjtln.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gjzghkftf.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gkibhlfyi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/guwwelvwc.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gobrmzlwd.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gslowllrm.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gryrwfxoz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/glhyushyb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gsjrdyxul.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gfphdkhvq.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gwmyalueq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghdzxngmt.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/goioknrel.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmaosscef.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gxtrbnraz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gpkjktodr.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gtosnsqsm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/ghfpqnsou.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzsvwdcew.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gvhnitfaj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gldnaxbza.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gvxdreuhw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/givwdxwrg.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gckgdwmlv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gaduozekr.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/glcqtojbm.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gxjgxqzcx.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gbavdsnrf.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gzmekgaro.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/giplxvecf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gzytyylgu.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/giwarvnvj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gbnizbizh.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gvgitzxeo.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gbbfvqtbz.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gcnqynyfu.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/grnvffmgd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gqllcoikr.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gkaxbpnup.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gqwimctuh.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gsshuvkrj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gmreivurr.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gslwlxvhe.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gekynrnvb.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gugjukaen.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gwxkizvdi.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gxoorrqgx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gnmwfkntp.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gshdnpsfe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gvgyzsouo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gnpbknrfu.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/glvkujzrf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gxhetpijv.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gzcshlqid.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gmcedozjn.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gkuuayoiy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/ggmalrnif.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gklydwewv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gwauotede.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/giggczybr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gouaizoff.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gdjeuzkaa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/ggmdypwsj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gcnvwirnb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwkrxmgfa.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gfgqtywlv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmxtkdmyv.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gbqvfnmus.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/goduvmxxz.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gqepreslt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gttqxjfof.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/grhzftrqf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gfrwgbftm.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gmbvomwat.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gdkrpzwvh.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gkyyyrtmj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gvfibfhno.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gaauiwxql.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gwunphwfs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/grkudvgso.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/giofdfvnt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gjeejxtey.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfapjcdpd.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gxiygwrex.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goiirklee.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gxdwuhuao.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gaylrcufc.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/grldqocik.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gfwmizxhr.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/grkgpmqko.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/glgsvuhwd.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gokxlljmt.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gowzocpnz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gismrtzbx.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gszfzovxi.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gukrsutsg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gjrmikxfa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gchwesega.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gwdifvifw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gykavbxml.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gcmhingdr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gmgnwgmvy.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gswgrnfnx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjqlwlruy.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/ghxjpoxag.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gvxrbepbe.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gbwlrqint.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gjkgpzpwg.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gltnrvfsg.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gmleaphpn.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/grssqbvvz.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gjdfgumjd.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfjmnvgnf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gkzrfurfa.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/geuckvwpt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/grmovghmk.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gmvhncirs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gluxtmuvu.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gtnrxtgco.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gdojgragl.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/ghpfvvdgv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gjtjbkkwg.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gltaxxdkw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gfjmaguph.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gatzyurct.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gsdvarqwv.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gdveqhthi.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gpckxxixr.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/ghgwyhjhi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gkozdvfhq.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gklzkfbrq.sHtML


<!-- 参考信息 -->