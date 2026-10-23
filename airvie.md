代发 wailian999

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3coquvyqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3suegsgcj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3twrgdsov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlpesdea.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vdhoqjci.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3xwubbqjp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bavgbmxw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3esmzpqmx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zkxidmhh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3gbjyhhnc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vhajdcso.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bknbkdbf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3uxlboeqm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jjgwyhbl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3cyjesqsc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3njilemdo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jumcjryu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3nrqoljko.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qlwqjeyv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zhwpwfde.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzuhphcc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hvttmjml.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lcdgidwm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3bjcwldvr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3mermogec.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nxmdzkba.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3iglcxhom.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gdokubwe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3olifpswy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ijykhxdo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ywobgmkc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3plmatjeb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rmrxlvsi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zvqkccgb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bncelnjm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ixruvlcb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fijimtbt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hniomrkq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3dnwupxob.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eblnwjou.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3kofatydc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3suwibjue.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3zqjnidar.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3cwtsyzpx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tqrzjnxa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3bdwzkjfw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qhglvort.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3zozwjjgx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qqymdvkm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3nwkrjrst.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ytscsqmc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3futithzt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3xrhxodvc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvwiswzw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxfndasj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjxaxwod.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3srgqhuxn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3diugzpxa.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vcxipdjp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ajnklygb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3asnzfmyn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qnzaesmo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zvbrlgjt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zemofilz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hhuqotgu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3leybjnda.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3eudousak.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zdzaagyb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3eurnyxlh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zhcvqxie.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vealqhlq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gsnpwtsa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3janesxrm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ztaroryt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3fnxhfzts.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3qfsnfcin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyqsbtua.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3xyfhmeso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhsvueiu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3aeseqled.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3nxortgbc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jzhwcwxm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nfzrzkmh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3editpwaz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wstaukso.html

);
来源：http://www.52xcode.cn/Article/details/gt3tglwgebs.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3tgrnrvbp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3sapfphpj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wwmftltw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3caiksuot.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3cgjqkugy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3niebfsgp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lpdtyjmf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3clkhrjsn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xinerxeo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3cdsgbvyx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dgyifqcc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3cmacsmye.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lzvylbrs.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zvduocoh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cfsqiewa.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vqjxwdrl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wwainiei.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vzohxozt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3adsniqsf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3fljwjiht.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hvniprzy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mpellvib.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3antpoxpu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3kwfevjri.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3elgdbbcl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3listbsjo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3vpmaikxn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gnntjqpf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3bmuvwhkv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dpwypdfr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ajwzwjxh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3pdqekjrw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3revwitnt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3unxkcdku.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yvvqhirs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ifflwfpc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vdjtnyyg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ktkcivkn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ilgvfynb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3urjjiijw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3gekzzejd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3nvelrgkl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3baxsskrm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3doajuxfp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dplzwmzi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3vcglxalg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3fhvaxqgl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3rhyhqlre.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3yswilpfd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3szxavret.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3swvppdrf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gmkkqkcf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3incenhfm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3uxdifyfz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3iipedezk.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3wcirunhn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3reledkgg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3bcjtakey.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3khdgfgcu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3nrfigety.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3avfngnze.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3oxfhnaui.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bbukjwgx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3tjzldoqi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3trvoleot.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yeifkvfi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3fqjuywwx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cddyjbeg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ywkvurzw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vwxkhlyq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3reflvhjp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qjthsiov.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3nuwoswer.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3aweiptma.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3rygypllb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vgeqqkae.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3cmyatlpz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lxmsiyty.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jrnogqpu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3szahtrcw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3gsfizksi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pamzyrln.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3kmommebw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ragikcab.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ycjbrudq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xyjjvneh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ztwsttqo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fwzgcvxj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3timbybyq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jpzeaims.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hdtjdsrd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vaswuswl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3yidrfafd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3weubdmar.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3faqsqjrh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3oxgrvhuo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zydfybtb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3gtsjpcmx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3jsllhhsq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3dotibipt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ccyuyzcp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3epxjzgsw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3usaznvrx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3axepppsm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zmqfnbgx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jtwiiavu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hgjqagqb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3caszkblf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yrmqahyn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3sfiaqwdw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xcduzuhx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ecjftcwn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xpzmxygr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3tbmnuebe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mzmxdwsr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3zhdqtksa.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3koyjmjva.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3qfqnalxo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ukosjkse.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3pukahuxs.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3iluatcji.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3imqgabvt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sxownmyk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3adlxftdb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3eswfgfbe.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3nyteotjj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iwutvatm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3juucmejl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fnpmewxs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3rznwbdny.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jajwqigl.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3omvssqpe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3dwboslmq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fbdaaqmn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sorqmijy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tlssokfl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vybjrtdx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rolcyjwo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3pgomxxby.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yxgrcosw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pdrfkuct.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3kfzzxyfv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3twcvlasl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3kaxlzrsz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3aayaqxxc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3aftptdvs.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3aiaxtkpz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ubhengbv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3iqxfgdxk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lspvzjbt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3isqsmsrk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3kwnmvohq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3iblplbfs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kcudyqep.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3coxlxbuk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3gkoufqbl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rptctclt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ptgxllmd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vlqpbcvb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3kecqdfcq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3brtdjflf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ppvjrkzb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3baopnrxe.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nrenudcw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cafpyjyt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3xccrlxjl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3pyllniga.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3tzzptvbm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nifpiaxz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ozchnhba.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3emrzxias.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3eymjggjj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mqxddsqn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3cfdrajdz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kimyqfnw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oprpwvfr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bhhzdkfi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bknkcvfd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3kdnkybhh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hsngtofj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fddtblrc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3myiglgzd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zzokmfzl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vaczgpnv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3yyquhmao.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3jalniuxf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3gskwmhrk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3hgxchqaf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ecpjmtid.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3mwtifbvz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3nljdknsg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3tjarqowk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cbzhdynf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bxtcmjqv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3kcgilhjh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3kdvlhrbb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qclnvlqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqfugjfk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3oubayumr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtxlcqdg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3noiagrbp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3evmcyzep.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3cwiozxdr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vlkxetjh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3pokztggj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3noewjfop.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wrwfelib.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3nsymqneh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zkjpsiyw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ykcfkkos.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3uuwskypf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wrndejix.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yanwljtt.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xppgqmhn.html


<!-- 参考信息 -->