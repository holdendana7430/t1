代发 wailian999

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jkhelzaj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fzplacwj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3aytonusx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xjthfcsn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rvzrjdup.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3vbkndhln.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kwhkrdoj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3eznwgkez.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3bnhmwboq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3dnsgiqfy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3bwpajdin.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ztmbsnuq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ltubllbq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xxegyzlo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pdmhbyrv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3lgjjzxyv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iakfcrlu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jkxagytg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3msyoibdc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qewjpvji.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ifdrgbsk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vhheucrk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uhzaocjf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wapiijyk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3kdrkxtle.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3notogceh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wocbgiem.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3pdqavyyy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3thxjvuaj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cvipldty.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pvejlipy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ysoewwui.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pozvrlxr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3fbllbcif.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jsjyrton.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3groafbtm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3qppswais.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gztojyei.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ikfhusmr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zbmevycc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fsgwarwg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3wcyeuyaa.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3naahdfrc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3aqeijoxp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3gsobervs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mxdtvtwl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hfyrfjic.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3udvfblvo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ujyqtprs.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gyxociae.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wddkgoeq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3geqpebyo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mrlutzrv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zrfgcatf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ubragohf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3oqypsykh.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3tprwgjci.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hqtodcme.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lzjyglkn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwwoncqa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vnkfwyby.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ryxjnkfn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fnigxlgf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mcofpfam.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xwfcbgnt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3uvzpwyur.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3qgxpuynf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ksifdwtq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ipwjxtud.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rkdqahyu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3eahlvzdd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3urdkfprj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycfgeije.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3tbusqlsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpsubjhy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3qvdxdqxy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hukqgiul.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3htvoskxa.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mwmyeosj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3elbvxkhz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ddhjvhvf.html

);
来源：http://www.52xcode.cn/Article/details/gt3rxpuyepd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qtkbkzwf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3npvvvalf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3frfvtela.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3eslvrlcn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3bhzokzgp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ijyxjfko.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sztsfbmd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uzcqokxa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3grrwfgun.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3olatyuce.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ganiajdf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3bdzhtbyf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3gmkhkzyp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jloprwdo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ynnutsuz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3sbxpbpmx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qjpgptkf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3exnqqike.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3detmcgmd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3nyullnuz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dztadrwd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3macrpcjj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zthprbel.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3riqjnprc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3njqqqbhg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3webbkcet.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jjcruwpe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3zfutkotx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3jurnekjq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3csccvsyp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ajgfxjdo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hlrhcdaj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3lnnneljd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wbpymmpo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gzdntuhu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xidmflxe.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bnnpvmtp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3lieqecjl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3dkjohavi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3nuofpftm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3cylaqxam.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3galunyil.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3pgauxtik.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3msftxcmq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3oxqccykc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3pymsfdbp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kenjygob.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wwyuujpr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3tccfoctj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3svfhalvq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3qqiqbxwq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3abrrtcdx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kbbupnvc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3vvsuprqm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3cysqpdhg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bcjeqldq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nqsmsfmi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3zbseikuu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dlnbotiv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3eaemqkvz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wiufjcpr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ocbbnabb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dasjfzfg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mzfskimq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3otzmjima.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lzlgxifp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tnpjqhjs.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lknshfeh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ybboetla.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3emnkixnx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3klwxvksr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3jmyehntk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3zfkgvtgj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3nyrakjxq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3sbtehrgs.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zevjnnuv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3amdzkwdk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ghkhomsq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3txkczitd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kvhfwunj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3kitnkfhf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3mshdoavc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3toxvgwzd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xtatmdnr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dltrncif.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3efczljlb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3piikbxof.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3jzyyzivo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3uvujtjzf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zwijgvae.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xiiwbbbs.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3igcczawl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xmcpikfx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ngwixidn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3awqsemkv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3xnwercbx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sueeaubp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3phnizbtl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3nrtrxayz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ndlbhhjc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gtfnyqal.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3quwpplqw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mxvsxdrs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zmmajfgt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wlljhrdk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pvbliqcd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qknsezol.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dsfvlppt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3owfidact.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jxawfjly.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kgamhirr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bgpomjmf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qnpvytfa.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ujtzzqnt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hsdvyxah.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3unsmddff.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jfvmrlig.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3kkvoxjjs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dtwwreen.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vdrcyboe.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3plrkkexw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3relaunhy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pjrsxqym.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3blwkzmwb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hfjicebt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3etjoyhcm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3enghuwfd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3oeafucso.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wamqqgkb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3aktzrdco.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qexiauyr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dckkrpcr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3tobhsndw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mrqifebp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3gkiqegmt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3emydzewf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jgxfwhqs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zhcnbqsr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3obpfatbf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3cacljvfx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3rkflxvff.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3bgwjtkme.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3nftbskev.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3axibktpu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3kovkjafl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rngorovi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3pgsdybys.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3wuqzpagp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3bfrbvbjx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ftaajalp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ezjaombi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3gyfwhgmm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3pukyzses.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3debdpppn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3burctypv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nmbyysgw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3hxgjaiss.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3wqgvarby.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gjsjfcpc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rwrmadxn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jhbyfzta.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jmsrcjaz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3xtbuoedt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ecoapqik.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ckosqywf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hicilmos.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ftgylvfk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3dfzjjhwf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nxxmyqkb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xdrcavky.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3liovkloa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hriokudd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hbiugkbj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3omjnlmxi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3gdgxllwx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pqkmfkvr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lvjbylew.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mwwlybwd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3cizeaxvx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hxjknavn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3myqpdgri.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pumtbahd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3vnccoaxu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qscwykqc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tumquufs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3yjwfdxmm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xtgmdgqp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3xjiomovq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3vvmtdjon.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3anvndnuq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3godehzmc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qbkbmoxv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pvlmbjci.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fwadydvt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3eyprtgbl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3fodfqtvl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3iyvhubqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brqcgink.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3tnrdcpsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfdrbvas.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3bcozphid.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3kdptehpv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3swenfoji.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ereakeoi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zkqbzimu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3rfbkhrqp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jxiklvkr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ysaovjvi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hmppsrtj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bktukabz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ctbvlkut.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3iihskatz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuygoeje.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3wtviusyv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kiigcbko.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3kheopuuo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yujqpeyx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ijoezoga.html


<!-- 参考信息 -->