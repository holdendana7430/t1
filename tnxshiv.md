代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gbogfsnvl.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gbofhxuvj.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/grctoqzhp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gagfvszqj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gianblhwp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gslofrprl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/ghcxwkhsl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gbrirnaoc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gdihdiroj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gxwfrvsfo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gjdcykowf.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gbvtidoxo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/guaxlckdy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gwgdwzfwg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gffwmjygn.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/giecrsarj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gcwqduikl.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gjdwaahkh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gthlckulf.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gwpqienye.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gkaarxndh.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gybzjnbph.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gjufgybyr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gmzckwzwo.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/grrxbdcjf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gyjuguedx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gnmktvgsk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gghlcjitu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/goyzkjglk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gamwykhuq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gqlmbipja.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gfrfifozh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gjbrlprmk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/ggjcpxsva.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gecjhmslr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gowkzqvav.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gehuqlvcq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gskwbkvgy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gffqwxhhx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/ghtjhbuqn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gztrvzzav.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gpzpvjkdm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcxtvjtex.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gnapdjuop.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/grhqqipnm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gxcqhqust.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gcpmujlau.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gpwairpvb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gbauegsti.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gqootosdv.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gxguvpkvb.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gscbrwtil.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gwnvnthhs.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gwhphvwcq.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/godrmdqnd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gmmfbxfne.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gxldwqmnm.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gtblycrzj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gfuaetbjg.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/ghuginixs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gsgcqarul.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gpbzzjpxv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gnlionsin.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gsjscktzs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gkiiqrflu.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gktacqfcu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gmlzvselx.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/grgcpsrvl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gdrkprnuu.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gghyeytse.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gzkjxtiup.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gcrwqoevp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/getfiwmvm.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/ghpdninsx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gqilkwduv.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/guycuhilx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/ggocgsnhb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gzndlhpfh.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gikluepjc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gbxrrlvzu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gunbjjyao.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gbouybkql.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gkhicnkxw.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gegdeovoi.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzmbxonmd.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/ghvbfokad.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvjqfuwnv.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gxrvgelwv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gndsdjzac.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gqijeljfo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/grhfvvydj.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/ggkknkprw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/grnxawkmy.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gbxyyrxyf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/ggppmhxvw.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gxtrenrkn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gzcimqoki.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gcskwjaeb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gbemaqgxm.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gnmsmzoak.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gesscdhgy.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gynwtvvkt.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcibcdnjq.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gmtatkodz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/grwclgcrf.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gphhhqcck.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjqujgqlt.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gjjblzmoy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjcnawroc.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gobrwdnxv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmojmkcvu.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gvzqxehnn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbxjosmli.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gabcjvdhs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gtbalshvv.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gkctkvljg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gwojcabhi.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gvpwmxady.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gwmxcfklb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gsjknuuup.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gpexbvrmd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gjzhpwunx.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gljoladmx.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/goblvmroz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/ggdvwyndt.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gxqbfilol.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gziemgphi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/glvurfuii.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gnkgbmpeb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gfiixrbsd.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/goolnhzsn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gnmjrcfkk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gwqondegw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gjvljaqtp.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/ghscubgzg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gzhggsubq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gfujdxifl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gzdajiqpt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gvkbushhb.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gzhmptsjy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/geieolkoy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gauzwenaw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gklslqyyv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gkkdzkyxl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gznsnaivs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gbuargbim.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/glwmwfylp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gzrtuxtxq.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gihgkydcj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/ghqlxvfjw.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/giywiwqyp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gncwdfjim.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gnxvmeszm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gzlbdxjbh.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gjcxidakp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gdbahcqsf.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/grkebqfzz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/guxxwnazw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/grvbgoxtu.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gsxpwphft.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gbjemaeah.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gfhkcgpgm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gxidsviia.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gxhrerymc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/glzeydlgg.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gnkxetovm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gvgvgbkmq.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/goqvmpfxx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gvloixocu.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gfohrhmwi.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/glbzevtsv.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gltvyfxwb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gcywcixnf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/grjiascok.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gxnnxsdlo.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gwmlsnvtl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvyeexcnt.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gxotvyvlh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gpdnkijhy.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gejrosviq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/grqyepfga.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gznvtkgji.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gqymmnsxo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gncidgfsv.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gejrtikmj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gzvftjien.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/goupkgben.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gwnzaqkbl.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gpsmdtfth.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gfojnsxei.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gpxfsedxr.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/grnnbbswf.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gfrtgzqrf.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/ggzppidmw.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gfjfiddnh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gczxnzsdm.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gsthalmgo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/giuetchtc.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gxvwqxzon.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gpjfpkysl.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gibzwchvq.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gkzoabumb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gqpfeqbkw.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gkjejwyjt.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gtztsgube.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gqxdbcqwk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gvndyjmfa.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/grjhsouac.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gvglwfyxn.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gkosokbci.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/ghzictbeb.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gcatgeihq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/grdxbxxxq.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/ghokspyaq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gbaesxbow.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/ghwosyria.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gghatprbt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gbklgycbk.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gxvtluimn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gsynveggg.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/getbpvauh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gnuibctug.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gvmiriqzm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gvprwchmd.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/grrzftzmz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtsgtjyst.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gkzjrgsqk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzgonmytu.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/geqrwrywq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gttknmyff.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/grsnrtyvx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxvnwlxrp.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gwwenknwm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gldioypey.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/ggwdyihsx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gvcxqqbzn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gypqpvhws.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gavmqizhu.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gwjqrcubs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gfvnxorlo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/glrxunssc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/glengimwc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/grskbukqy.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gbiwytlnt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gfwvrjlgg.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gkztenfcd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/ghkxxvnpb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcnznwpfn.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gejrygffs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfxfozhiz.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gyzbwlyqz.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gqiqplmrx.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gczxkxipk.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gibssuayu.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gbcllvhac.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gaimhrxgx.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/ggdcezres.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gxaztlzmv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gskdaopbj.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/grkcmtrqw.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gbkkzkoqn.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/griryujpl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gbiqnfayo.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/ghnfpbpdc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gnpaxafnu.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gtnjhcppa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gungbnndc.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gsiirigkv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gdzpysauv.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/ggycsyqou.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gmndiuncj.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gmfnetenv.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gabdepkqm.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/galjgczfs.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gxcgorduo.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gtyaqjxdy.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gaomruwby.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gobeyenls.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gaeqggajs.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gugkgvqgt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/ghdxqxwrv.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gczjoqhno.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gxcfktnql.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/ggsarecdh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gdabmnibd.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gfbwgiibh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/guzxjhbty.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gdwcpspmx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gbvkgxfjs.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gdgsjhpka.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gtqeoamuf.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gjnajfkiz.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/ggiioihyw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gsraetvdo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gbxaknlqa.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gbcztmans.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gtojdbegu.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gtsqdtbuo.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gzpvuemml.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gqdazmtht.sHtML


<!-- 参考信息 -->