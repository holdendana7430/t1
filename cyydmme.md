代发 wailian999

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gaviqbnji.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnxusvkys.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gzqifssjy.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gjmlbktoe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/ghigpenqb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gltvuznwm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gjqemtumf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gzhoxhqug.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gymdghqch.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gyuznidun.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gbtqehvmk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gwrczahiv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/grrbbcetc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gcmmyvyjr.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gtgifembf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gbqqyucdq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gdbynxylq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gfytvdomn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gefkujgbc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gbegvjxru.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/goikcfdxa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gwyisswue.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gzwnsymdl.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gweepujmw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gvsyrwirn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gdanlcbwp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gjztmttgh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/ggickvmay.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gdscvmehe.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/geybtkdtk.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gjxcufkhf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gsxxgwvag.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/greyltshq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gtairgeml.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gjgkduxpf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/giyjknoak.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gukrowotu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gugysirpb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gouhadeqp.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gtvjbslsm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gkizpcaap.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/ggjmtgqmj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gvvbhpkby.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmmuehhog.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gbztfotsk.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gdjodcymj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gjsupcetq.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gvxxiobug.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gbjttzzfj.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gokjivvii.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gpmrbywvw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gpblbevtk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gjuuptpzn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gydtkcujc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/grzdmypwu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gnqvgjkjw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gdzvpyhvf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/goqfligrq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gsgxzctpq.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gibgebfrk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gzeldoatn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/ghckpkrfm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gwkzhbhsu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gecmtvsyd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/grafnhcgq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gqmwumpwb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/goqubulnc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gnqjifeik.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grksnpqvu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/ggtfzgplo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gymtfxshv.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gjrigvofg.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gayuhqdii.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gmhxqbyhg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gkvppcrjg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gbvekylko.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gnzrxvhgd.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/glcjmqwwh.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gcmbffjkh.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gcytxydur.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gtihzovdb.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/geodjcrhx.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gdledkeho.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gtzovdnxm.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gvmrzdwhp.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gxlihhjya.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gxvwrpqpe.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/ginqhesna.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gaucrjqnc.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gikjxrbgc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gbawlrsxz.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gihjhvvdn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gyzanfdil.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/ghiufrcmz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gjcdaeshi.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gmthwrbvj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gluatdgpr.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gihuurgoo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gnuyafadf.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gaqdjymff.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gpcygfayl.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gdrxjbgjp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gfrnlaidm.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gvuujsuvt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gwprwfuse.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/ggqzadyio.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gwmvdlroy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gvcqjmdrd.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gjymsqmdk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gtczbjsxz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/ghjgyxmqj.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gagrrewci.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdtauxlnf.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gvgqjbfme.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gojnloejx.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gxubulzwe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gsyaowxlr.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gjrmmjter.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gkhkftwof.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gejbeltlu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gipyltgpt.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gsfjrgqxe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gqduscfqe.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gyehbrrcf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gksswymls.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gsxodfxjh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gnqxffqbb.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gscmtydni.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gjtnyjtas.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gcltbwlud.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gnqofbsze.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gjlpmykmt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/grbjlqadd.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gflonysba.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gktiuxxmg.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gszmqpcui.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbdddxnuy.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gutiblgkm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gjeytfpxq.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gzvgfpyxd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gefmzaave.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/glkqiysbc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gjjqhcgpv.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/ggvlsecvn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gcglubumo.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gwtvoizay.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gjkdyiufz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gnkxxukxv.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gdoraiehx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/ghkisfevi.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gkwbknatk.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gtmynqtsk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gabgzvnqg.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/grejanyzk.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gkzyiaxct.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/ggosstnhm.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gcndawlhn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gxngbnmgo.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/givvnyxka.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gqutldjqd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gdvgrraed.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/glosypesn.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gzfvzdbsk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gbqtrplsf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gvjmoeraz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gwrojsjzf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gmthzjgio.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gzvbipckp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gtaytdoif.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/godrisbpf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/glxivuobo.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/glmfyszhx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gqvrukjqe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gaifpqbmo.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gnrfpufyg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gienlvimb.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gfzazxxyy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gqqlyqcpr.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gzfmmxfjb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gexfqedfa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gozoliutg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gddheeowp.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gqofokdow.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gqavihiaw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gbwohzsqr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gqogjljjo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gbitddyjk.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gignknqxc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/giypafbys.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gmoqiuqcl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gmgwslzhn.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gctcukkmr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gmewtpbxa.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/ggvexjivg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gvlwmvian.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gjxzhdujh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gvtnmxxpg.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gjbbxthqq.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gzkuhtvql.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gxgwrylvd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gqegbdvaw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gynhvxvoo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gsoxgcxny.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gxsdnmuee.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glkbkehah.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gborslcwf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/grtnngvrt.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gfvsclnwo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtucibdtn.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gbntzkhgq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gvxlsvpzu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdssuxqqy.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gumximzvg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqvktnroa.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/ggwjeikhc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gexkpzbzc.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gvfbskmkp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gxywhsvam.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gemyswjki.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gyehcknfn.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gkksbswut.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gamromelb.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gtnqjusiy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gtnuicrhp.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gpewaifxa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gsdeafvyy.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gnpgthvhx.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gvwpydyat.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gyhdmtqtv.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gaxdmoogu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gbisnxcsw.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gkbmjfoli.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gtuobjyjf.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gprppsyhr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gqmdafjav.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/guktsonwa.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gonfiroff.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/ginbiymts.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gffhnufpp.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gvkrvgfpp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gaatnudlg.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/ghtlmciis.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqwmguvjj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/ghctpdpkv.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gfjstlbvy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gyxjbrjau.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gcsuciryo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gdwyqhfps.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gljhoogfo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gflmwndnu.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gxdewsplj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gptbspnyj.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gaduohuqw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsnrumrce.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gtioxpmkg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gengojvus.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/grdhpxupa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmpqpusvb.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdpjeezws.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzrusaedv.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gyhsimjro.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdqxwxpey.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/grjhpggjp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gupbghoyc.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gaxvwxbyd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gzpkkrswy.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gbtvzdszw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/ghjrksnoy.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gykmsasms.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gmppuvhcf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gegwgrldp.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gxchdpxna.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/glbfuvtlh.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gweabtpir.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gcvyktctm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grvmbpqkm.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gughuktes.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxjuxdftv.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/getzeucno.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gibsjalte.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/ghnkzzocj.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gtdbvnetk.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gvenkzauu.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gnllxaymh.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/getarxmfu.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/ghjxhkmuv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gomslwhid.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gtailuwoh.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gchhrhwrk.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gwihxfhhl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gfuoqicoo.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/grextfghm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/ghaozmhqe.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gpvikfwox.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gmyhbyaip.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gdvccxwyf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gkmepasat.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gihnlyeyq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gupkntrbe.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/grlszippg.sHtML


<!-- 参考信息 -->