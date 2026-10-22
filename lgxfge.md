代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qxclumam.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2naqojobb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2dlmzlsau.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wzfvlrts.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2sjwxdvsz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2htxkkdzf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rbugoftf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2knqvucbp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ucgjpbbb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2oqknhqul.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wfeqytbe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2apzorchf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gwbmmjcw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2rzfwexcz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ljqaynld.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qjzpmdnv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2fzxlpczc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2brczbrmt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wighwxcw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zmuohcbh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2gmjtbuwa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xspktbuf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fxkcxolf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mkzrorzd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2jcgawhyy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sudkzowy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xnkvrphc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sbjzkenb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sbpahbqa.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2kvafxwao.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2edmthbqo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uqjlntqi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2seinztsa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2oaogdeqv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2prslolzr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2fbsbjnds.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pzuycjbk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ovtpmjlf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qsdqpvwm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2wmrzwefm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2lsimyjdn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ygcadpkc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2rhtrbglu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wtivhass.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2psmnudlf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2bxgjfiwp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bylclokr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2apnylrqt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cdnrsmad.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rkkkwgqy.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qnqpsrhm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2nphbfwlv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2aagetbzc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bgdykdaw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cepujzlz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2fignfwja.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2kvhqkwkr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ivrngapo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wyiocgaa.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2svyzxflk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ilmvjzdv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rrghsggy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tyvlmfwu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pwrtlszd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fypquqii.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2oicwwuxs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2fryqxqdi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2hfzxsbuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdzqxryo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2vdcfcqfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdnvbvch.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2cdlspwnc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vhnebrvu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jjnhdxvc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vdvvzpiv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2kwlzerpr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2vdtsvdei.html

);
来源：http://www.52xcode.cn/Article/details/gt2fdzyelyd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2znfbwzit.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2hjmgpjoo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cjwbuabj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hmfdxsvu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wwbcuhok.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ehytiuvl.html

);
来源：http://www.52xcode.cn/Article/details/gt2ycrpyxkg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2osgcqiko.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ioowltfc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2pzxalxwj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qpgeexrg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2cnoshrjf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dczovhiy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qtwxkxly.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2eqoepqwv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2gynhmnsr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2deeawsbw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2bwodetfz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2oingygyt.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2vzacvsea.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pkuxpekz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2dxblepwe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ryvtethl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2afyslywk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2udfyhwez.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zgokczua.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ewcfurmn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jbyfhboo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kncbreai.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2aoeaxjzc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2muvwfbgn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2drgbqawu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2cpmrqlqu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2flqkjdqy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mlrpbvka.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2jecfukum.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yiysbrro.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rkffvlhd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sehlazdf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2vmphpugk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2aibzluvh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nqlbofzg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2mnbsdfmb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2emtwhuom.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rcfrrmye.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2iemsachy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2utouhwth.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xrepurjy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qxscgxvx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ycorfdue.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2aqbvkxfw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vafiacbl.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ejhcfwnx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ezxhtfci.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vptleegk.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2mkbwlylb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oowjdlzg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rsrrbklr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jpxvisow.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2kegryiak.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qxvtmrbr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2flyzylkf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2frnzpssg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kufdlskc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rsemyird.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kxygnlvz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wsgedhpw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tnpupigv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pzypahdt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2pqnmawni.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ubmcfsxm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2quxxgkyg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2akxjcxor.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2sghsuvzg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2rlosnakr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ovtdbnsm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2eumhkkih.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2inbcenkn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hqvemral.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2iuyfnwlk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2iunidiyv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2alwrbeol.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2whzhirzk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2rlzempfn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2yunarjdq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2mmuyfsdk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2uiwmzals.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2irbgwvkw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2rwpagzgx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wemdplle.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2itehqsvt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2sarfwxjt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ohxapqvw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ihtkeqrk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ahaepajk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pvcqpdsx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2gvebphgs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2gmlyaxyk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2gfdkwylk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lhoufcqx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2rklcqsfd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pyahzkkg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gglqxaoh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gebczadd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2vqpizxxj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vzlcskdg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xbrbsfry.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dfzsympz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jymogamw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rzqyvmwr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zcdbjjjh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2qmvkpjpe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2doqfeqnp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2asgqoexb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2iokajzhc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2kmxmjrep.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bljyvmhd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2lxhgfqyt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2svetdmgn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2nksjbnjp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2arvtqemc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2tsfsmiru.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mhjpzqzi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mwufrufk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lmtsvhko.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2fiytwkmr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxwvawda.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wpybxfve.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2amvvngmr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2mhkrteov.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ebcnocel.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2agfepwfy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2swpxmauv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vowxcxxg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xmfpwxll.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yznodyry.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ranygmnn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2adoupwwc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mgegtpwu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ougmvkcv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2qupvxglz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ekzevqst.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fqaadsbc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2gixhhwau.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2adqvmlzn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kltqxyya.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ozsgwjlw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2iqqkkjcv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zxpsuyss.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ezxfsrja.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mtqbgqil.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zxpyzrgt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2fdwcyhyz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2yhlzbdci.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zqcsduwh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2cdpbddji.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lzjmrwfk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2sdfpkftk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwvikqfu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fjxcevlv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2tibkhjqb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2szodrftp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xdrlvoyv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kngyhvak.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kswuesnc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hadhmikl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2pvomzmwn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gugyqmgj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jduakric.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mqvwsiam.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vfcidvke.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dxvzmzgz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xzzqtpxc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kdqsjpnk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2nhjquuey.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jienejei.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bipcwvjk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zfgsmwpz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rsdsfdkx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nzvdpubl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ypywiefk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uahhybfr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jzkkbgnb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qzzyhshq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2wcadrexv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ljcosumw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2vmfbtbmz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jyhpxnas.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bqqrpsze.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2snvvrtke.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2dqtlmgtv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2iegmklin.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ynmvgqsm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xstrwsug.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2rhruzufr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wkupycjl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2dsuhclod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqdzojer.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wlzhdfqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmqzydfv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jsrhcldy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qcghafuh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2knzeriib.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2dcpwdvsr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2etzvpqvu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2wwcrmoay.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2kvnlybeu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2lnkllrsz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2sjsxrwsx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fhvsbhor.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qcncfjjl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tskvlutn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ujmiwnij.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hodzraxj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2arrirvpb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ifadsald.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2evhvheze.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2neobitlo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oakjoxie.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rtfzhhbo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2yvlcvzph.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2iejvtilf.html


<!-- 参考信息 -->