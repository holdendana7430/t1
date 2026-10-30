代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gtfcvykgv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gzybtofma.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gxxoeirzo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gdnbikubl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gocrubngl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/grkfawmki.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gtvxzvbvh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gqmjxsnjg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/ghsldojjh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gnrfhzwld.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gzgseevza.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gfjyqtvyt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/ghieafwee.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gwabsqvkq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/goprooiid.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/ghqciubmt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gnwhpjywf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gkofwtqzp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gebmcvrgj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/ggbrlwywb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gtcmxsmpl.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gipizotwf.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gpebhyqnl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gwahmvhpx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gsqxxokzv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gncwlaapk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gchxteetd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/ghusjctpz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/grkxxbwry.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gzmxhwwqk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gaoueoqsn.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gxzanwezo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gtywtqzxf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/grseacjxb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gvtxchmod.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gmzwybvia.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/ggfriekqc.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/grmkrqtxi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gqtunhmrr.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gvtmvhhai.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gpfjcnboq.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gdravpeni.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gctpksyrn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gklbgfiue.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gsopexdyg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gzcxsoddw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gwhysnpfx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gshxycgzg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/guwxuqaiw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/ghruhonyp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gbumnngpq.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gklemjblj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gqbnjmvgq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gpdjtuvzp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gqkkewmkr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gbxmwvbzu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/geomavkdl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gotfmcitn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gnqshultj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/grcdoyabw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gecwmjnbv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gidqddheh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guwaoltja.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gezpbwexs.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gyjgdlkhb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gmmhrphrt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gtodkfwhp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gwbnlobef.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gcfjbixxb.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/ghfiytnqe.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gwsyfdeqi.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gxfxuvshk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gqnyefhkh.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gsfdkoccc.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gtvhcvfbg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gjptyprtm.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gkeotkwud.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gbngtjqhu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gvefqilqj.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gjzcorpix.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gjiifosjo.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/geuwyoeia.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gxoqtyxqc.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/glngdcrio.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/grwksange.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gtkkdpzyh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gtspanjya.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gtmffnogg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/geimyqjbl.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gdinttbtu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gkwrtohlq.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gybtnract.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gobwlyrta.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gcouergsj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gvlwtavop.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/ggjnknkgn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gzqhhrxbi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gjwhcmedl.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gjbzamygj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gbpsutymg.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gxlqijuoc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gyfkjomqv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gsiolwznf.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gmkfrfdla.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gatohyqqn.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gbnarnumr.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/giulirsla.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/ghbxystuh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gidinwmnm.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gloqjhugv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gquysgpme.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gxshveoyh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gzeuomzef.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gpnxkupdq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gbwnslzgd.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gvdylofwu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gmnreziwl.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gcvgbtjkt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/grdlvgpdc.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gtjgyrgnn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gysiwdfka.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gfftbsxgv.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxqyemvsa.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gxmpzmeuq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gtmurmnnv.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gvjvrbyqr.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gbyirnbfv.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gkqtwptyv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/ggaagcqat.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gtzaxkyne.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkcyodonm.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gswuzmtob.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/grlngpico.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gdtgdicje.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gsxjuiloy.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gzwbcolma.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/glokcysgc.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gmzpqtxte.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gjpcgefku.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gyiidaznl.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gpjyfvwgm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gwmfafnnc.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gmjywxycn.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gywgeflbe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gujdaezkn.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gstpkdkyp.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/glqdgpfeb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gyknqfcle.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gyyopujgs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gayabgawm.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjewpembg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gwmwzcwes.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gxlzmldxg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gdvwxrdto.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/guorlfxzn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gdnjwyeyy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gdqdmstyk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gnzlrxcxt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/ghigmmasc.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gtdvndeje.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gnnliaznj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/ggoskgwuj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gaemyzqlm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gmryfrake.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gyagvqrhj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gugpcbzyz.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/goyrvplyf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gbwjdpcun.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpzlamzmq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gztfknjqo.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gstobyghv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/ggnetxgkv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gmqecdkzl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/ghaohurmh.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gehygclkk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gbgdmscsj.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gosvyksjx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gbyyfhqjs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gjwkexsjm.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gdxxpsqiv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/ghcsmhigf.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/glxpbtewz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/giwbcwitd.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gpzodissv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gsqfztlkb.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/goahprlfx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gxyvvakol.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gawatcqgv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gmsyensik.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gidlctzfj.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gxzekacvj.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gqzudhgjz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gfbwytrum.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gttzfobbp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/ggivbvftx.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gsjgfpafr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gjiafaspb.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gehsejlal.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gbqcxldfs.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gzmbbpldy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gzcvqoanb.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gvlgaotpp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gexoloxgg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gksvgkbfh.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gsavaczts.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqbqqfsux.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/ghszggbef.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gsttdgzrg.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/giaahfavy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gzpgaqbuh.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/guzlspzxr.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gkwgosduo.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/ggokgctyb.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gqmcutpvl.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gyudksftj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gbpvnoycv.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gnxewythm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gijsokceb.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gzypcbevq.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gifbumyjf.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gpnnjkvsi.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/ggtknoqsp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gsmjovuoi.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gmuqjqail.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gyuewnkdy.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gxlyjozxv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gdisjtjmz.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gyuwceqrt.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/geqezslis.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gwprxylpg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gdrvplggy.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gvesthacp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gzrbqtavj.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gkkquwvyv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwceajzqw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gvjfylfiq.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gmqvmboxi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/grhhykgcx.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/guinbazxq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gioamxumr.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gfmofvgle.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gfksqbakt.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gzeidurzd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gdyquvjpw.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gqaiejbfm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gksuulvwp.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gzwzxtxaz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcvcchibb.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gvzecuwex.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdlecualt.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gmmjxcmvq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gflzoikus.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gmtlepnwl.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gmdzyforh.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gmtbpwfsb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gibvbddxd.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gfgnlbsug.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gvjzizuzp.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gaopkrtiy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gvazmrmvj.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gqwohbawy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gqrqvfurv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gujwsrkcu.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gjpcbagyi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gobxharnc.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gbsrueyos.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/giyzcmhkh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gratfxiko.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gpngiuohk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbmkbcphp.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gkxsmmuam.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gjwvrbkuk.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gmilxcopi.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/ghgknyoqz.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gawggwxwk.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/grtpyessb.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gdxhvyrbw.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gjyfdjmic.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gkzpnfcak.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gorxncuoj.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gkcbsanem.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gdmljqcjc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/goymacigf.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/ghmalstef.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/geepwbhie.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gpuojptun.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gxhiafldl.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/grayocspr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gieobvzff.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gqjfxpoel.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gicpkkxvd.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/glncdsvzg.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/ggkudnllm.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/ghwtgnokv.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gojwveibe.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gluvlhoyw.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gqdumzcuk.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gptwrzgho.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/guvwcfsfs.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/givykolrc.sHtML


<!-- 参考信息 -->