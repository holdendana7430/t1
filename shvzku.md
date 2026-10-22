代发 wailian999

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qgnfvqjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlfnhbno.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2beknubkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nykoyujo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2flbsuvpo.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vlgwafzq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fylpyuwx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2whztxbdf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2saoxsqqt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2cfmkhfwg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2crvtlpbn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wdgpurku.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hvucbkof.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kalgxdty.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2deginthy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wmadtycz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qpydndml.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2zgcldtqj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qsuepzou.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2kuidridv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xotfntqr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2rgpclxmg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ssceilwu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2enpnazvz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2zuqfcpaw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vwhjbqjm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zmnpjxec.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2zqzrpkng.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2tgaqzoml.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ozppcrqg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2rjrmjxsr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2lktnocsk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2onckkawy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cbdjjttc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ufykdzsz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vqqbmtpb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jmfbcrtj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2socdpaoj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cekvzrpg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2manvyypk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2nptjlrkr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2cwkugygs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qhozyqht.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2amtfjnzg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2aubmelus.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ydktcnhz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xuulpokr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2xxdiykrc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2fmpbwgsl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hdijrgjf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2homgelwp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zzojrbva.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ikzcknra.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lppqyirt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mmpjxplp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ufwsnqfb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2nndhxque.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouwytjla.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2wamxjzkc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2sqvkfyoz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2mfuewvzi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rkggmpad.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hvbcklge.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2obsmxwnb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2zqxncdbt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2rijjbytr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2sydhtxed.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ytapabwf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ddjzqrgz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2sjzjewha.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2cexvnfyj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zosmybfv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2lxssotty.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2xwechzva.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gkyvncwj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2nlenktde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhcrvawx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ybjkayiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dunrsbrt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bddassqr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2elfxpigk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hjhpnyun.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2evssnipz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2facfpjog.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2relmulxo.html

);
来源：http://www.52xcode.cn/Article/details/gt2keyabnsi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2naxfyida.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2wmipncow.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lpywpgno.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jzozcacf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2spqjinoj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xrahnwtu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ppglihrs.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qlomkpfd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2fzmrpdzd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2znrqriln.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hdlyitze.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2bbqqgkqq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cyxzaznt.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pgbfjikq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xcwkkuxt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2fofcejke.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uxrcdszp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2lknobbbc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2iwdnjrpd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2aofdjwvf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hwjxecki.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vemsiwqh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2slggcncq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vwvxiuio.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kythmzou.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2igmlxbyr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ndfdqeop.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2jvailoik.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2mexnhvlc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pvkqnncx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ecmudqvq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ahmffsjd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2qblprwoo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xhjlyrjy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cgnvjrwc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vofflsrk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fikxctxy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jsrjqrum.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qakrnkjz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xjewovku.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2zjcbynll.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wkameszf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2tbdpiscx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jzyvytxj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xutvojuh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2zxyrftiz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2rmsbtupm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2lugubakw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2vhxmkaly.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2pstoemvm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2nrlqqzci.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2xucuqsen.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qdgqmjdc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2tnzidmpr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vrdfokyf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ynqjnlkn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vijoirjr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2adyvxbgj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vtdrfiqf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hixonodc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ihnerwuz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yunfqzvb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eabwhcnw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2yhrcgkjj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vuwedxtj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2brhmzcqx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cmfyzvzg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pjxkjjqc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xgxpubjx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2fuytanmo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ksemevrh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2tyuznbnt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2frweqtje.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2kolgebfk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2efsykhkc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tvcfunft.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2sbokiyfc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2evfpgpvw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2blueubvz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hpturtmt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2odiayqzt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xofqznqj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ycjjckwe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xrsnyrow.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pmsrmhkc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2maavtbra.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2prhefazi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2qzxkalsl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ehhlcavp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rcsbghqf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qifssoca.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ngtmkhuj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xekjrtvh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2bmntvoqu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cklskzaq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lygykbth.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jsmdrnil.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wmnxbhyj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2almaoagx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qylhblmb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ndsqgidl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ehxueiaz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2cnajrdah.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2anbftmuy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2aqrzwrlm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pampambw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xposhedb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2qtguurjd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mwrfkmgq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rmykifrs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2adcgjcfe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tqsddsna.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pusyffvj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2haiepflk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2nrxrgijl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wgazotaq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gdekubgm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2intomckq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wsubmfeh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fazoozfd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rtusacip.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2dngtexky.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hinhtrdc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2riyebpew.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rqbsxbwq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2lczeptrb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxqdvghp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2wlpyatmi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zkowuzye.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xsxkonhc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bbbeggls.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pcwekmjb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2pmheyriu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zxsdiefc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vtrpvqag.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mhqzkeoe.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2orgtnaqq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dtewjakw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2uclznckp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2cmcvmttx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2rndfdfbp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2rxouzolx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ztmxaytg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2dkpyijhh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2sgwnhdsz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tdguxrji.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2fvpmhbkk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pqxekkro.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2yzegwyeo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2gwolwiuw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dywbxnig.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2cpanerqn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zvytcvzw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2lgtleqbc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2djauylnf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2gupyksen.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2okwzzyji.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2fwdvcacy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vymhybbw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hdwnclnk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jsrdonxz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kesdxgsr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2tvknmkee.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bygaelqe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cmxzawnq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pyysxnsf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qhaihpke.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2arkwuehj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2sjzpzozd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2pqtqbxkv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rxvrwzrk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2uylghmzw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wdqvlqny.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gefivgpr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2tuigmqzm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jlxuivij.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2eksknyxa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lwfmjhfu.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2hrrvhpdq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fqiuzzob.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uyyokzmv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ozcacvnn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jjmtzhoy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rnvymvsp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2sffogctz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2kerkpnsk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2lclbfbst.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2htnpvztv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dmrdordp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2dygakpck.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ospdulos.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2odrlukbp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xtudccgl.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2hextcwwf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kndzdwao.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2sbubqiaf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2zpcezrrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwzfqulw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uwluevbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hepaduhl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2tvydkbjj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2nwrojgkl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hzqssuke.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2tmwabntt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qayjvgql.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2uodkfafo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2yzpngkhz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tlavtmxb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qxwpnltc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hqgkfvhc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ncvxgpjl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vvtannrq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdemnwpa.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2axxmnvnv.html


<!-- 参考信息 -->