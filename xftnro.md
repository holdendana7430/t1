代发 wailian999

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2zflwtxsm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nbrvmizq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2gxotkxoz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fkivrtoe.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2taympmqi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dqtsexow.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jqclmwqa.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2appildvs.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jnawngbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuwglzix.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ykdnmcsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdlzmdlp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cfqkesgj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2aylhzfwk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dpceexev.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ffbrhtce.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2seufchvn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2nrdzafab.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2oqtwcncs.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2czqjdolh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jrdcehhq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2flplvzyg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2yhpumyxc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tfimkcii.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2bwstilkh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nmsypbme.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mybwrodi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2vkayramn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2cfejqgkc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hazwekbg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mvutlvkq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2hoowaqxe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2gjatmmzf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2navcncix.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cxcnongx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2qfrkdfcm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2rsolpspz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nxkoixtk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zqwwvngx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2oinspnuv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2vofijdfx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2erexgagd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ppdvdykx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gedptrfl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dccwdmwt.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nmeaipsl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2sjmvvfoy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yjdqodkn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2nqazkjyd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2onvgiafu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jpmoczud.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2liuqxqfd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2crzaumma.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2lxeufldi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2usffclms.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ahbfojrd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2mxgwzxjo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2eldpyqer.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mgscqtma.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wavvxhle.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2degezmrw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2utqouugo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2agzxnhsf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nttlhjbg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2rbsqpvxq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2osoinbfq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2phryreoo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2vtuhbieq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vzykjfgo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2czefffry.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2efyqsxoa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gktajugv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2rhrzbrhs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2aftjclmu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jmclyjqp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2nnswaetm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2fwtgbcmw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vfvmtysh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ecwnbnly.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mevquzzy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2rjfsswcz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2lycpfeoc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gfgfatog.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jpggtknr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frgwznpu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tccudjgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccvgnvnv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2zigowkvg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qwlrpkae.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2oieizsln.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2txrmiqlw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zlmogehu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wotmnwoh.html

);
来源：http://www.52xcode.cn/Article/details/gt2pcphtkfd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2lldeficr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2skjbjgrk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2cxolgzws.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tnnphczj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2qreonprb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2auomrqms.html

);
来源：http://www.52xcode.cn/Article/details/gt2tqqiwthr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jpaognvb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jsustmuj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2devkedoi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2darwiusl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ggjkfuuu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cafmocko.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xvgiqkja.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2rxadxyop.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2szphsbdt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mlmaegep.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xepxpblj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mncknpar.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vsuwjccc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ruzpqvju.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qwiqjmxj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hszbouvk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2lxwqzhin.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tvgaaods.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2fmyaegbq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vzajbuev.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2uwcfrejk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xrjihelm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2aennbyqj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2llqkaodf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2vfkiampl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2xsdrgnxz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2poeksqsq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qivdicls.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nqfmusbe.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xogwihzq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2occuuchx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2whekigce.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qrfzdyja.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2pgpqpzzj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rmcozxkp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2goolpxgd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xvqxowjj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2virbluzo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2pxtzzfnr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2pcdpaadp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ozzodzai.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fafxcexl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ukotgpbv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2pozloois.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vqrzosbi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vmgnrjpj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mcwydqso.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kjtrlows.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2rdrsplvw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qmiqxwoc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hnfezsvg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2knvsriug.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ptqrmwve.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zdjnarel.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bxhvpbrh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2scyiaytx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2fryarycj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mtmqdeti.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ajuphzth.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dtobfqai.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zyubegvh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ozkncqkl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kfywjkuu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qeisgsop.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jjzexokk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2yndxfgvi.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2urbmjiyl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2osvsymtm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2bzcrfkab.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2oufybrez.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yqauynvv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qorlkjpd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ciqhtqao.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ggmjcuzb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mnvjfkpo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2uspgdsaj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2hjatqfhq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2jawivmnk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qvwikduy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2kutekung.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2azqbgwfi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2eoypvfti.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2vibdwfcf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qyydfmbe.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ubowvekl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2npojpjpm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2xlkhvayn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2tjyxurun.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fpekxxts.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ubxgfeji.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2dhipivaz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yqwclftr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rliitjfh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rdvxrypv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cdeaxrki.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gninduib.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hxgocbpf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kbclraax.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2eedokifa.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rnowovtc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ogcvbbzf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hkfzprui.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2hbhpdfgh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jrvedaik.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2estkdomq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2trktaeya.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2vnberflv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cwvilfjb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2owskksvz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qqwzsapw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2bpdqbrjp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2unpkyrmn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hmvjfoyx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vgevyxmo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2phjsbgxe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fyitplgp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jhhanhtk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hxbsbqtw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2muzuagub.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uulwdamy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pxiwmacn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dqdhiqkx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gjofqavw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2axupjxqb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ijqclggp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pzlzakqu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eqvjnmhy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2aaejzkiv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nrotqtdf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ddzbkonb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yogqzdop.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2awxwehtx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gvmwxhio.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2xdtvxbcl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2cnqiwqhf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2lqvcjyod.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2pgfrvrku.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tunytiws.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2edgcemgn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2jgfekbbq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2biklvzrp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2apozdzjb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2yrvexfuz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dhuzijpv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2iasejqsw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2pjubnqna.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fnzkaqml.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2fewgdnzh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bhfvqdap.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2utxbtfrf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ptoqlwoe.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rvhynxyf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2nrwfqkcg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2eohmxlcs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2immuarte.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2bmtyyuri.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ananufna.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ztjoefso.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jqvoylgg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xnicvxbk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mvvemqjh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2nzwhtztx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ztykadts.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nnqbgmyp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ujdiivup.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jzxamgez.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2lypswhtx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ghrbqevr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxinisql.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sxgslmry.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hvmiechl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2wyvtwtvg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qktceqpt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lavmjvsg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zxjocjyz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2lfkqhblb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gpxqidcl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2yveevoti.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2apfrghqx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2yseewshc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vehiljgq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ulzkfcdv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2uqbnsfke.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2brlepafb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cpsjotfr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hsxyajxl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2efyodfeg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xwhwbrzr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qpevmxkz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2oyymjtzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfqrjzyg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ahizchan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyuekdgc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2bigronex.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2cnjgffmf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qbbgcham.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2pcvmllyb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kbbhzaym.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2elszrtpg.html


<!-- 参考信息 -->