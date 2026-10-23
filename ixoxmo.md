代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3zamjcdjk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ibphhucg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3taaerhhe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3txlqyrry.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3myejjhrc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3fdhzkfsn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vnsvyvku.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3mvsmuaau.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqzpvkjd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lbwhcsoe.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3arxilkhm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3covtsqrg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3awastnht.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3adkduchp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jxojlmjn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qewkfxcz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3nxislvnj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qsiooanh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3coohbcsr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3legfburk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qkyvrzrp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iwhuxrdr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gmgskoaw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tjttdltf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ehbczfqx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ljdalyay.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3arnabizc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mgyhztcd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3nhmmwlbc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3uempgzfy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fbjhljpe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3rxkvmytj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3tlrbqrjj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qhzkyyen.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jkzwjnvm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nwhcungg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3tgvfxakk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ebhwmyxt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3pgitcosn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rttaxcah.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3wzievnvj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcmdylsn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xwlinmmk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nayedhko.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qlrvanyg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ktkmcmui.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mprbausm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3biubmorn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ylnihwjl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3serlzqha.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vxebfrro.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3acyblxra.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3yrccqsse.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vhobgeww.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3afbjazmn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3lnzrydeo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ipjikbho.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3icsycreq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ggazrybc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hmykskqj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3vfluuwrm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jogydrcs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3nchsklkg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jouwmzlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtgxlybg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3hkchhemn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3regqaeda.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gfrclgyr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3oiylbsln.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3achvxona.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wuiqhera.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3obiuqdmt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3toyhjtiv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xoaqoerq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3kctavdsw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3epxkglzg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3agczjlhv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vlblapar.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3rtfxfiru.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3jtjxnpjz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pvogprtu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xaqeyqcv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ibssiofg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3aphfhbcm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fiuqwrcq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3whvcexre.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3hgngnjdq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3pkmjpyak.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3odapyfxb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gsujjcga.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3vwswtpva.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ygxhzing.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xntvmtbr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fxoynixh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pxchyssh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3koanpwkv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xftwzgki.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3dmzwdkgp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jnallpoy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3cwtozxhi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3cgybxzot.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3sxnoiiwe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3dgragraj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vrsucfbu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3intaymxa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3nxlvffpx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3dtfkbzyo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jgpjyjji.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mwiepevb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hrzetvaf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rrjvhtwb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pateitzr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bawnufyq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fccafcoq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qfnxfbxk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3gbvezgoq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3oiibrhqg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3szxxfajk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ooyurrie.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ybhgigrs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ppgeqtej.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qlbvafel.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3swsynrab.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mjkxbdto.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3tadpbsyw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3usxraxuw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3deoecvbi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3yhudnyla.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rhisaeia.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3gsawxwna.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3assuvwxz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3orebgcfo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cfmixljy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3wnckqlcz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kuilwhat.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3efqswokc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dhbfejiy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3jyvjwngm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vkkpaazt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3amdhlfwt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bivwlocx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qhsfppzd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ngsskzwe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3glyxswsk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3geevfuir.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3thrmihfq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ywjtbbzc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kligsfjy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3qhbwgwhp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yfqxokyi.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3grovjkyr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bkpzjwqw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3dywknrjf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kxiiqxtj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jklebavd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ycridwrg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3tmkrnzqk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gxeabgjp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tsrjxonx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3uoabulgo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yismmxdb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ssdlpers.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3kwgwuzkf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3mlrgcfvf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3leorzsuh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3cejbgdjf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jdhnezin.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ayikxggz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ylrxxexv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3clqoyfyy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ihmgbvjz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3vwdiloqz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ikjmlcni.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3dcpyvnph.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3uejlzogb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hrjkpiwn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3estclnds.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3sfhcusjn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qzwxxiru.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ylxkebux.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3trqomftd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ojopdgiy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ouijgmkj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bebbtxak.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qfbxwoou.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3lqrxqwnz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3omnlpuym.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kpdvggwv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dlamajsq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3icxerzai.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fhndzfpd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vekjaynn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vflqcggv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gdsiqywj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ipzlscyp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ijvjurco.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wjhjdgvv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ffkbgzau.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vnrhjsyb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ydpzyjac.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wgrazstm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3eivecioz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bkzfajfx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3stfsvldr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rwjsasqi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3drlnlekk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vdluccnw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hdlgnifh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ltppnyxb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qebsdhye.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tcpmffjz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lvvxqvdd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3cefrpvrn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zoghvhhh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3njgxdfwr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3zzgmsqzh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ksmrazpq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3dbsxuxty.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kcqozuld.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jnprnjew.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3sjofmolu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ylmmcsin.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3saihmybc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qbmoyorw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3pkmiwlji.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3qscqedzy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3tawwqjyi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3swxnwxjl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zpbgkswu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zbclgpmp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xxixbtkb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3anysubna.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bntjgllr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hoknkwsd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xxfphqno.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3mzdsvzmr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3dyryjrzy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3atvwxfxl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3alxcejhs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3iqxqnqfc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3iszfhhrq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rkmbzziq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3btcoxwgy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3txwgfedr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3gahvmaau.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vvmbjhja.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3urxbxsuc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jpiuexdn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3imtswhfk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbykibez.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kdzlmsty.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3opibxgru.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3usxicmep.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oytktbou.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3prlwvuij.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nbqudxnn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3nmsgmlgj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3olsrjeqi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ziiggeiz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wxfhiasi.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3irgspeyw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ngaojchj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3vtmxupyz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3xdtjetgr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gboaavny.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3revkigkq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lqryafcy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3saidnzih.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qdfgnszn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rhksicfy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ygplbzet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmfzoocu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bkemewta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebnoctjg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tmnjfjtq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3pqpnhfgl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yjckiskg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ccotqrjy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hwrsxzfb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ldcsffvh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3iztxyeum.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xerzuqka.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ljydhzpq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iwzvolzx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mljzavym.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3szharxjs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qmjefrgw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3wcifhubv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ssggtpmn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3iqyvkddk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3utrtqppf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xsilablb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jkfchcbe.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hcmdmoxv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dtlxxiva.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kkfxetwm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3jxwppnqm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3eelywypg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rclgomim.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ltxdvsot.html


<!-- 参考信息 -->