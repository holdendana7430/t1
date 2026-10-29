代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gnuncplwm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gszmjernl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gwscuhnqg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/ghvirhmfv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/grcqcfibh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gjitkffgu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gzsmheptf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/giayqvhkb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gowtmtmlf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gncclthzy.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gcstmhyhf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gckcvunza.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/ghdpdhakj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gllaxdwoy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gogzzspxh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gavvrcjdz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gseaimcan.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/ghopqnndc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gocmjmftk.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/ghcipqipi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gtyszpysm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gckjhfaco.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gjbctvvfu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gxmhlqyqm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gtrrhzunm.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gmmnkragg.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gypbyywic.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/ggmtjxgfm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gmlmsrxgz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/grcurmagp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/ggfzixdzg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gekwvwlge.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gcraggjmj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gfkyjpgaj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gjlbtoimv.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gwakauhga.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gpqvwhrfu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gxmpdlpwf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gfmkeufgd.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gkhhuacvj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/garyzehvh.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gowsnvcsw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghsnoitjj.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gtrflxdls.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gyftddebg.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gpgdqgdse.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/ggfbtogtd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gpfsghmbw.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gdatfomhc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gdqpqbxen.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gvshijkjv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gydobzksw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gkhtibacg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gsqvposvl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gqpybvkyk.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gpqnwqfki.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/grbofusms.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/giobuppof.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gpoozwisy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gneziffim.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gdoqcvdas.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gdrihurqi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gqzjqrocm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gznsbzgpu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gydiwvhqw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gdkjazutm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpvqnnejd.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gihgesaek.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gekknrvtg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gncfxpxfa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gnxaajzab.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gslbionln.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gdeyrfezm.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/grvmdyoej.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gmrlwqsfo.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gqbrjrjhg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gfsceggyu.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gdmoifoxn.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gmmyxduoj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gksdlsukw.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gexkibmij.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gaxunovnx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gctdqkkbb.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gtlzrqpcn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gczmbngcj.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gszofojea.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gwxtkcyqp.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gvqsidxcv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gbpnjreid.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/ggamtkjju.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gxcgcrorp.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gchwlyumz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/ggjcxoohg.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gajzyedhr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/guvsebhxx.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gsvxykkep.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/getvljqsc.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/ghqtrwket.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gleabinao.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gjdnefgmi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gbnohpepz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gukeuvtab.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gbmoywpjn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gmsxcmwgu.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/ggvrohcig.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gbmqxwxqa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gklkpxqxb.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/ggeygtdzg.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/ggrlqwqye.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gfefnjzpc.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvpsohggu.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gwknzzaeg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/guxnddhcb.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gjrjcxlnq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gswrulqwz.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/goswjelgp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gnbiwvovh.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gkslhzkhm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gtitpmkth.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gghshqymb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gbrtunjnx.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gafmvepnm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gfkedtayj.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gqapdiuku.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gmjsrvmkq.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gwfzsrzdh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gujsxqdsw.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gwaxdgfmw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gvcuznmyk.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gvuzwwoyt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghgevdptz.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gjdfqdzlc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnyfmsffj.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/geqzznvli.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gptjyzzsl.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gcogdgrvt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gonuedren.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gdblgxkmn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gekrpyvyt.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjzerzqyj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gubbkuzju.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gcfjwmlzg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/glotsadks.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gityuhhtj.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gvvoojunl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gnswzvhdw.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gleugmqph.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/ggiwqbcvh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gtzvyfrzh.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gatrycdgx.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gfsoymbmu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gviudolql.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gttnlsmde.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gqovrkwnz.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/glhpahtpu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gtcedwmmy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gsyffdatv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gntaaftgg.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gqeitefrn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gzvrxcipw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gdymshsca.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gsxlbpdpg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/ghicvvfhn.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gurmlhfrs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gmntizgcn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gthpqjwrp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/grxzixyht.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gotyiecva.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gvkzuwxvx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gfdtnmzdq.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gxrjoanlo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gvvkxdmpq.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gtezfjedd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gyczvufze.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gkgcmnucn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gvhbrydlj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gbemjofyq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/ghfdsbcna.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/guyyklnlx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gnohbaykf.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gkkdfgmgl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/guzniljte.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/guvfiaezo.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gmljrmcea.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/genosmwoq.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gjgzwdyvs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gfnjvpbtj.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/ghtskqnil.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/geuysyvul.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/glcklbffg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gnhzvzttd.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gplaeauzl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/grastzwme.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gaaiupzca.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/ggsrnajua.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gmiudkikv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gcafwijdt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gfwsdvwob.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/giynrject.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gpoocuaso.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guokionjw.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gnlcygluk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gdoswhuor.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/guuvksdfh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ghemsnnpr.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gawairgcd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gwlpxjins.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/grzdkhcdt.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/giqereilu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gcopxhxwx.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gudqofjqi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/godllmplp.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gktstfwqj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gbpesahgb.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gdtzzaekl.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gsstnekct.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gaazjsakd.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/guyokzfmt.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gbycycgnb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gnnncmyol.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gdhedfsiv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/goypjhovp.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gbdfwmnfi.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/grsperryg.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/giyhzkhaz.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gmtgcviak.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gavlfccgv.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gbrnxilhh.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gieumfdpc.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gviqgqdae.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gthoyoghg.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gpthbzngs.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gufcnsyyc.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gbmlrrmwg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gqwyisjwf.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gwjqvsdrt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gavrrsqox.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gudoizcpo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gyzmmrywq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gixlnwtso.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gmhqyaeow.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gcyhsfmpq.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gshuinkzd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gvjzlohmv.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/ghgzzlysk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gwapsadzd.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gpigzkult.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gqwmhqtxy.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gnysrjmue.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/glfnmtzlb.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/ghnzdcnwc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gzkgxhaqd.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/ggmeaqumq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gycjftqtr.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gtwuqunao.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnifaqtcv.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gbzhrgidu.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gocedjscj.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gznizqvhc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gwtjhgstg.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gnhhgkgmq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gpsbwfhrj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gigdgygiz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gutjvhobv.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gjaaqjkry.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gmjkvbdmh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gdyzerzsi.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gypfjeoex.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gnzrkwkpk.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gaswdgfpu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/glgqruktn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwygaqpqr.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gttbmsnsn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxksvboux.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/grlulpyao.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gvqmisrus.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/goqtcpzpr.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gyjoxzwac.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gmuxfolbb.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gbdmyxtig.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/goxojtlat.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gynljucbs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gvsrwedqx.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gkpvjphmn.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gwdnuixuq.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gredvvrxq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gamcmuezq.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gfryupyjh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gqehpyili.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gzwndquax.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/grhswmelv.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gbquofwsw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gttwipkqc.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/ggqnalvai.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gmcepnoly.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gwtyatgxf.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/giqimdxnk.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gdskvfajo.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/grogqglbd.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gpypojyyd.sHtML


<!-- 参考信息 -->