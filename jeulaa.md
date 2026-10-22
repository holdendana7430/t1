代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2twfwrrrv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2otmisnxr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2mnqsnght.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rvahlzhn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fxzhjzhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aliwfwrf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2xbqipqrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugqbchrm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2buljixcu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2kueiqjcl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pkmpplci.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2alrobeia.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ohwshrdv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2fvlqlyqb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ujneuhwj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fwfxdnpd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jukynteq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ufaumusz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qeurcuwb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwxbpfyn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ahkrandf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2sjwwdkog.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tmtyznts.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2odwpfbrq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2snjflhfu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2cvrfcjow.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yoioprux.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hjqsierm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2imowmtyc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bwldzszg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ervhitol.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cdnzjqxp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bizbstty.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2kekxduan.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2klmruhoi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2igofukbe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2aeejyosy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qlgnbhle.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cjwjkouv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ogsxcfni.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2whxafxsr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gyrqaeno.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2akjhlqag.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dkourqiv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rigroghx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2lqxwddyx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jukjtvth.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2uyvvdkkw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gqavfqlm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2czdfgqae.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lnvrnive.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2srqykrfl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2rwgplqgl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2cwlvmxsq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kguziduq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hztjveni.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xgbjcruf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzsxkoht.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wjqqpedf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxqfimyg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cbbegzeu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2uulupsyz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2uaegogcx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2stypngmv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2milukftz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dgjjjlwu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hmhmybqm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2txwriezo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2loyuggxz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ohdczncx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2plzgojug.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ykndeauo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2yesupjzn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ydhpfeab.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2qtkndzrm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ymkckcqi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2gisuiqmf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zgjwgbsf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ajcvyhak.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2pxxfyipw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwablcdm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2uznwcgbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djnzptpe.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2elazlakq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xcaaxslz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2czpzuwys.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gvfhgmuh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2rifrimdu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2beprgqrd.html

);
来源：http://www.52xcode.cn/Article/details/gt2jhquebel.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ravtdbwb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2rogzqbrw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nxbmtmpp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2umdfgbcb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2rwqguaun.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ztuaybng.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nepisfdr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2kchlctjf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pyydpjbj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2wutmmnim.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cijrfmxa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2balrfaxg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cwaxoqou.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zlehvyzf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ivzswovi.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2fhkrcmfm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dcemwtkq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2pmujdziy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rrvrjwfo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ardrsgrl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yyzhpdaz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2xttreaxr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zkuglkqj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2zauhvwlm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hkowzgmg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2gnzedbtu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ccjwkwnb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2euvlrsmh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jxfteerp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xwspgtkg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vzxwxegi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2dyaziltb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ashppfuj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vwlelqsc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zkhycwoi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zwkbsaqg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zmvnbryc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2drrkhswz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cxaxqnkx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2lnxbvdyd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qsocuqjo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rgmvnjjb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xxcepoch.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fsrrptth.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gbrkfghr.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fhptjehg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2harnmjpv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2puteptrn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nivusqdf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2wwwahvcu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2pmaoxqey.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ofwdnjqm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jljvslvf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2acbgveod.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2axuqlfhh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mfgamedh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qetapvce.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2dhhwrjuf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2skesbuqu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jmwihhvr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zdtlahhh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rtrzokul.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ukefhvyt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xtkznddn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ovecaeqg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2cdlxuntb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2omdetten.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aqoipvau.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sbsbqgln.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qtwjfpaa.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2asmxhhsj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2huvylqvk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vncklomb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fyrpfnop.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ncjiluen.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2reomlvie.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dnketymq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2chmpasfo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zfbwneic.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bpeweloj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2yvwfboht.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2szawbxkl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2mjrabvob.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2otbnmzsx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2osnhkvvh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2otiyteyw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2sfukjzlf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2inbyfpdv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zkekzaph.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tvzmqzfk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2rwxhoeii.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hcpgxxcv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mqbrusha.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2hnrpsfbp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2iokewkpf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kfhmksfi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jtbfhadk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2edkqjqyh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ytxybaen.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2mhorwspk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2sqwmcdau.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gwqzdapm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tmiyhkad.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ofzbdzkg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zjuhzmwb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2tdmblbut.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gvhbyqqy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2vhdbhktf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2lavnwuow.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rviwjmeh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tefwwjda.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qbxrgzoj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lplvauru.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2exuddrxk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zewrkqaf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xyowxmzg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rfjxmdpm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2iqwymnau.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2tbsrvykn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2oymnsboi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lnvojodt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2mjpybepb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jfjbcbvx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ghyawdet.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mgfsmjei.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kymtlzll.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gnrspwav.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bdvrfgxb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cvkybbkc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2voddvypq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2treiajcu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jihawsrj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2lewivcoh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wqrifybo.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2fphcueuv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lsdmawjl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2sjvyexeb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2demyiyft.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pvtisrex.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2qnkbbwba.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2cxtnlhtk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vqnhojpd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2qhgvmsvu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2sawolsve.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cblfteks.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2curvwfnq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dvoawuax.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ewrdexqc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2twwflcuk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dgsuydjq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2tdsqmmzl.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2quraglkc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2pkedypqa.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vzezfotu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2edvvtaej.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ljfoixtd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tehruiem.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rczxavgw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ouefuafl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2qtdyjqgg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xkfspkxu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2izlpnjun.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2vwtcqnio.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fewuqjki.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nmjrjjdd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ghlvcdfu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2mrgofmqb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2nxtdkaws.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2wfsejusb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2askynxkl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2eirhldbl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2fsmqmgbu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hfzduxka.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2wzanlujq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2usuzfxnn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nchxhgfx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zpdjzank.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kcytcikr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ftnmytvl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gscshncl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ehzifprv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2awxjophn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2oqnzxjwt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kmelsurc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hjxoqcze.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jhhsbwgc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ylrpbcdc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2oeoprtws.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2relidiab.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pndgcgku.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tkmrtjim.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ivwdsotv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iamcglvz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2mqnpywqt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2vwnphjct.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2lxogwnui.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2uqukjonx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iramtyhr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2uiwvlrwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yspajypr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hdqajgjw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mhpzbssb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2cqprssti.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2hcdzqwwq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ytuhmutg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jsgfvuwf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2leoxmnce.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vivmhvkv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2fgbhqcmx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2biijvxzt.html


<!-- 参考信息 -->