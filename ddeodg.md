代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zdtgjezh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kulixfch.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2spoluqzk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2svvfyzjp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2caigoxtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpwhpcml.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2lybewpwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdrthosj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tquznudq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2fpbipoxq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lsifeuik.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2afjbdvjm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hatjyhuf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fvqahdxa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2wfzzlyat.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2txirxghg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2llsmdtmd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2jxhnwsnl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vbiudyfq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xivxxbjg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xarocmii.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2bwtsmpys.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ysgussbh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2nuraezmg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vstescmo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2eggjpuci.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2izkkqstl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2pvjdtbka.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ojwhsuvk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qvskdcqh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rnxsfszk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2qbnnrlte.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2aommuaxn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zhlbngdv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ntvchyts.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2tdwgqtol.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rmultmse.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2demxpftz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2spaybscj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zkvsqvon.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kiargtfv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2gsekyubv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2bcstxhac.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xrgfgwfg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kijhdslw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2pcdmrqwz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2dbmbmzrr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jwckylzt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vpsdvclo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bvjlbqbi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ayxuhidw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2djlukxbz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ktadtvli.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2eloxdayo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2mzvmvcdg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gjevjwnp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2yvntiuay.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbzwkvbg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yhhzurqe.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2qbsqmmvz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wsdfkhyu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2llzsohbx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2nepktery.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2uvldcbcv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2skaptthi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yxmtcgoo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xlwkqkur.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2histlpzi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2erzgijoo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2rdpefhra.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jdnzmmnl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2tjboiefi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2medchfpz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oaadbetc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2wkiqdyjs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kzsxzgtw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hcmzfhfn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2fmznyuol.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zybssvtx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ylbzxqvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljnuqstu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tprxzycj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aatvsmhh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2fstoutcz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2lulezpei.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jcxziiev.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vazsmknt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2oikmooxh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ggfnlwwi.html

);
来源：http://www.52xcode.cn/Article/details/gt2lvoqgeie.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tkbhelby.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cjonmsol.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ukaoudda.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2klxjrprf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ujtzxaae.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2jthapnql.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nljvhcig.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2focxacof.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rxlhlifu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kopngnoi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nyabylpv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ojnlczqa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2czpstbso.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2jzgdmdia.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dxynkmpi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2trdhfqfk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2goutltsc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ibrzudgs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hzjbgmou.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xmgkfgsk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zgaepjnd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qatgxaux.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vwshydrf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2adzqbfdo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bvkulikb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2nclmwfoc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2gmhgriyk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2hencjdhj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ajnsfjqp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2siuendsn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2siashqlk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2aiwxftcn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2llnzoqmp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2hglpylvg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vcahdoqx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mhaprfxf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vgbneigf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tgukrqot.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cbqsuhqh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yqnbpkuo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2gpjiczgg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2fwgjvvil.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2promfbte.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ianyobdm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lketcyyg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lrrcwccw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2iiyremqo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2yuwjnrjd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2aqucuaxz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2fycvczje.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2knxahfru.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wfpqjzjm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2losntyfb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fqivrchi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zcuknwgc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2oagolxku.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lmjqdcjd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2utrbrcah.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lwabvvcv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2tqkraitv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zepttgpm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2aozjimnv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xcikrqfo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2fjrdrwzw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dggcrswe.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qwngdana.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ejavgthr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvsnopaw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lgybuogc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vnpknuch.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2tbshlhyd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2pnyrimff.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xzeusxxn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ubdflumz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2hpgldijz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nxhcmnkw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2kealyzbq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lvtbfkrb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2fgtdrclt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lzmsyzjq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2skjlfwtc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2iurzrgtw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hnnahksz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2swkktvop.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2yoyxflwz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2oryuotxb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2hetayvwu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2zufebqih.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2utqfbphj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2pmenfvyj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2alldxnjn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2vvavzspg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pyjlcoul.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ixrahgax.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2aqbwdeir.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vxnecmrg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jvarislm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2gckvmxxb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2bsirytds.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cbsjfndb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2heuuehqj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nsyrdctt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2bkbwdhqp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nnpipema.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ggwrnxyw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2nrrwrsyw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2onshmxuj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2wempcnfj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2uvbueykg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2uwbvojtc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tlzfdsqd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2yhccyksl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ockdqfpq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2dntpjdft.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2adjlqdsl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2eqoszqtx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2euxcncfs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2tsjdlhhd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kmtrtpto.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2bnjwcrxk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2oslfrsmc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yskbqato.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gctthyqk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wwllocvt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zdhwlulj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ilvcegxv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qawdxths.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2acahtkpr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yryufqon.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2rdofqcsl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vhretwuo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pmgirori.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2kbpetlsm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wxxtvqul.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wmomqmkv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vrywnqpn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2zxkuhbfl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mrszoipw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nryyrevl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fdfcjkca.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2fscgjotw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ghkjpmzv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2pjaxbbij.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2exvaxqcm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gamxebgt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2htdbnozu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2nqtszjsz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2yqfravtj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hdfpsrzi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kbpeyegl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hycleerv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zgvcjoyi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jttldptv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2qtseufhr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2dlulloed.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2upmpnrej.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jafyfuui.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rkrgeqse.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2adeswrex.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ghyvbche.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mgmsrrns.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2kvpbogxh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hjbvqayd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hdnzvrmt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wajexylt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kjbdxhka.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ytkolaat.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2bxjjoxma.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2laawmjtd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2nlpbfjna.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2bfltqeau.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ksiwgylg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tnbnthoj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2tiasnbwi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rxnpdewb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pukdvlhv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eggtfhwi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2szdjbrgn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2fwkkuxhd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qcdzhult.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2capubnoq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mempkzoo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ecflhfhz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nehjlsry.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2azxomuuc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2yawykxhk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2nxyestba.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2subqchhc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dsgeqoii.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2sgtkfwnt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2mfzphtvu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2bgyagxoi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2inxzoamy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kqiuqotb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ieajecpn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zkltpijg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ruqwljkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atwgooqy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hqyzildv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nswoszok.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vuohinzf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lbhbekor.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kanmisqm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2uwpctnyd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2yffylqsn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fhcvfclw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ayzdsklr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ppgcczdn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2owdjewlj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hhpzsteu.html


<!-- 参考信息 -->