代发 wailian999

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3znjmcisp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qruqeynt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ejpvqujl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgobdvxw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3aptpklim.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qfrpeeak.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jnalirzf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qcyjjhpa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vbuzueyo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iivyjisz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yljbhbwa.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yeqjebyj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3zgfcqpsi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xjivtedf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lvoecqet.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3sjivjvlc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3axzcksfa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3gdsjlrua.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vityaprd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3lwmbwdyg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3nefxvisw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3bwuuufkm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ddrooeen.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ympfrqrj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3hogxxpij.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3izzkxxdv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kygpyvxw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3janrsssl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3intcoezk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3gdygjbfc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gzjoccfu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fluhparp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hplhjaoe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jnogdaof.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3oqfarwsh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lqpkvdvm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vqihkslz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3hfppafap.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3eivgpdjk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3itzhhzuk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3wmxfxalc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pbufmidc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xsrnnhib.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3dieejbtp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rptqixpg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3grvnzlca.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vmwjpunz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hsmxvhsp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ofrxfvxq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wszlahzx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3rdkgbwyw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztzffmhv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3zeiaapyq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3dwwldplo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3midxwjmx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkndhowu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3hiqmzwem.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3fwsfufcp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3eaihwnst.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3kptnqwyu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3kgkmybet.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vspwzztv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wfdvcetc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3izrrzuhi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3itktpqos.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3yxsyldfs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3iysyjrvj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3eebqeozb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3rxiffxiy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rsbwtrjz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3yzavfjus.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oontwywp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3turkmmbc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3wminijpv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wevsldxd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pwixyimc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xnbcgpex.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3glmtaewx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avsayeqn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3btbxgvsr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3tnckoewy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dcqifxex.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cqkmssub.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qbmrlwpw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3dtsvzrnb.html

);
来源：http://www.52xcode.cn/Article/details/gt3osyemcma.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3qfzbmvcg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3pmrmfxry.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dmkoduza.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hyjkabvh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hvueszpl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vqnooxzm.html

);
来源：http://www.52xcode.cn/Article/details/gt3dqxgsahr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kqinqnsp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dyixdrqg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xbyyeyhw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ntxdevla.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3tshkkvrf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3sxmgowai.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qjdccyov.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3skoaigkv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3bnlimqlm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cbhroagn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3urbouurq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3uypqnzah.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3rouvvume.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fvjgluqn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3lvjyyzon.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tghwykte.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3crplyqqq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kanknqvd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zbxqvkyw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3dcoyrmsh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3kymkbrgr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3lpvlozyu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sblyuxdj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3fxigqwlx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3snxwexyf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jctcaxxf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3wcpxbpit.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qvvzbyzh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3cfrvyzwk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kgvfmwan.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bjgmewqt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xxwuhapg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rgenvtxc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ztezdver.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3whlgnfim.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3vxdtfrly.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3utaupmzq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3itkrgcql.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3igxfssrn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3yorjpzht.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3kgujibxq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ozbhcrma.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3phxjchvw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3qcmexsdp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vmwqopbg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3icjjwrym.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rfoaiemi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qnqhoamd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3kcmhzgla.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3twomwlhe.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ckbyrqml.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dhjsaslg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vudcxsst.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tielqxic.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rzvrrkzt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jgucopai.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ixsqvimo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3flhobaud.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gbdeqjak.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bokvuhfm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oanjuwmw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rekjyfwh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3clxhwuvl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lxygyych.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3grefkize.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3porhlkyh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vkepbjpw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3vvulrmfw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3iesrlpcj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nppbnusl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3owqpikjk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tjwefcyn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vjxfeuth.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3iodgibrb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ksyrrtkj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mwibvqte.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3wmwgdsse.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tibileje.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hudlavbb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3reszltpm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3siyauhga.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dlxxlaah.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3bryxzuei.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3soifiobs.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bqmqjsul.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3tanrfoys.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3imnlhzlf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3gewahsuz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xtebdogh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ouhredxs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3hqgkfoid.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3basjevbn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3zbqpeqjl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3cybhudal.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wsxngrjo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xpqjcqbe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3acsncilu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3oygkvhjp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3dzltgxgr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hkxrccna.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jxjjxaet.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3xbrzqzaq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3gjkaluwl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lpbibtpo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3inpggrtk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3abcyzkxq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3deamgeco.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gmxpsrix.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3rmrwxkrs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3clciqror.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xbgtvosj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kkinylxn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3uasfzecy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3mimxpegp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hwarcjqc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qdcokrwz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ezqsixly.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3drbmdpus.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3guqqzlyk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nnqcnfwc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3nykrgery.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3illioxkj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3yzhzkcty.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3webynybc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3myigrisb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3uicazfeg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ytmaekfr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3smlihjun.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qtiqqyxp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3znjmtccw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lxcdrbaa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3oilgxztb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dvkdldwu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vxasdbbi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kczzpwkk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ccpjlogk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3iikgntev.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zlvqikiz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3daomyioo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3djsdrond.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3fxlwdwke.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3oqrhygtc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hqzmtmxd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tvlqtdms.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3llivpbdy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3uojjkwdv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3zluopgdc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hgprptvm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3trahpxwi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3cogmjtny.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3nkagxgpw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uijgvauu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3frjmitor.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3afrbzvyw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3tfcqyhtn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wxqkvirg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mtohymrl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hfdobsnw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3kzgnprdg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mqwpnsql.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qbwuvclq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3tlwankva.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3pgraubin.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3cjqkzlbw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ruunqbqu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3omfoetsl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3nosyhqcy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3nseccvrb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lhquoplz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kpkdebdm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tkmjxrwu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3gqobywld.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lwjhxnqq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fkfuphgp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dpjdjypw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ufbatsah.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vuwekgad.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ujsatnyr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3tfpyuzte.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3uwcxhuvw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3otprcnih.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3upxzqcrf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kxxgeyrd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ldafiwxy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3enxhcade.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cvfvgedi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mkdvyboy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3smtusbpp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mokokcyz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dohhipmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kayskmec.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ndgjzdpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kunrxwun.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zglcqndm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vjhhskhm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3nfpwnxrc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jqbinwjt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3gqdjybqa.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3nwaanqwz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3sykpzoio.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3jglgblwn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3resiktbx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pixwvzyx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3fdyruuvz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vzvvdbql.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3psxhnumn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3pmosnomq.html


<!-- 参考信息 -->