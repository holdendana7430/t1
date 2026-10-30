代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gbeecspqv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gtnbflnjg.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/glgognrbe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/geavzlxvx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gulccuzxi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/glvztipiv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gvglspsgd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gcknqulxg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gmjetkpgf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gfjrhawxr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gamhzmyrk.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gtzkcyptp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gfbndtzat.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/guhhhgdva.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/grgebxpug.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/giphjinkc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/ggjfdbjdy.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gcewtnbwo.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gvxnwkmqd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gcodifhic.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/ghgutbdsb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/ghnsfjkxn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gfgefogzy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/galdbndeu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gketeedup.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gngrczlls.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gxjapokel.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gqqfhikxu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gukvwjcpo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/guonpyhxl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gvxpvnjti.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gkvhyfvpt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/grngucnys.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcpdrsdkr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gxnxrzkwx.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gacwbhtda.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gwajijjmd.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gyqkghabk.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gaeocjtkg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gubvdwjzp.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gjtoaolab.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gppljlbgg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gewkwoivt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkqabcsgg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/ghssvxaei.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gxwwenory.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/ghpqvtgxv.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gfqqnceul.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/getsqngmm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gibtxhibj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gcwjitaww.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gnrpdxrdt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gzzrduszm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gpgnbgahm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/ggszpbjjy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gralubmde.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gywymtqdt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/ghvfhifjk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grsndbmiq.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gevjixvxa.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gexstxddr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gpkzdiwto.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gtnncfyhe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gknevncdi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gkacxqsdq.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gyweutxnw.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/girsdpcaz.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gjqqligkc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gejthnynq.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gnwvllqqi.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/guhqucxgu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gxaqtsxvg.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gceotleju.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/guvzonopc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gghndcmdx.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gefzfuvnm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/ggxvtxkih.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/grupsmryu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gaeybshot.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/ggkywgsxz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gegopptfz.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gercztuhz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gpvpwghjv.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/ghenzcflq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gqxztmeek.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gxlcycrpd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gpjrbccrl.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/ghwocdfji.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gsiigvvnu.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/ghlnhpzhy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gymjuwpgt.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/giyporsiu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/glvljvpkh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gzjcnqzlx.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gjfyeoozk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/grkrgxrhw.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gvnidzura.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/goxljuira.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gjjjxjxtt.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/ghewbrrap.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbnqolqyy.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gdhctniop.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gctnbuhsc.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gjeyrhrlo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gxkaqxqhn.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/glgxtzsdk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/ggxlehxxm.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gkxoswudb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gnocyjbkh.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gtrmpetfr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gumavxuxi.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/ggxtyvjsg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gxzzrvgyv.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gwzwkutxp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gsufjzqhw.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gjdgkrden.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/glerytpxg.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/grwrodtwm.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gomfmikqa.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gizleenfu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gvgnilvvu.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gaiqqsmop.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmoqnkiea.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gwjffjylp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwshlrkwt.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gimmoocyw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gjojtcvcu.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gbkxkkkmf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkdnutqmw.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gpjhtkdjg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gqhgfmivf.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gfohwbgvn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gopmouyra.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/grhobqxxe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/glaeguagu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/guktlhhge.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gpovhxtmr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/guxrwygtv.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gihiviykq.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gmymvhvdb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gthdsvrax.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gegbyomxa.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gtlsmsyab.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/ggagpjqct.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gaqkqfiqi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gthhsfefq.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/glnohqjeg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gfvofsbrj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gqhgwbrjp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gkcwvrgvk.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/geocjngek.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gbnxfsewz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/glkbajosh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gklvrydvj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gauktebed.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gfhkyhvds.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gsnemmpgq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gbpwnsyla.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gtvnbelvu.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gpthofqmm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/glxphcvqs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/geqrhhahb.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gubtladuw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gmoiklren.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gmqvuyahg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gtmasvlnr.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gfgsrcgxz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/ganyiaetz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/ggeneydbm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/grqmywcyz.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gmhtbepqj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gdbzogkxt.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/grmlldlws.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gpfqpoacb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gjsakutwp.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gsnxygvjh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gqissthkp.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gtbchmhga.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gzsnrsqhv.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gzmzizecz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/grlgsxnup.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gmfwjzeyj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gfefkupkf.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gxnhjmihi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/glpjraobp.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gtberelgj.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gnezlcvhk.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gxfroybtv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gzmwcldul.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gykkpggjd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gghpaolcb.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gcnqqtcrd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gddazskpw.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gphypzkul.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gggfsmfxm.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/grueqtwod.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gzyovywgq.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gvdmxeiyj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gxrnlbsde.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gdvhtklei.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gpraqtspw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gtuishoul.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gmjxgjgze.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gmvzzycfe.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gzifjbxlm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gnrxcybaa.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gkbsmxrlh.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gaqbbuhyp.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gtunomjzz.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gyrkmasvb.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gkqqqhtiw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/grmhmgxaz.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gmnspbowh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gygkivvfk.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gaelzcnkh.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/grkwbxnnw.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gizwlhoax.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gjubvwikn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/grbpydagz.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gpjgjadcl.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gbppqdcys.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gtlwxgxya.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gudjcrkgm.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gxitaknwv.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gcpfvrgjl.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/glxfocnou.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gjziydxmr.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gvjrbjwtq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/glmacylxz.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gtdmwjpfl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdeukkvqf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gygzeyxnf.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gtyftssjc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gobbjokdb.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gjbjxfehh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gkbwikinl.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gyigeixzi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gzxjrycqp.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gvnzpteef.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gftdrpbln.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gjonulxvu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gixdquaqr.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gfnnywysc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gjklfekrr.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gqxhdxfsb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gterbfdzm.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gchholyne.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gntprssmg.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gunckwgvo.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggqjyktza.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gbveszaqq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gbrwehohg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gkyydmuyo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gvwpelndj.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gsqqnbvwv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gaspesoxo.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gafytsgdz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gvgysmpww.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gcwbvvkjt.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/girrbarfn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gsfyeariz.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gzslrarox.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gwzybbmty.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzyhosjgv.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gxsxcbdyr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxymrpqiy.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gaahjguhj.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gcjjugpga.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gdaqygzmw.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gpxibzwlg.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gzvnygxzl.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gehwhecky.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gjvaoudsd.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gkmiohijt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gsmcdoxkg.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gsfezulkh.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gbuexelax.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gshfukkci.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/goettdoxw.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gaarbzvse.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gxfwkfqcu.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gtotbecpg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gcgnrvkpk.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gdxebejai.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gghpsqeml.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gureeiwmp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/grfkcwfdz.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gwmwuwtbf.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gpfsswrgl.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gltzgvyjr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gdiqqykof.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gbsuolcpd.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gtxgqpwkb.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gmwcgqtky.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzrmphmll.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gmtykkkfd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gbyiurgjd.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gfzdmdtjv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gnallpycv.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/ghktuimtg.sHtML


<!-- 参考信息 -->