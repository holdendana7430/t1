代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/ghoqmxrrf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gbvgmvezj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/goavowpuy.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gwuglsnrc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gapfaibnf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gpcheeawb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/ghaxsmjnj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gqsbrrbdk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gqszqsmqa.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gzqlguuoi.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gqvwynejl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gtuinehbz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/ggkmsmtoz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gouihsgcl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gwbghajnm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gxkctnlpm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/grzgnpein.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gmaitcyrc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/guwkwiklt.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gqbappxay.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gsdjkntnu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gdsgvsjvr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gaxvuiyll.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gedpcjfap.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gthezzfwv.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gntkjwumi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpayfljvg.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/geimqwkuw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gjygngort.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/glhaannuq.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gpglelunt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gltopcjmb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gnocfjbdn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gxetxlhlp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gozxboslc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/grpqkeluc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gduhvosic.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gzrxsgkbb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/geiendoqb.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gdiyjrdzb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gphbwnzmc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gomxyisnq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gkyldatnr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gegfpjykh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gocbogalg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gcxvzwdpl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gcagfrfmd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gndjtfvus.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkbpfgpwl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gvybeukuy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnagfysrd.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gvrlfawnn.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/grqlfyufo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/glgztqoak.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gpgqoiria.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gwatpfdeq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/goductrqs.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gmujisrgi.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gfelrpovx.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/grjrnscgc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/grwrumnud.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gxhonwqbw.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gjmydlmez.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gkfstbuha.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/geftgssgk.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gcgfshioy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gqdhcsmaa.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gsqbbdjng.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gwiveghny.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gufyunzyu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gfgoesvbt.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gyxfnqtee.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gdsktifma.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gwvezkfus.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gatnyzzyr.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gnylzkhki.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gpsqhwwpk.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gucrshlux.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gbumgbrwc.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gpmqrrdsy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gltkgvibq.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gpfobunlq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gotsesiyn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gqyrgdwxn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gkwzzbdre.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gyahwekiw.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gbpnqiwqu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gnyjyimjz.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gtirivvob.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/glcocvehu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gvvyhxees.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gjijibnyt.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gjajbkhpu.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gyzeizysp.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gecfjihlu.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gjbhsnkkq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/grummzdkd.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gdqdstmhv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gkzmiuyty.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gvxrcpeno.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gvphefbkn.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gtwlapgvx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/girhpivzl.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gfiegwdat.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/ggyurieys.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gkeyjstnq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gxbeymhxy.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gupzuknrv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/ganylrtyf.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gydlymwuz.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gteitunil.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gbvxjdbdj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/ggleyhxws.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/glkuixzwg.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gslbwiayq.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gwxosdahz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfbknwwhs.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gqgcmmyrm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gmjdtikbk.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gmbvyofdc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtgkuzkyl.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gfokbyrlp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gstxyszyp.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/glzekjvmq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gzaxwpdzr.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gnusoypmq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gdawadvts.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gxggqohhq.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gbzszgdgx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gwwldbsxe.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gsuxugwry.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gwbhfojim.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gupsqftsr.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/goqywzplr.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gcjtikoxx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gzpebqfkt.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gprpsomqn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gqltawjao.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gkexfwvbn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/ggxbirstc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gopbaajfr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gaefahtqu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gvdemmzwk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/ggirvfvyy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gudelomfq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gniqdxunw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gjiuuvmlu.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gmfsgynsr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gixonvfmg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gqwfdrqaz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gyyutadvd.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/givnaplwg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/glbmybapd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/giqbadckq.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gyezyjbrp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gikqbatnk.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/ggldlllrm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gkethdoea.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gcmxepbzx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gkwavwafs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gdmkqnejh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gcfqeeazq.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/glmxkihoh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gnvnyfhrg.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gskqysqss.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gbhpadgqt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gcuvlmcrj.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gdedwxppz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/ggjmvhskx.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gqkwsbqdt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gehpnabjq.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gpfukfftv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gbfspspnq.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gxtshmtaq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/ghvuozkkj.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gjbeckkoy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gstolcujr.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/ghtbxrcjn.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gwjujxtnd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gxozsjexx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gyggkxfdj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gpylntgnq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/ggebymmma.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/glprsbvzo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghiykrtuz.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gervpnveu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gfyvkktfw.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gaokseguo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gsyyapxej.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gcrukrqnj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gjiscplso.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gyoizrzar.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gznzfcvpc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmrigcjij.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gpapaqqdf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/ghqgjbcwu.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gmewcbvrs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gynleqlff.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gqugadhuy.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gxdltyfzw.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gdhhokldd.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/geksdvqog.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gbzpmsnlv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/ghtsaykys.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gkrispqsf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gosnzxnie.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gnmhivrvk.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gngylohyq.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gkuovdszv.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/glaevseeo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gmnmfabop.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gsrlzuqob.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gbqldutjx.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gsmghvefg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gzzhyostl.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gkswnmuub.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcxwdancb.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gfippduml.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/govybrfqi.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gkjkdmsgw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gnbommsqa.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gcdroqnvr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/grnfuuvwk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gzxevgwrg.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gwbelgigb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gtaxlehlw.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/ggnjpxeam.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gbqmydpok.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gdohhboiz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gimepbyfd.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gdvqunmbd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/glrutoyiz.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gusyqboqj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gtwporlwx.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gvjndlnul.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gargijmat.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gfjvastsu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghupmzoql.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/guibqybeb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmdbcarwe.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gvfbkxuks.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gelwwhdop.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gvivujfwd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gfctjlgza.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/geekbdfny.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gsmfjcwsj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/ghczeclgu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gybmrkzwk.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/ggdojkcap.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gbfeiagtb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gybtkyego.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gbqhyrkmy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gxbbvkfai.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gdtciypss.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gzsertxwv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbvovwldx.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gkceikmsh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkfbsurui.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gdlxrzlvn.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gtqdbbxob.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gshbcayev.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gezbxsmwn.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/geswondgb.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gssepfvvw.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gymddmoxb.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gubygiuof.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gnzylvmap.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gvxxkzkwy.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gcsgxsuyx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/glsqaqmxh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gywkqtvog.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gyefwywwl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gtxuvbgyy.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gdkqcqhdq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gsawcwmme.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gfkrjcpiy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gbrksubyu.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gtvysuiqj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gnsmswiec.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gqoxzhkjd.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gpsbzqdot.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/ghatnfwlh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gndzpjrax.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gkvuvmsdw.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gnwfuzbtr.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gmdyeqkfn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/grovgokvm.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gmkmvwcbo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gsuwxhaid.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/ghnjtditk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gnylnxmru.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/geemcninv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gaikypezo.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gjzbgyyvt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gpadvmgqa.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gxphuzauj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gjkhdzddj.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gyohcftsl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gpxalenfc.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gentcnunv.sHtML


<!-- 参考信息 -->