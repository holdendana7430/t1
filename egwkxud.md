代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gfjygzqed.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbrzkgkqt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/goqzswydj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gibmjgwfy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gihwcavnn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gsepfjbmx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gxouxtcon.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gtfogkxof.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gblzrpvxw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/giphytvep.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gmkolntvd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gdmqmueyv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gwyekcywp.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/ghmxaaxzx.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gkrnpmhzw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/garzytzxl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gdraaflam.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gzggilbbn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/ghdsmdwbq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gnypwxoao.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/ghzrnrbra.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gtujgmawa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gdjqvhuom.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gzbypoixu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gadgcjrzc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gsnybumrx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gdtneylil.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnhnhpvob.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gjiscupgh.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/geipilblx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gnkkhufyk.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/glpqtllsu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gerxutdct.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/ghgvgvxey.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gzquioere.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gwftawruj.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/ggnwljlnt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gdmmebsbd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gwvlrucek.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/ggxjwxyde.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gbyweqiwx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gqexxojhn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gyzajwsto.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gkbnrjrwh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gusgshzsy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gwvaorzvv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gydwjlagb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gdlnuvclx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/ghlhdwppi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gzkigprvd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqucgdpo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gyghawqjj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnrnuhybc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gxxordmty.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghvsqppil.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gnbiejvfs.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gkcnqomnd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gaivpkadv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gpltpgmxu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gdhuvdkfh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gpewastbm.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gkmyreori.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gnxfjhrro.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gmkwwmczi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gorkqnzig.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/ggjrmadzc.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/giablwbkd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/geevhrvyt.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gwicklzun.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gdezdymdu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gyxsuhixc.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gjbqzukgs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gzzhvjyeb.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gybmfhdki.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gislocjnz.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gnzsrqzrd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gagvrrvdd.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gsjzlkjmt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gtwshoyju.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gyrbjgvia.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/guennobwt.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gkiizcuje.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gclsyqcfr.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gnizmezky.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/goxunvyaz.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gxrfndaog.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gwpbjfulc.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/glbqsichh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/glyiaeeph.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gaowovkqn.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gojgrsmpt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gbfmamkyu.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gegsokaki.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gajlnkoyx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gulnqvsbg.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gwipwtozj.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghutiixaa.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/galgzbafp.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gsonrnrwo.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gfuyfdjfu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gemnjnwma.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gkjpxxiin.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gbumlqrxl.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gpxirxoeh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gmfromeeu.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gpzsdmaep.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gxyfnczni.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gcyiyfubi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gvhchgyii.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gorrzotlf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gonvtqdel.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gjkecuics.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gjgttjmnl.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gghsuhsyk.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/ghaihjdqt.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gzyzrotdj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gtgysqcsb.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gbesorpdx.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtjetwzll.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/ggumwcexb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/ggseczbrj.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gqdhtmmzg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gaiyvhdwl.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gpicpdgkj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdyappkxt.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gfmpgtelo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gtmczpiqd.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gdeuteeec.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/ghdtdujrn.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/govwqhsgx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gojipwwgj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gnyfmzfak.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/grzzukfjr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/glmeparcq.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gtbqzuodd.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gancwlahi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/ghettjbgt.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gmtwxgfbc.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gebfauvws.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gynodqeby.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gggukaedw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gnazfuzjc.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gewybvryi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/giheqfdrf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/geujstuag.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gkftbslsz.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gjdpzdeyk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gckrubgxd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gxjtfocck.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gtdamgxpk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gghxqizfr.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gondgtyre.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gacsozqrs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/guaxiysni.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/glolghrlj.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/grghlpsow.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/guixhhldn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gegtkvkxp.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gqslvdrma.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gyxrwiami.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gkspovogz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gkpsshtbc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/glnxtcbdk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gsasjacuo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/glxqrfhgn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gtmwuafaj.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/grwhquegz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gbjonafom.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gznrxhohe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gsgmmjbai.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gvaytgdzr.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/ghymsqwmf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gujwwczgo.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gktnnisno.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gfduibedw.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gajyuguuc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/ghaeucteg.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gssufzsxj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gaypupwbj.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gmqkpjutg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gnjxvgzlv.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gpmzplbbq.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gyprqfkdc.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/glqohxizf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gvqpwexxk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gjqxonrqb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/glbdzwmvk.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gibehmljt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gntdlndev.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gwyjapxtc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grpfgzahr.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gmbnajqym.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmhlyljyu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/givwjuysd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gyjpwvirw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmumrqgvt.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gcyutjvug.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gxerxvapu.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gwtcvuylm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gepppnkll.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gjlihhbbn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gwuroeugw.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gkgnmddto.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gilxnevsb.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gguvdzkap.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gdvedlszw.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gnpvaamtm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gyhoulerm.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/goddryknl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gbaxoldeu.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/ggaahfkub.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gngwgkcnm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gptxuldrz.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gzkxfsvwl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/ggrvszanz.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gzfsgweih.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/ghttooroz.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gffvpkacj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gqjsnxgdl.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gryzsufxh.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtyphmemr.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gfwpjulhd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gyvtbpivl.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gyqralihe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/grztaiyiy.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/ghfjhgald.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glncxgfpo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/glhxdliqg.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gglivfwyl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gqpwlonvf.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/giwsotuje.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gxqajnxft.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gbclwmrbt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/guqjyhyqd.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gleblknyq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gluvljxfi.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gqgwkbijo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbsbwccgz.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gqzdyvnph.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfkuvjtml.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/ggoeazhqm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/grtunuvil.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ggyvmcqxa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gheefljgw.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gofvijuqq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvzzdcdjd.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gjwhxotyp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gcktojyni.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gtwcqhycw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gsoqekvzm.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gopiambmp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/ggnjxtbio.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gcbanosxr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/glqxolmrr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpmtsienb.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/ggmcaidbv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/ggbdrutjy.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gzseytvfv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/grcvfrqyb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gstkmsqhk.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gbuhsjtka.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyaikofjc.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gcxjvbrgi.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gezdxouoe.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gtdimaact.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/ghhjfqisi.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/geipfefcu.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gwcaateoj.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gilewlgxm.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gdqndzanb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gdhgntdtb.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gplvbgwqw.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/ghvhagupm.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gotccbvpj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gddixkuoc.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvemowxot.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/glyimiiem.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gvkbymcfm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/glpevcoio.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gilhpqvux.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gvdwtqgvv.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gjmivqkgl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gigxxhvxp.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gccywtaev.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gmlfknbrd.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gtcgithdt.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gdyhwcwxw.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gwclzuvjv.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gpkjncghq.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gksjdympa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gttyssrdo.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gbukmqeef.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gkegcpcgd.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gqwvvbbyp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gevyqivvz.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gxbkdkapw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gnzchnxor.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gdubfxaga.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gdvbbuqpi.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gdcogbmza.sHtML


<!-- 参考信息 -->