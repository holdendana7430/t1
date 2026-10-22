代发 wailian999

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2itdugbpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npgkzfnu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2lvtyseht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jeeyxnoj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rxmrwwdf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gdxggadj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mmmxvnjx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eujutglz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wqsdazog.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2saedbanu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2twvqilht.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dctkrsow.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2gcdlxcgz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2egvqknyq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2youexyqa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dtecjmqu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lczpmzfz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2venjmbsv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2sjipgiaf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2arhniecw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejulzyfv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zeqgvdne.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2tbxhtzfa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2capzslch.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xkdhifdu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jputswzk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xpigkhot.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vjpckxib.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pmzppcbc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2luspotpf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2qmqkivml.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2baavbkpf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wteecpnx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rsmqiwph.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dqsxbqmh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2eakhktpf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ashmygjz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2btiqqkyq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2rzrbfejg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yuetxklj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2wyrqdhsl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2tldfumuf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2erpumuef.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zvrbhdsh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mfvuornd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2krvfdmub.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nulqmwqq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2yqgvseus.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2jkwsntvc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2nddxjciy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vhpuwnyg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dxinbuhx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2btdlwtue.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2snzwrvht.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jkhqvddz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkqtxbkg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2pvxjmvfz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvbpzief.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nznnkecc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2waqrexdr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2cauzpokl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ijvvpdqq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bgzrnbmn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2akiqofje.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2mvpjtvli.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2omsmohra.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2zexpicov.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qonaokpy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2dsxenmwe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2fnndgpcj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ihkxgwph.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2owqftpnm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vsuvflez.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2nomrnuho.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2tfbwxcla.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ntqmdhnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqlimrde.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nbmmwvpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmeroohz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2warzpjpt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2pbkrilpo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2geopuqbs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ersixbns.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2sjgippad.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2snbuqtfy.html

);
来源：http://www.52xcode.cn/Article/details/gt2ghcnfljz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mspxfite.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gmyqszuz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2menuncck.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uzejqtui.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vujnjswr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2yahmsdhb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xbzhlpde.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2fvlssetr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ggnfziyq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2nrvhctny.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2jraipijg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2iypkrgnv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ifdxfpbc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2foiqwsqr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2vcwsnxih.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2nfxfkqvh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eyoenhsl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2pfdqzwkl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2usspblxs.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2fjyyatet.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wrljqgps.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2fbwjwrym.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2twhxikfa.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jrbapqvr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2loguyswx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rfqkkawo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2atirfdrm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2asvavceg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zthbirjh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2onxdwone.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2viptarhh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2kvhwpajo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2pqqqsgoy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ldbvkfyq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2auddpwft.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2sclpagrq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dxgsvzaz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2akqxkhcw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jekwbqur.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mxnvywqq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2chxpasah.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2dbiornza.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bwnzhjjn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lrjanilu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qjocgxlq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jppvgfha.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ojasxsst.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2mnwhzyrx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ewskjxxk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wgugklli.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2eqqrorrp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nsqoqtka.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hbdyoodc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mqsrajgy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fpgyumfk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2unwwwbql.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ygcqxafc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2zmjkafky.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ycujsybn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ixtobikn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fngruuzv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tefsdsby.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vazoxmja.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rjexucir.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fwgbkrhr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xvrbtpab.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mcbjxbwu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qeqttwzf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cpixewmt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vhytzmpo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tsppaqgj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ghwmtksw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qttyiqwj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2byeothyd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rslqbsgg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2krydgrei.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2gbidyvxd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fmodjurb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2htgnyfcp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kmmaedlb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2eonkeqyd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rpbjzymo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2mhfyzahk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2riktcutt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2sarsunez.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2texeqnyn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cxjnboqn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bjydxigo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2htaxixje.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2glwefwfq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2dcrlcqad.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2etiorpao.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ixnlasbu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tqydzksz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ucxhalvz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cximspfl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2wxluqgww.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2segenauf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lbjdwszg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2izuknzhe.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2udbcbzxu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bfpvmade.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2panuohcx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lgrdtnsd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2upaumjve.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2exbfvldf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sfwcqczc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ivyyorfi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2jkjqkmzy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2odborwja.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dlffaiuv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2zuawwciq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kblncvwy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2glljkdbm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ihabrdom.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qzqgboau.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2frabmtpw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gcjnyxjb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nuusnjxb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ytrfcjgt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2pdvtukqm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jfsxsdtk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2orurviaz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2icotselq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lmblcuhu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2smsvrnmk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rgucslgj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vslstpzv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rtuwnxxe.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ikemayjp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yquxcmji.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2asgpmrpc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2juutaddn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gmjswnmh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2hkoxziqh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wjehshab.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2cyjvoofu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nxobtfwr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2butmypwy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2vuwsxfiy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2wdnjrkll.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2nectrnbb.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xlrwwixd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2clzguzpj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2udcscybo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ugwbnzdq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zckqlinb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2weebocyr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2igmczrjm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qcqtagvs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zcbgxavk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qcbxwnff.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2dpduigck.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2phwbwync.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2okwpuovl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qcnnctsu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2wcyldfvt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wvpxrrng.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eidbvvpw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2jcnhgpjj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lknhvorf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xsfrcdpt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2vychkpox.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ofsumxif.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xtjhnsuk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vqdputgj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2guedadaz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2idptmbfe.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2aqimfpcd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2xlkjeyyw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2zodhvcey.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2pyqnskdc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rjvjulbp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2sfbmxtgm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2msaaavvv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dvufpbdp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jalyetdt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lwynfypj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2qymxbksu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qympmyhi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rjowaaqn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pqugkxpd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qilxiwpp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fhdmszua.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bsdgibho.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2bzdexwog.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2aqkztdej.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rmhuskog.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2kiothibf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rpvxkydj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ayadvcoj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ahivfsmc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2seftetbb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ygikooyi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2biyuojhp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2trbflfsf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2adlwxpaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqtgzfgb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wenvzvhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sclmlxue.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mjdtljyd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2eopxjtgo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xyxcwjtb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jgeotbrj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zjwawirn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2svoifvem.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wrmevxmp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2sjurclxe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2dgbtijxm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2sunsrpvd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ymeztpqy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nmtasuss.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2waysgxxi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gkfqfeqm.html


<!-- 参考信息 -->