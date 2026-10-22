代发 wailian999

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jrkxlfaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evwddkgv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jigcguka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcmrelbu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2yntwnzmx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vfdcrvxu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xlmfyxtd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2oewuptyd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zulxeqer.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2gmnxywod.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2aynngmmn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2eamuohqb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fapccxgc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2evkgvdgc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ohcqwesw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jtaqwqgk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2htiiijff.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2uujkzdis.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nzxkvazv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2moauecmm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hbcrzjox.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ijcybkgb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kwhmwkpe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ttdhtsoe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2jumwzuxf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tjcuzvil.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2calbtask.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ecwflluu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2orajngqc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wicffnhx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dzmgxxju.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2wkxvgutc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fusmutem.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2arvuxyqr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xoqsqzpl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2paoujjim.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zjodefeo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lqinfloc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2faqqupfu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ygwuvqle.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ionhkysp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2jlmatuhh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ddqqsedk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ludauhdi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fztrhmkb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mmthvdni.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gmuydlsw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2oyrytaxt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zdtvngiv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2mvbkmxus.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2eaiuvcuk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbkpmjnh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vuxegzhm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wawsggbg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iksykbgw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuhuougp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ewenhiyd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2lrhuryfn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jccegzoa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2hiiarivj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xbkziexc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ajlvqrrq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xgeucwml.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2baspqqlh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2cwlkrpyz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vciwfggo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2vumjazxq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2rweccmpw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2uqlegksj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2jkzcithv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2swbsvfun.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tkgmgaxo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2cklsylsk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hzxalmca.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mrmqisjj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2abkykvuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orfaewvz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qdhlbpwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yystiejz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2mxgfqggk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2fzlyfmrq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nzyoxhev.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qldfwsst.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2cdvnozoa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jocucono.html

);
来源：http://www.52xcode.cn/Article/details/gt2lsahxips.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2xwhfmzzu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cedajgle.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qhgemdbm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2sdimdobg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2qhspqfvw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hjcnfvgb.html

);
来源：http://www.52xcode.cn/Article/details/gt2zjlyqmhx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2tdzddvmm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zfpzdlan.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wfybdpls.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2llcpwbba.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ydfkuagh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2iruspnuw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2drgyimgj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2urhexpwe.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mjgjjhlk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gdxvqqgw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2wkgmappr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2khmfeyao.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2znnpafez.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kaalqwng.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2smxgswqj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hxumfxrf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2lwmolpgk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ffsmcevf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2htsywsmm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ovzecqgi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wyssfrfk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bosaucva.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tbfguwzq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2tefzofad.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2brnrngrt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dbdtywwl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2iolpwbfx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zonacyww.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2iwmlpigo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2afxxykvi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ifbkolvk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2anoqdmge.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tyxqxhsy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2chjayynn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hgbrwjky.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2pxxglchd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fiztnehd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2wwpnztba.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2dezeqkzb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zfazomre.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2iiymlriq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2obsexipo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tfzsgllg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2gpdzfpju.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ddibqwzo.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dcntganf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2nwemrqss.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2hqryjkkz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2dxyfjayq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kqlthmfz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2zznrwkch.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dgpmdaxt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dunlesqz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jwfqrstp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2erqnzyiz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2khxmsqls.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2dqpjhvsh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xboqlncu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2vawndwfo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2svotsids.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vgpxtbzl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nfwlbdah.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xllibkvu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wnwtnscv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ljbznmhb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cxywntuk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qcqylrpe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gcbkeqgv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ncfaxqtp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ihdrorvm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2npwzsuvs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2nvfgvjtb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zgpjybnf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2uqyuozph.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ipgqxkkm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ucjpgjij.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2osijmwrf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2wurtwrmt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2stdsnrem.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wzsozwpj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pxaflmvc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zdyaxmer.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2koepljaj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2retjpmlv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2fyfxvuvw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2lerdfeeq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2idycgdys.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hsvqrsoy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mvushhnp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2aivlngyi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2drypgpwz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2gjkgyjsj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2bnzxzfkw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ncnifmev.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xoawknld.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2uzbdpccg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xxktrbpy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kbfxzeez.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2odsxcfwp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2nogopxxv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nacogihj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2zhltfmwp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2cipevclv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vxgmxcke.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2bvthenri.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2aikqxjyy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2phrbtszy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qzqtfiaq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mhmvzpbq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ehhedblq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gwumatgy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2frrfadna.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wmlpzlxg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zjemhcqa.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2gqhjzhcj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sjjxbrsj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xbgpkihu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kybnzokd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ywfjpajj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nrgpiowm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2wxauqusx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rdwehxqt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2spybecju.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cepxuktr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jjxdpdaw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2lwzmpqau.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vcxtmtqm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xjackkul.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2njxdrdno.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2fmogqipm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2eblfhcrj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2sjnjazkx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2cazopfmn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zbuipnla.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wfbguqtz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ijjvjhqe.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2plhorqxf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ebpuouhh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2qjpwjhnn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hajdcmpb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2egpiqmxw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2cqjofdua.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2snyhgqss.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gtkbuufo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2aeslcehn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ydgkxydj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ovjnzvms.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2pcrikfjj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ssqrkekz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2gguuaabh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2dexwcxiq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yolfhwfz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tgwghupv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2cuqahieh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kbpvrhme.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zkgclymr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2skvbkcts.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xsqiswdm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2wtvqjeyw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lbnrqjcq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2njkoejxi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ziogvaua.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2awmhaquu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2msfwdchr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2algwaukr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2urrvhlqv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2fesaaiyp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rlzffyzr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cyqthxfx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gedafjdc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ouuqgkfp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2kdkmxkik.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bupfweke.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zkgguuea.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2raxysyrl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2lrehenro.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rmegxcuo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2igbwkkbk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2bmbymcts.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xfkmemno.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2eutoullk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2seczgmuz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2mcsalhmu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hzmxaeog.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2noeoqkua.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ytwuxxlv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cafnpzil.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uiewlbzb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wjzasmgw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tfbpeyfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvcqfwbu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ikkyiizh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygprdlej.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2cddfoaqr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2rcramtzh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xkzuuwfk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lzltssbc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2lzqlwhgp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2lybnghen.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ombofccm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ybyriwbj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jsjbctvn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pqtmvvaa.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2tyecanww.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kiydyntr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uyrvpxbj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2svivzsec.html


<!-- 参考信息 -->