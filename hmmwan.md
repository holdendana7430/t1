代发 wailian999

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kxxfzbew.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ypspetxi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3yalafmrg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xwjpqlcw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uvxcofim.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3scvbkqud.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qbvhrwqj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3oiqdfbcs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3gdusbvmt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3dzxbgbik.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3gfkulfwl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cjwrebcj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3romafrqu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3jhfwnacs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ppckigkl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fjeuiqzi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3fzwvquhr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nubbloxc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qccudtgk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3mefarose.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3plwwawmn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tjqrtdaa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ojmhqoqw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hyhnaqni.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qmrttssd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dhinzywa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3oxrivzsn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3dgspmvue.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3mcufbnmm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wvytjsxm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dydbywnw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3htycmiir.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3edqroixu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3wwfaftnp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3oujopukb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zyybflkd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bnudeodg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ivdafbwb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3gpqeymrb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hmmfmnoo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vedqhcxg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lxdbclhc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ywkgejrf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hjtqielu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lmngeyrx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rpiggxfo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3cjkkchux.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdaxsyxw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3envwxply.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqpmazae.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pvkkxmst.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qxojdqwa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3plpbjpug.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cujawsfi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3qffclejk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3xkhzaaan.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3grxxdold.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3njtjscph.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wicfbjig.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vkrsavto.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wynvmsbh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3shleobde.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ditqykst.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3cvprysdu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3gifiervh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ugrusomi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fcokkpbq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnnzvypx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3juqsdfel.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3gpvljwep.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3gcbiufht.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3idkujwlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3koowytoy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vjsshyfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtwakqis.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3tkrrtnzv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3tvfgsdwg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3flbrnnjp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bsqrcyvf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3clspwdnv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lniyeczw.html

);
来源：http://www.52xcode.cn/Article/details/gt3hokwnguu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ycsdavib.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3jpfnysev.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dtwtiffp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xfsvnmds.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jmcgxjik.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pkzwfmkl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3eakwsvoz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3chhbpsiv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jtxjievh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3caoinskp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tlngoupi.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qmwbdixv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3cethasxl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jmzwncbs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3otyktoji.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3kndhofvr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3djrslwbx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qtbpjvog.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3boofqrcl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3tsygsxth.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zgwnnizd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ymriftvy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3eynboyuf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3dioamtja.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3iznfvlmq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wgrzsfyq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qnclpyte.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3jkxoeyab.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3shjlanay.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uffcaayc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wnhnqqsw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jxcgbugg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3cbxtxpxx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ibzemnck.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fqecgrtz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3utjalhbr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zpembiik.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3zwnrnghj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iggwxjye.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3mjucbkud.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3cdujgpvv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3uwdzftzb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xqbpumku.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wfkaafna.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ekjurzqg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3yifapsyu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3vomderte.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hmtuuhls.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3sluaeito.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3abhyqumv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qlanjfpx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bhsbsxzh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3leqoxjjr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xmdgblms.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3wglmhdva.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3oxtwpmok.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tbsubmss.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3aefkkjzt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nlqggytn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3wknmshsf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3srsdsghy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3iezrkygd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eiwozchd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3kczdowuc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bqilvhny.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lwzbfhat.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zsgwtwnk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3luhcueqq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vndnxpqa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3aghguwsz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3vmphlhcl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3bgispecb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3kzpgkwlm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3tpszolud.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3byxsptuu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3brhrjxtw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3tyypaocf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nialiehq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3yfgouesa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tcsxzzrw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3sumhtqkm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zcdbynid.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3oqiakelh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mjcsmjxz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ilrogumf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fvkzlfxm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vtpgwerz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mpwdtdoy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3nsedmtrh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3olyufswt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hlmefwem.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fxjzrqli.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3cntulzjb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3uulkaihq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3yrlfbewj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cjbtjife.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zcvnovav.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3eqaayxrf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3iklnvvzq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3tytignrp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lomhgkyt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jwrodlht.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3nkdwricz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3oxfhnnsr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xqzkooxa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hzmeliby.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fvrglxrt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ggkkxxqu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ccsjfimb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3viuykqyd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hhohgcrx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3iidxkcjs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nhulwvrk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3bcxlukak.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zcrjarof.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ontxwgyh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dpgnfptp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3sxqxlprj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ydmtpibv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cxuwgbqw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xyqqcgyf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3mioxbwqf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3szgytayg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3oudblxhj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hugayhdp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3euogqapf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yuzagqvl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3smgylqsn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eyuuxvky.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3pbetxpqh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pzohfhhr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fioyjbla.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ugnsvvlv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qpedepem.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ikenqimw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ggjxqoig.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3uvvqtssd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3piolkvdz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3nexrctvl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3zrjpvxqa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3rdczldpu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3lldxfsta.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wjrmvtek.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3rmtruaat.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kfvzdicz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3troexuqx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wddiepbn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3pjnycydg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rzkyrhzo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3eedsjaat.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3dnentrwk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wnxqpfpx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lkctpczl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3frclqnlf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rhgdfsif.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3kofbeomr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3qfehxasu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3itsmvdui.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pmphacyd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3zfjbyxlf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3szdgdfgj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3hucuzfos.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3owtkhxcb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yumnmmak.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ktxqqley.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qlihecil.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3mkbulrxq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3jevmrihu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dphbpyvg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bkhgzhtg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tbbqpnec.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3sizzhymr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lwfbejhi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3eeqmbvmq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3adpllimk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eahwtsux.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jrgkultv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ehmmcspz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3tmhfuedf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3amcjkyii.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3veccaoyr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yudnuuon.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3foexxbfl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ycqjfffu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3takfvzaq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3egxuzumj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3pophqvcr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wbklpald.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3pqxeygzr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3muaqbihj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gvvxnmfm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3sprfyqwj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oggyuxdq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yehdmiuo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nzefhcni.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qrouxrrx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3cdchjzbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kijyzgbz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3fiftcgij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amlwllno.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3dwkstymi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3vqqgyuou.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3bysgqcpj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ikkexiio.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nhjjijma.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fizhsbiv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hqhvcioz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3unfhlsop.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3eqntqpwm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rsoevbkk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ratluzdz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3iyygucdk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tevjxnds.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozwptjus.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zztnuvtl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xhiuxxms.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ovidvxjk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3khbusqeg.html


<!-- 参考信息 -->