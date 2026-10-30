代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gsmdjodts.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gvwfwflfr.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gddassvvj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gjzmzwwaf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gunpikhmb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gmewthudd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gxyhjcizs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/githfyaar.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gwzqwitsu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gjuhzeisu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gfowrexqi.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/grownymqn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gxaeofizo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gnwwlqcwo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gktrgbofl.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gposupnnn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/geldxkaol.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gtfartlut.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gktdjizto.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gmcrxtptu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/glplbmzqc.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gwfxdqtjo.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gipigiegj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gikunlpui.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gznuwwyhy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gcyxvlupj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gtispsyle.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gcicmqbgn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gbbreecee.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gdsscxhvg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gqjawivks.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gpkxrtwpk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gwtlkndbe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gmjgnsvtn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/goglpynmb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gjbkenuhl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gvblttpgr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gctcyclph.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/galddkxfl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/glohkzrlf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gevjtrotf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gthklirep.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjzgdtdqe.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gdwafncew.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/glkmpxjuu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gmzpduoze.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/ggyjjkbqf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gnaxvnkyh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/grhspkwee.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gtpasfrdv.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gqzpplxmr.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gmjfojqbi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/guixayzmn.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gsqoenbhw.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gkkbuccyf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gxvusdsdq.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gqmgjoogt.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/glggcgouv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gskykzgrk.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gpbhtazkh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gggxvntzj.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gqynaosmi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gwdznlmqw.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/grppktcyw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gsoqabath.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gybueionz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gbexisreq.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gyynmcsyw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gxlxlzewn.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gvvcdtswh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gwmkzdkmj.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gknozwqee.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gjknozfgw.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gbgzvsmnq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gmqfeiuiv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gxksdslbb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gdgdkvdvf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gfjroizud.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gcokkkjzt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/giywqveuy.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gmskfztjg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gvwkvyrpf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gxlwjyzuz.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gdiwpifhb.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqpiioylf.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gwzcpvpgr.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtfwtqulk.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gmthxpgul.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gcnfrezao.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gqvzslott.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gnlbyiwac.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gcqyjdboq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gsjydfmfj.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gxjxfpfwa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gnbncpwem.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gxewsytid.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gqtwaunkq.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/greouwchp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gmfefvnwb.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gpyvobdsy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gbcihnrzp.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/ginyxiszu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpojdvcfx.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gpnrcudtq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/golulfomm.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gsneyfagb.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsqdzblnm.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gtomwjmec.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnqnklpbo.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/glhszqyiz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gfbcitmdl.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/ghcqvmflp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtpgdhdiu.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gazttxrcf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gzjsztlmo.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/goqdvyswz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/giyrifvqh.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gsikuhonx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gcgewtmdb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gwohkomjf.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gtngohdkv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gkomixhuc.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gqsaoghhg.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gwbdwqrsr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gwbwhpblx.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gnxisrpal.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gijqisiro.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gshebctvd.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gfeqybtip.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gbkultnvq.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gzrgirxdc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gaxwkuxoq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gzmeufdnu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gcpikssdw.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gnujwxvnn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gfhpnhjga.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gzfeqfwrj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/glncjytao.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gzruvjzlr.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gvhbqtrjh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gvkhlqjcg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gzpusyocv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gjfyljome.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gwuhzazay.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gjqnhhjul.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gfrrgggyq.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gjtqbkbgo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gkpwgpbac.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gztqcxbvv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gsmafbbkd.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gacwemviz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gioxigpqa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/guooxphjh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gafbcvwjb.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/ghfhmtyzv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gekthnjla.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gilivtxnk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gcfhzurjs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gtjpwzhsu.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gagljalua.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/ghqvrmpfw.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gyyzddjen.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gckyrmnff.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gjxpcwabc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gbylugayk.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/grtlyhyqo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gmxiamjre.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gqkulkhtd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gfcmwuywy.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gjssdvnvw.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gwouiwgtm.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gwpspwzzm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gxjbydobg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gtlvbxwsb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gxdlxnhee.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gmnihfoxt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gokngjurk.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/ghdtxpqlc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ghxzzfdpn.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gufvmafnc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gestxtids.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gxciwttsk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gcfjqaveh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glebuurte.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/grptahwpt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gbwiclbvv.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/ggmmgaiqw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gnpoxifye.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gcegpgjke.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gbvmifsku.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gyevesnco.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gxmfhxxdf.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gyzrmavmw.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/ghidkgazl.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gqqzkdfcq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gmxzpgahz.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gmwbqtzyl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gkhlrjtui.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gttqlyjfe.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gkiqkfnxa.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gnkvoamsb.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gvpxozumg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gtindgvba.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gcuxbqgqm.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/guksrohpw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gmcgohiyp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gxmerjmhm.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/ghvagqlhh.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/glkdfjrjm.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gonhaabcu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gjihnpghg.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gfngqnybm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gnbsicjju.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gkwhuxhdi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gzxlbsqqd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gclwwgxxo.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gkwihkvnv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gtraaxaoy.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gmtfragfj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/geaxcdbyw.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gehvgmtxi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gvbmymmls.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gcytbnjss.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gqekrgppu.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gcspkjmxa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzxebibwf.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gqaadptkp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwcozaqbo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gpwedtplu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpdeeshau.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/ggsulwjkw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjfrhoiri.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gsniyrfta.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gneiznxtj.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gasvkzxny.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gboahkoha.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gtasefaod.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gmmnwotlo.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gjhrfzqzb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gtcjhrbys.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/glaxokmrk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gxrvhjaas.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gurjelojk.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/ggzvhlovf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gzozdutsw.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/ghkuamvlj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/guidwnikr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gchvwvjgr.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gxoneqvim.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaqcptssr.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/ganpyupud.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gctymlroc.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gvnvqxgfs.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gdiojihlj.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gyqagnsgz.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gituxlfjw.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gsgascbtj.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gaeoldass.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gbtdwfqyj.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/grzklziml.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gbtmvjcmc.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/grxisqggs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gtkwioiqq.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gqcpbzosa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gobpdprob.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gsldaugzn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gqqhzgjis.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gwrqarzmo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gyjxjemcq.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gfjbwcyfd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gptgtxxcs.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/guwsohlmw.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gsvdxhzse.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gzfowggnh.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gfdbgljlb.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gbzjzwwzk.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gvwbamffc.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gpqdaqbtb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/glsflbqib.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gewkdhqcn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gmzghztxu.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/geoxbxaor.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/groporhhy.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gxbbtpzxj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/genwxixgl.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gmubazifx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gjvnpdbmt.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/grnimptpg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gpogdawpa.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gwmbgvtih.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gajjeosvw.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/ggddbvqrj.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/grhrudtns.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/geqjdwwox.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gnlsktptt.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gqjrpzklm.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/geyevqlya.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gizuwehfs.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gmkflrwhd.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gpjpeegkh.sHtML


<!-- 参考信息 -->