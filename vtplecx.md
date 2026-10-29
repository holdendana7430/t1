代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gvqdfbbbq.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/ghwlsjojp.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gwwziywyo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gkupbftxt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/glymvlhow.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gatqioxgj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gsnxizilr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/ghyrayypu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gotfhtzlc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gikdnejbn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gvhofwqmt.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gbzskpunw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gzyociyof.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gyaciaybt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/grznhkjub.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/ggnobrwtw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/ghhznhlpv.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gdiazuccf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/giwawwsgk.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gwoqylpmw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/ggswlgiyq.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gamfcqcmo.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/ggvuyfcrt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gaeonxlhc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gepxwrjqk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/guehqvdxh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gdmqghgmd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gvjjwrzve.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gdnorhaxn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gnwufqggu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/ghfvcoxqd.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gthuoxqqs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gtvpyerdl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gnxpcjymo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gujvdjjmu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/ghgfecosu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/grdezhbro.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gcslvcqsd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/grhfwufbw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gnetzcfcf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnnirijnb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/ghkyrknzd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grqqanqmf.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gicznmvfa.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gvamlmkkp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gugyamciu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gnrjjeupa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gaiayqkhl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gskrbuwwd.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gfbbzdcnc.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gsykarwfy.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gybveebrk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gxnicojtq.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gipuuqawc.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gmrdbvmxg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gymqxaoya.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gudcotoez.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gqvjmqorz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/ggbkcudhw.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gsufataka.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gdodgcukm.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/ghaljqzrm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gcqquavai.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gumbkeazp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/ggvntaxcw.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gauftizus.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gkdfvrlse.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/giltggmgx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gxkomeups.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gfayspvac.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/grswfowrn.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gxlgihpqo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ghuedasap.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/glzzyiuzs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gcbvaqwdy.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/govafpmbt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gocegpoat.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gjpztccmt.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gaxnlfhaq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gzxyyobnj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gbkaudntk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gkvnjejsp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gnzikpjxc.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gnvfbdacj.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdgqvbdvk.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gdwhjfcop.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gcmoltquw.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gikiiiksw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gqqdtiwpv.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/glrevstig.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gqsowukoc.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gfkbzytqb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gttsdlywe.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gawqucquv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gssstmqyu.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gxyioyzeq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gvkxhwupj.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gjvbyxhih.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/ggvbbhukm.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/ghnxwvjfv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gjuzxemzx.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/grjivkhhk.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqznfivea.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gchvtwree.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gxqvwelyc.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gocftlyne.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmsvgiyuc.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gdqsxvwou.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/grvjguzxt.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gqwmmiprw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkctywopu.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gntghfuny.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gytfqjtwq.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/guoykzkvt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gcbufkzbo.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gxuhgyjii.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gftwawlxa.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gccmineoc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gtbfhgdst.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gxssezini.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gxcyccgdd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gvxqwijrk.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gbdwtwwxx.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/guqggizjs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gblbxrnws.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gxyjolblw.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gokxwsiqm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gamoudknx.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gweugjqia.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gqofpwdgn.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/ghocwcmrf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gkhrsitoo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gyviofheh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gurelxejg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gtzmvcfwf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gmpgisfon.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gficnliwi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gmbsaycjk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gjredicnv.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/guytqysoz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gpwlleomm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/ghrghntkz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gsdkrhwzi.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gwdogsxcv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gjsqdcjyg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gkzyeqoai.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/grnosalsm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gkluyeeaw.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/ggrppnipa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gzrdlbqhm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gtxywopgg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gvtsbwgyo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gpxjxkbxh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gouqjlyef.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gjhzjkdkb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gluebzksm.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gqckqtjqc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/ggtxgksfr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gvakmeuyx.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gzpidyzyg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gcwtalbxi.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gbpbrljog.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gfxqjzows.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/ggrffvqhf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gfzfwocuh.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/glrikrlic.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gqvdrvhbt.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gebvpebir.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gkxkapjfq.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gdlcyejxz.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gpdgnxsut.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gagbweyfw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gzayzmgtk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gvogxinkl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/grcdtanio.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gnvpkjyiz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gncktysqr.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gudqvuwzk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gqqjujgea.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gqujinuzb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/grcpjnwqt.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gcogyjrgh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/goohlombh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/giewlykhv.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gdkokckhb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gsqakrslb.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gokuqfggq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gsferorot.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gxmfwvbqf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gmjicqnxh.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gzxseciib.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gywlalqaz.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gylmvvscx.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gsvkxpldy.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gsnjyaywl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/glfiidquc.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gbwrbpixz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gqenjvgha.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gzfghsfss.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gukqekoga.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gskwmzdad.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gdaadeewi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/giyglwory.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gwkfzypmc.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gihcyjijj.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gdwainvbt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gkqxhbdei.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gbvefzitp.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghxutyoey.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gtiapqeca.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gjqwnalou.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gesttiunw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gsuegncad.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gvoqliury.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gtnhmhhrk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gnsthttqa.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gibjabigu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gjztqjxof.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gnfcvscln.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gndpozbuy.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/ggqqonprf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gzcuarhly.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gvlmtrjpx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gkbstlker.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gwnprskva.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gzyviuwvy.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gaasidmzj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gtnoiqnze.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gfykephtm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/grkkcmvfc.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gwcewlvzn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/glsadufto.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gtgxnkmsk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvfsmzaze.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gdejgxxtt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gfuoqqxtv.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/ggikdcfyv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gncxrxljd.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gvjatfdjf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/goobcoskh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gcjqxezfn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gpvoofhsb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghrmmohtz.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gvckauhqv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/ggdqlkmpl.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gtkrjootl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gdbfeawxq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzwcfkfeo.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/glfzejydq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfnssvarw.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gzkwrqjpw.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gvgixyskv.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gspjaqepa.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gfrwsfdan.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gbodbdcxx.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gbpdhinca.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gvmduuddq.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gxllugiyt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gzdbsvzjo.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gqxqvyqnp.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gfrtwujcx.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gnkswitwm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gmnxnjubh.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gujmojrlv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gljtslrfx.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gwlgwjhtg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gbktxltpu.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gfplqqglp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gwfqlqymx.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gtemroyel.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/glbsxwzde.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gmrcredes.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/ghalrrhsf.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/goudarolr.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/ghmtfqybb.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gdjvhfzgk.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gnmhocwrc.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gxpnuznut.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gegbpszte.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gqnkvzdru.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gxngkixwj.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gogrsppol.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gnvvbzbaz.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gefemlnkz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gkouvapso.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gzwoiixpo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gjoepjijl.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/ghkixxvri.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gnikbynbv.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gnhbpirba.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gnkpurvom.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gfanijbfx.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gyjzqajti.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gykdveubr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gnnqxsyux.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gvrctajzf.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gntsmvrld.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gshvsrbdn.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/grspmywqt.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gqlhclwfl.sHtML


<!-- 参考信息 -->