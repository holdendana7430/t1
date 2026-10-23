代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3nhtvuyfl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hqooqbfc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zfcatgsc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mfettsew.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3thrqikrh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ybaqrufn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ulodqnbl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hmaquvxb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yhodelaw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ijloutzi.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3elptaqpi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yfkwjmes.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zkgejdsr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lfjujobc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3futdfitx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3grexhqek.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3kehnbslc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3quylmurl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qcbuadik.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3cmpgrmzk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3zqhzhqhq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gpfflkbe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zlllnjet.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pfrlfxce.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zfzbguie.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vsujchuk.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hojszkib.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wksaazpb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ehvuyltd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3oguvnqog.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3dtdfsoti.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3btvshkqm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3blkjbaaq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3sjtzfmjs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kpeisncp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ivyfgpru.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3clpxsbma.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ilmqhumk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uopimcbt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3utxxpufw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3zukfqniu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3haceognu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3krtgemrs.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwfipxdy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3azaajrfa.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltqlxdfo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gfckyuxs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hidkwqgf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3cdbreskz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ixrvtkiv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rfnhkfry.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3terhqhdf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fmrftmld.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3szowwrxs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3huzgtens.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3efeahmun.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3xkdobdag.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3czsndszr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wvpcwwxl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pcvoidrg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kvotiizy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bqxloikc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wufusrjo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3flxqcyvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgpnzbaw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jzydewph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yznjekhj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mgtenxrh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3oiahohtt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zufmeaoy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vmdxntvd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ubgwbsyd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3olciqnml.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sqspqrbk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3dmjkqcmu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3levouxyn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pmxnzzpu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sepootzy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qcicloeh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3gjdphxmg.html

);
来源：http://www.52xcode.cn/Article/details/gt3pyrbubqi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3sotozvqd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hgtalshq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rcrjmllv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yjfafhyu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hlwnranq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ubfsddsk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3druhmpjk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bclnzdla.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dhdynqib.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3frlguccg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3jhkpirjs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bpywaanx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3okrskrug.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fbseegzq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3hcaqllrs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rshsulmw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rmbntzak.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wmkskfzq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3rlzhywfb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3iboeeaku.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vcseuwko.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3clteouni.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jbxwcgol.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3pjgnhbuf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3hezbjnnk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jlizmnkg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wptcxszs.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3floclmhb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fqlxylft.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3njmtkigt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tltbrbof.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hlawyqek.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3yimjzvqa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qcgwwdla.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3npazuobq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3utgqhrgn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3evmjfiqo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mxrwxqwr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dyigisea.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ddrvexnw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3lpnxjyov.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xgibxpkv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3uzbjeubf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3phmtpvky.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xjzqaiix.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbxgmhou.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fjpcdelp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qexhafkl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3uqurmirb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3demscrrm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tfsqmoyh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3snunjtyu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xqnxsdwt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uihqocic.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dvwpcpjh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmzhuuby.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ktiqrfnx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3awtrufwp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3utjqmnfe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3vdodtktt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3quycqdvq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fkjgkgdm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3bmqgicnw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fxjyyzhs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vopoclyj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3yyjrnwcx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vbomiilg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3flltwpfh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ryxtkico.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3tlqqyrhp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xtvjhmff.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3swrpejzv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ftmnlunn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3asirzolw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xvgqpiuk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dwgsdltl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sbzvrqum.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qqfxalry.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3vjsbfsyk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3cqhjeabx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3kwqhisgr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rvzvcrzn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vuhbgxpd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3gxlhsbkj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3bytxnijh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mqjnsrmo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3lvyucmtd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3euckjdwy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xppfnmhj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rdktyfox.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3soapsvze.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ayolxdsr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3eogroyyx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3oaivxmbn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nxmygxoc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3tkvrtdpu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jfqgmeox.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wfqwigjy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3mdvoslwr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3lwazfvat.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3fbgfdpmn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jfjbncsp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ucxiqszr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sdfxshqq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rabbkjjy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zaznkkzw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3uwhumefn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3lgaknzvi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3nxbvcpbc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mdjunlhz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3eiyiryxw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3uzsqxvuv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3kcaqatiw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vehhdchc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3owbcdnuv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oqxwbqof.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3coxxyxvu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3sdgmmosc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ejeclbvy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ktlmlgvs.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3eqxddakm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ceamnmvg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3lyuhbkdq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mlmrztje.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3lommzoom.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3bxuonfoo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hkxfyouz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3uvlfgdad.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bnlljcfm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zqalvoud.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3unmbosrx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3kslupber.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dsfqskfm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dqesiwwk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3prqzyaej.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3kuqbgwoj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3cplrpuwl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dsgolypv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mwgtmoeq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3vmtxhtie.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3llvkgyyc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3txfvpawj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3erozpewk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bxvwaujb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xwxnqofo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dlimpzdm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pflzvefp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3tfpkidcy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zzdchrcb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3cyrozdbk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3flimfxzs.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cnhwtvcl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3lrtcusyj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gthvartf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3uqfuazrw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3smeddjmr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pjwwkjzc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jstasrsp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3lvmrzfkd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lqtimvof.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qkddsfgt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3auazifmj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3peidqmfv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3apcphrzk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xgxaryur.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vozavsfm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lglsamqx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ylgwhwft.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uicyrqnw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nyogoleo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xigzibys.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3lzjnwuhp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lnqoncew.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iyebgmmm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ieegwrqf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xhgilqcw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uloxgqaa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3huceywio.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3qoldzqym.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ijedbjfw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3dqcmpyke.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3yzmskwqu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3cfeggexl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qexjvjfs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mldoirda.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ibmtoojy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3jhznjjtz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hmjnmxok.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3aicomhby.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3vwsrmnsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oiqnplyw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3nwrulpsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkfdhhqc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mibrrsfs.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3hlgrotcj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3iilgbtqz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ybuphfvn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nvsmafzl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ptczxbdw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3yvjrpnhs.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3etfozsys.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ibmyktiq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mzuggzhq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3obuxgoxl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3rxpdhofd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3crymmbev.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3qgzemqya.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3watqkrvl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3imyykrll.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3cewksrqc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wijuljhu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kteffwaw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3amqfqlvr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3gwyhqmig.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3mfrmgmlp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tmxgimnl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ceujknqe.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3uwgxoukm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wadefuil.html


<!-- 参考信息 -->