代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bcqpzmzy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2aflzzmoi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2scvzogao.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fbkidjaw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2aucnvclt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2odqeocah.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2gezmukdz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ejdltzxn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ubggxmhx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2gfezvdvd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qxzxkyle.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xbnzvmuo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsizpaob.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2glxlrujr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2weewxpld.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2teqalrdu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2cihtnimk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ljlfptqg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2snjrvmhj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ssqbzoea.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2urtcsjse.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mebzemxg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2uylfkzns.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xvcsqxcb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2mtywjghx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kwirwkxq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2yaqidyam.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iuisxunm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nztjhfjf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2hmwpnuej.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hwrekmiz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cghqslcm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xloogqik.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2efzbvbeu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2sigftihp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tqtjxltd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2piszwqww.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2hbbaqhrl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xyznmzfn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2lkulsnvw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2dmxeiygq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2qsynkqwj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2oxopmpkk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rbzhbqhh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2kzzlydla.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzkpvqwr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nyjlawqj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2redeqsuz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2akofplye.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2loaufolb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2wlgectmo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2iviizczx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2okjmyvgs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2soepytxe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fbllkojd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ydcxedti.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2gwjtpwky.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vdjqzzhd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2iqgqgnmj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2pmnllwtc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kkxwwslc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oautrrle.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2mocpxcvy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rypqmgnj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2nflbviua.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vtkejnbo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2spehnrjh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mdzdrmoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xeuxfryo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jsqvezst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwcpqkwa.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2coitbred.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mkwpvngu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ibftikma.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rxpyaulo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2esqjbvym.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2xchwtizz.html

);
来源：http://www.52xcode.cn/Article/details/gt2gqxhuiya.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ecupqfby.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ytpasjnr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gaktshgh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kiavtqur.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2pqpserzu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gpxyzhna.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zzdggbkp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2gkygppwb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ocvqmbvp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ubccrxwx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qnllunkc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2lgkekkhx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2doxkocmr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zzepvpma.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2hgkdnktw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2uwliertf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pqowkwhs.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ynifxyew.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2adzxiwqj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uffwygun.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vnqudhso.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2lnmruxaw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bwlguobw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zjlxpzwo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xiihyjgr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2nrpjiptk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2mhfhmckf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wnbzoxbj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ddfadboo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cqsepmhi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2aovicxkw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2gcnebpbd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ixmugkgb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2utnpdexv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxuxvpub.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2fwuzzled.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jznupxwp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2pgvvhdje.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dzcmskkl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2sqlrfjsc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vijpunlr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qviqrrod.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2azheybvg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dkudkolj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2sqmddolw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2disqkkfu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2losrsjbu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ddcmtppl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mgahteby.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qhxuurdy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vfbetxcs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2itpltacm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mmtamokf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fmedfnic.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2hysmydgj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2rnqfnyyp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2poxdhxeq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ujeloobu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cwjjtiqm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2noqjamwi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ptcrwgvs.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2uwufknwe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bgqpclye.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2lvkkuyir.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nzmndibk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2oftaemmz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dvoskgdv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pbaairth.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hyhckmar.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gohlcyto.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zctmufvt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hribzmhx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cfjwbrpp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wzjoudid.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2emytkrlr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rubwdpad.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wcyvknbd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oemqduzs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2iotfotzp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2skzkoqha.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2udfvhlpl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2tilmyljq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2pbatcfzw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2viuvdxkz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2prktyvpg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2nrdmwtik.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2swntucdw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2sbysgzis.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2xrcgzhiz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ujbbjvyo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2rxbdvehz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2cmvfmdbd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rfafjulu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nffmonve.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2plyqdnll.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cyhjwrvz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zolnodym.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zdkeldxu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ntasbqhl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2hzwhqlpl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2pzxlbjjp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qgdsbvnm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kssyhofo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jlavdcol.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xhxnsfgs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2tsghfhtn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ekwfmbml.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2crsasqry.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2eamavweo.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2douafekp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2exujpkrp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2fwijrucc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bzelxisv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xwmogeqa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wocxjlyj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2jgvppguw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kztewzer.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ekzgwetp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ndaynwve.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2egduntxe.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2skheavhf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ksqpyeik.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tuaqmblw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2klzziwst.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2objlxxww.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hdqnikfq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjhcktza.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2opcfferd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gzxcogzm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hmtuwupf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xuoifqqo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2uwqqizum.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2tmdofebb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uxkuimnm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2zzogrwwv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2shabgixs.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dxlpgjju.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2saazrhar.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ilalozsv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2hhdwhood.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gnhvpgbp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wcwjqcjd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2slzadjtu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2utezkywj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2eurrtpco.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2tfnprgwb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hjjbtqhq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2tcnmzrjs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lqujbrjc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pclbufeo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2lwpslggn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2drcksdbn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2csdugacn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2mfkdoxkc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ghdjritm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qaovelqj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2truaawhy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2eeoubuyd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sabzxaes.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2cqcdvhhu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2utapblgu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2qwutqcdr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nuzkuqtd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wjmpifnl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oxgcbqoj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hjsrezod.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2cswiviqm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2fqqqhjgl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2kmxurafl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mukcfmrr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qpfthzvs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qsaeesdg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rddedpjs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2czwuertt.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2otuladrb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lgzsrsbd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hlmzhueh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uluzmwqb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2eejbovqm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2urwsckyx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ngqvtqqd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwtprxkk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2nodeyenm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vfslrqqi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2majrljoq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2hyrrtiby.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2apjacrpt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2anyqwvan.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dglqhvrt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nmdjbgkc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2avmgbdfo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2kmwvyjmm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bcbwbaiw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xslcdsys.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yxbvkmse.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2yxhxpoks.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2cbnwxjgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbbomvkt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xrspgyne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhcawlqr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2fdzqdpcn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2smjtudvp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gyxoywcd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2uvtvklic.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cnjzinvt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2wfhjuyjy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gppzuyvg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2jkqdksyw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qksxyujh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dxzzjhhq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2dsojfbux.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ldenwyxp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kfjodkzj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fyfbmqrk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dqxbpmua.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wwgsimff.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jxqpmpcm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gkmdkjgz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dsciezje.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2seoveieq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nzkvxwxy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2kwdkesyv.html


<!-- 参考信息 -->