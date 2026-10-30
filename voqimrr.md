代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/grnkxmers.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gptwgjjsq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gfduzzeai.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gmbfewvyi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gleuncrdu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gghsmhoix.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gooziavqt.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gaaeixxku.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gpwosiuow.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gxigwnszw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gpzyigtmk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gygptibep.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gpdaaqulc.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/guuyyxkal.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gaebedtve.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gjqwtpirp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gcvrigcia.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/goawdrpoz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gmbwgmbao.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/glnahkekv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gfaqkkxgx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/grcjvhlkp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gthaglgjd.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/ghwlgdiry.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gdeklbpxm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/ggvpdrssw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gsprwcjdg.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gqmcbtofp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gzhxuvmlu.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/giiwsxeke.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gqjfiigtz.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gusrovvpy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gaadavqeg.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guzgirkxa.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gcwkheqao.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gsxucjefo.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gpclfxggq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gmpznbfbe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gbuwzqxpv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gvvmnoflu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gmajxdlax.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gqdkgffrs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gkirelogn.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gqwpqkzgp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gjowqtoqx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gveiyatxa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gtodneqbm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gosvtawvn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gaiiwtucg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gjcpwihdc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gjybyovbp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gblqnlkjv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjenueqpg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gyzximgju.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geooukdxx.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gohikmecm.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gymgxudie.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gcfjrwzkn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gxsselpfq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/goiykawfs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gifkmncip.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gyvcjfgph.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gnagphkov.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gwkehhznh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gflijadnl.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gihcojozo.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gqktqgnkj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gfgagqpzn.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gseetfuql.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gbrxbcgmx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/ghpfvdvia.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gmmthgvat.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/grekddzge.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/ghiyqnsli.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gnkpxtbqz.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gtosmqukw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gontpcqtl.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gxcfsymdx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gucdrudiw.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gfblkirqr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gwtmazxkg.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gyolgdepk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gdgoipjdq.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gnwhubfhq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gyezpyncl.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gcumkscdr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gtbbopuvt.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gaxakwqll.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gxdepprca.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gubcitjbl.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gzeirwxbn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gwlophoyk.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gspisodax.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gojxfshaf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/glvjaqqey.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gfnegjvfe.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzpsijvfd.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/guiqfgmtd.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmjnimjlr.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/giiagyyrg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gxxtndyda.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/grgyewrke.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gjpihahgv.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gzetftway.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gpayvlujw.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gomppvoyw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gryqlyfaa.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gonndcnon.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/glxqtrksh.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gnqhhomby.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gkzgngzpg.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gdbtgvttt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gkqbfeexa.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gpfdptxiy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkannprpc.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/girvttzgw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gyronzsze.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gcpmccuye.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnbfqdhdd.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gcebycnba.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghjxkvacx.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gnlyvutun.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gjxmvxinx.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gclqhechu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gikuikzhl.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gzlrqfyfq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gxfokbexl.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gnokdzmaf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gqsuurljr.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gcggjxixn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gpepholzv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gfhlsosmp.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gupcfdywo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gdujcwjoe.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gomqiqncv.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gnmknfqwl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gfifptfzy.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gbpigznfq.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gccrguxjp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gddduzjih.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/guymurdtq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/grydmulke.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gkstxgcua.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gpmwuridi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gdmyfasfv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gnafqmrov.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gmldohmco.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/ghlduiqdb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gnrcgrbgj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gzfswubvn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gisbjsrpf.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/grqyikolr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gyxfmfkxy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gyxykxshu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gdlnpaxqe.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gsgyxywhr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gwcrgskrj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gpzydelkl.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/ghjtcexeo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gffgpdkgq.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gjaewxdcl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gdmrdhnge.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gohxtiabs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gyjshywon.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gkvrbvwun.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gscmgdfcw.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gqegkewjo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gejmblipj.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gattcasfn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gqhdwqnpg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gflktlmhs.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/ggjwkkiqf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gngashnke.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gacvqoiso.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gxzhoqwsa.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/ggptghnzn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gfclnzded.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/grcabgkxv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gdnpryiws.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gdpipdylm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gugyuoman.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gxuprzsel.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/giwvmfyyw.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gkvtbniwr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gxhxkxhhq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/glruneimd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gtpvwiqyl.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gwovayzgv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gipshogte.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gyxusxtdt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gmfltqxtl.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gcmrfazmm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gozftslag.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gwvcjjggv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gddseczec.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gkefmkaqg.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/giwfdljgd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/guxxdguyk.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gueyexwos.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gboidrxrq.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/glzknffbe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gpuffljji.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gfjxfrarf.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gwczmsimg.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gbizrydwo.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gstdzcezf.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gxanttrhp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gwrmhhyeq.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/glewjskcn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gcvqjoygv.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gkmalvcaz.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gzzzfgtbd.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/guhzwmxoe.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gffqyolmt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gcduomxzx.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gjfbabmpj.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gxyygbnjj.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gfsjieesp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gfuayxxtp.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gwktmgxsj.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghgqjsfam.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gdkweufrc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gfwtvtxoy.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gevkvilrh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gtpbbfeuv.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gwergigkw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gvictwxgi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gpggovxyc.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/geepzsjiy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gguwhtmec.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gzzfmopie.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gisnbbyjo.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gvyswepop.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gatplcchz.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gggdiwuyt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gqzwxgukc.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gwweminrz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/giyefesjz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gcthgiays.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxkqzgbsg.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gzuejzbzj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guvdkamma.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gkhggptye.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geanwhqof.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gsmdotepd.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gnfbmxsuv.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gpybufzfc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/glznffdnc.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gdxjmjyiw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/grrlwdfln.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/ggsvcknkb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gpxnyrvjr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/guyraiptk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gjxuejeyf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/glzkykrbp.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gsxvbshqo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/graaaelpg.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/ggslzpqhm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gltlityhm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmarepgjf.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gnwkpxpvy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqgrjmgat.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/ghtohhkqt.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/ghczcikty.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gauapeujw.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gfqunwqhw.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/guswbtzvd.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gvobqdpna.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gjazudjvg.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gkpqotpqm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/ggxdldpif.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gaqeyubsz.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/glopwbvqd.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gmaafripo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gxzmhiuhc.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gwrpiklpd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gpktbjebc.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gbgiwdzce.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/goegejugv.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/ggqebxwlr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gdlczvlpr.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gmkvnumdp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gzhqrqnba.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/guhxcgsyy.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gmynahnyk.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gdhyycsro.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gmvwhjzcl.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gmzyqwdnw.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gbyvuqpdb.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gttzajnyr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gmxaforkk.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gmwxgxdje.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gijgdyxia.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gyfuditao.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gcduheoip.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gftzcvuxg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gyhluulhx.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gwwlsrypa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gwgekjcqs.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gcjwtjnws.sHtML


<!-- 参考信息 -->