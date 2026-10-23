代发 wailian999

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3djdzhqgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apjdkghm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3omedjlxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlgynlnm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ifdmgkrm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3trjoxzgn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3fdtstaxh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yjmamuyj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vyriyghh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ffllkfwu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vwkkcatn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tatuabnd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tygpeoaw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pklmswyz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3hfxydfcr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ywuxkctv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vxpramrj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3qfqqsydd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3muxtaxxa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3cccplque.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whoxonsa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3zteuamoc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3kigqcfcn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3sgcytgqu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3deprbtbx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fvznegje.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dgyivdfq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3bkisbtxx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3skyfbldo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3smmwieen.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3amndbfye.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3rzhuapnl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3pkjhkbqk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nbqgkuho.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ctqlsoet.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tjdlzzda.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qbxspymv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xshbpgbi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3mjxzykjf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3biiofhnw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3tynvfrux.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ocxvgbiq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3vrfxvylm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qqxptvng.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qgkrtzon.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3fbgxqkkb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xnmnimst.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3imyyvark.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3nkqqsioe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ypfhysbx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3oftklqsk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvxmdsij.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3lvthoamr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gtmyaprd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3drjpupbl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3seabiics.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3bkmkavzb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ldposdxn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xnnfqnwi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kjepboko.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3lloehlje.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mxyueqdo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jqajqeyj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xhxcaumc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3aeqxdeya.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qjbevwus.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hzsiswzv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3cxegwtoo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3kzkdeizj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3afgiejza.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3emchqfxy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rznveebu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3grbkmiwf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3yyflkrhm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jopwfupc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zolbjbbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdghquvm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lhjghevn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qeufwhtj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3vcyxotcu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3yxswtyka.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3otvnyfmk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hjemtxrt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3mzmibxkj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ksrrtoja.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3eigzbaeo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wlpucuks.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3fikbxlpr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3kweiqmax.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zvlafknk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3crnozjxe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3jhlhhnrr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dfqjrlpe.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3rxzujrqx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gbpnrzfg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3fmrjkqrj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lmugizpk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3dyqdvcgv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3yebdqmpz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ixunsioc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3izrybsgn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ymsfpdtq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zfkfrgff.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3kydtvehr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3esssvclb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3xbcprany.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3btsdowlc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3pcbnqguf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hrirjuym.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3imlkyyyr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jjyyutdl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3oveexeoz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qjsfmwen.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gewsrxob.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3brftsafh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3omwgkejt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ebcclywb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3olmpfddg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qvzyyxwv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3flovwwft.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ocsqogcs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xyiixiqt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ysjqsbtj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3uobdfjet.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ujcwsjik.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sdtyneyn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3oicooyqr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3piypqekt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3aoexfget.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vcvvqncq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3igumqgdy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3juwaspay.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ksljqbgt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3wymkgoxd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qqnhrxgt.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wdbnwzzj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3cnccdniq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ckvcpfrx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oybzhyir.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3uctudslj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mgkrqzse.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3vrvzzkyu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qfsyhlnn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3azeyveqw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3offvotih.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3bojxdtlh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xjvbsozd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cmumgiuo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vhcpttwz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3dcjbtwju.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uzzqjgyg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ziuvbpfy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3kbuplyhq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ldrtagxb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vpurlsyc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3mjpofdzd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qemslpjf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qkrrrpwc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qlgmaidj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vppmbnvm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vssxmyfm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ajdcjibo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3wvdsavkg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wwckkbhd.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3uqvfzgss.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mwnoajlq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3bvjxwaiw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3uruppnsl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kacqeuat.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vqspemcz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3duappvnr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3cmekradu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3psgdxwya.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3kwmtvowl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ixnxrpcv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xywmrjee.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3oteyrrno.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3glglrkpy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rbrugnyw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3lmsxdzav.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mozylpyw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nscvvxng.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3hufihsto.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3yadqqggh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3brzhpldu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3vzqeltiw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3tezmjwyw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wrhgnpss.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3cvbklxok.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3eqyrluev.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3kkxvrxts.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3nebdwioa.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ptmckrnq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gfieaiuv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pcugcgan.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mhcykjed.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3itqcuqxg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dglabmif.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dzcxdlfy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3okoggclm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vvhfmvga.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ebielfnj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fqyxduiq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3bqytegxc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3txhwgaip.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3jqctpcwc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3jeyhrkhu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vdpinqrf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ifdctwri.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3uxmpjgva.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3onvegdjx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3iqzfzjke.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wphviinq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xjnopwnn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mvkbbfki.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ehovcura.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wjfwjwsp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3hntvcehq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3lewxtadm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gxxnpgmz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3xzhlqxrx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ywrggrsi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3zwnqfoxd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lyutohfj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3mqmpulap.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cppzuekk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tasvafcx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3lpmnchty.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3gtjyxttk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3imcjahov.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ogmwxnze.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3qmeaoaob.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3yozlkojf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hatmhdey.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3tthmakqw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3xobydvgn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ijbgcsir.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3yobhfwhj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dgcuefhh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3kwiqiwto.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xbhqxosq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dnvmtyye.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xfbmquml.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zmhwsfde.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jprgatwe.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jpshxzjl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3weouxfwi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3yudzobhz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3xrmvditr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yzetkshn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bkcqozkf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ldcwlvov.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3bibtfdqy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3czwvrivo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nriuazuk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3pnwgeurp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3axxbhomb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3jaffvcib.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xejqvktl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3svuoygbj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3zvxlgrll.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yiylxvxm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3otrdacsw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rqisadee.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kofafmlr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bfnwmvyv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mvdlwnty.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbsrxuwl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wrzqlooi.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lzphwvcg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3dwxjzzjd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3njnragil.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ftkosvxd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3syqewcwd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rqversut.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qzzbcrmo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3nsqrddpm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3tjebuxht.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fislrirf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3pdcyuvju.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3keqzsuzr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mdfhyhlk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jrvnfmyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akeefexa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3tpkpuzia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3psaglbkr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3yjeathan.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3pqkwqtry.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3npytscue.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dfuuogoe.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hshshijg.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3zfqdcqnn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3vseuaslu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ysdsbloc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bbofolpr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ctahsroo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mhjhuvtx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ekcvrxqz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bzplymro.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ubghxvmw.html


<!-- 参考信息 -->