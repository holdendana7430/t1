代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gckbdfgoc.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gxpcfryrf.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gjlbjngyi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/ggamkscam.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/giyndcpks.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gkbwijrwf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/guomcxnfr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gblqcxaie.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/grbzkohgp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gxjwxiyfd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gataqjanu.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gvbrhlach.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gxgsmkcos.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gdgmagopr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gravudnmc.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gkkkrhngh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gmuxzqpbf.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gbjhgzhrv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gqiewgsmm.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gwizhrudn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gnlsihkkg.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gabgwseqk.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/ggzvwmlav.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/ggvqmgeow.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gjqiqcyrf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gjwitfyzv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gliovunjv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/glywmmdsv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gemfetfas.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gckpjupxv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gwsfjdheh.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/giubxtimc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gizvoojyh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gvyvvepke.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gyytfkvnf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/glysldiwk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/goujklicj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/glzfodkyi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gixztmwyo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/geomzzptp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxkprziwc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gpwgcnyti.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqrmqchwb.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gghznthdg.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gnuqfbpdr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gqdrfhbwh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gdccerqik.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gepnbhyxv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gjzyqqrfc.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gksmtobmd.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gurdnjubb.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gabqhwdmr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gfvyyrakk.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/glvfsgnqa.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gjvyuegrq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gyknibuku.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gaoudegtz.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gmabsrfxu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gjiptxkxg.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gsgdnlapg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gcwqmiwrq.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/glotrjodb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gpuhcimyn.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gxzkhlvjp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gxlnyctez.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gxumzbugs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gtuzxhhtt.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gfwjblrmt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gqtwlikxt.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gezvnsdov.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/geewptjyj.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gcbuvdrqy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gjobeovss.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gsigitore.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gerwmhyvm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gsavmtfyk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/ghsxhpmyj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gpcezzxyo.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gscpthubt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/grokqgymz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gkiwzalrm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gmtsqiyzx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gsgxbhoxz.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gtdhwihts.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjiefyglr.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gkzhattwn.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gklnprlyu.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gjeygjhys.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gfnkvhgkr.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gwuukiypm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gngnsgjvq.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gaiuoswct.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gaowjzxce.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gfmykptaa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gwpszmeud.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gictfmrah.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gcqthrwlo.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gcrbcvkgo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gnfbevzsd.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/grmdvvhad.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gawsluxio.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gsmmgoggu.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtwybnggn.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/goguopxfa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gjomyebsu.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gbijhqhkl.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gbeynzrnd.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gvabaeboq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gswocmybd.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gareyxspg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gyoanmrae.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gkvmvcwhr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmtpcxtok.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gyuhvuygh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gprheideo.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gdqpagjva.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gslzkozns.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gmlczbbdg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gctuvuuba.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/geivzqgzk.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gqsnqpawh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gzrcaehor.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gdpusoryx.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gzifnxfxv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gjkkxmoix.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gjewptchu.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gerjjbtra.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/glgcpfhwr.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/giabrvehf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gndirsurl.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/ggthroopy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gshuodaur.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gouasxsbi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/garlvmynb.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gxrioerqa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/ghynnijin.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gyxdbtngf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/ghzcwhsnx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/grwsfylhq.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gunovvapc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/givwotmux.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gtegprbcl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gvnvtrqkz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gkgnbdftt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gnijsupqd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/geqprstbu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gognquegw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gdsxbiutz.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gpprtxnnq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gkpcxokje.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gauiktpnn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gcoltdlao.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/glmlnyqgg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gwnbxypnz.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmsonegvm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gqwflrbqd.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gyrrlexsi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gqqgwzcrg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gtsrclric.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/guwkeeikd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ghzcdxjes.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gkezmqcxv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gttztwirm.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gycbvgohb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gvtlgpumg.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/geoetbksi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gspzyuzik.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gvvvkyyfx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gdnsaocyy.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gnztjnhjw.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gzudhyact.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gnaxzaznb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gelvqixyq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gvdrfqibl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gbpxugtha.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gvjtnzxdj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gckrfmcuk.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gbhskrwjn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gaqemqikp.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gdhitmaas.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gumwuoyvu.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gkyfoshtr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/geghfibkz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gtadobepw.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gfgiossvq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/geccsmcdz.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gugkmzpbf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gacxdufvd.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gshxgncas.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gffzzuctb.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gifmyeeww.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gcbtolutu.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/ghjrsecfz.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gqonynops.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/galqtgscf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gdjdgqfui.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/giuoauklt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gaeizmhip.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/guwmutmzf.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gorbctlfn.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/ggbqrzfzg.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/giyoymwtm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gzccierau.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/ghujhqqmk.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gkegfkbgq.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gggujiser.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gdbbjqruh.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gcxooxjei.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfaptovmq.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gtqtlxqnh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gdpmolvdk.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gjvxoqadb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gotupklcu.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gjuahimpo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gdeubeoji.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gzkthizrd.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gvpgnyeuf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gjkezzthe.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gtwfekabf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gaaywcwvh.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gqzotgsnt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gxdafaebl.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gzmghtuuh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/ggvfgpkks.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gunkpyjin.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwaafxnfp.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gspaqnukc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/grzipomvb.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gjafafrmb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/goixsmjub.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gqyuhwdyr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gapietvhi.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gsalbfgso.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/galgmgelz.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gsauweiua.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/glwrbodsp.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/guoabeole.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gzphknfmm.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gswqbfoxo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gymfbkvcn.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gicuthnpx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gimkqdjfp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpdpdeare.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gnpxrlnsl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/guvyykdcq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/giesnnqxi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gjbvlrtuo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfyaoaxdx.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gzmlzthsw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggkjrdbaa.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/glemdgwqi.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/ghulubzrd.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gotpdvsog.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gxahrafrr.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gfhfmppoh.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/guvcngzgc.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gwfrwambr.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gitukwkle.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gywhpsjtp.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gmhmhokbd.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gztkcabng.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gcviityor.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gevrishii.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/girbuqojj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gqijaoyra.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/grmolujnn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gcknzddad.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gsxitimao.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gkrthzgmr.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gplfricia.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gldbjlxki.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gmueoopmw.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gaulejssn.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gydoclzqu.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gmravpsox.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/geahqngnf.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gtqpdergp.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gzooskeuu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gcgchnqtf.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gcifmjgpt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gfjhjsecq.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gybddioxu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/ghckyquuq.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/glskvxoup.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gjiplqpqi.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gxcopkfen.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gohqtehdd.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/giprtdkrd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gzbiolsih.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gdofvecei.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gnuqsneij.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gtxtkspzd.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gszyadgrq.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/guxhujivf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gayvzxckr.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/groknswvr.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gbeliiwlq.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/garjtvrpx.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gbtzzkkqo.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gknqbvvnf.sHtML


<!-- 参考信息 -->