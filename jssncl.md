代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2quizyctb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2whjnhpgx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wvpexwwp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2nebqghcj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qmqtximt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sstlvmxs.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2kpvatevt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpkjigct.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bbngwypa.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2teixaxli.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wjmglxkf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kibjmqfg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qblazptr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jnhhxzqa.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cqiigkfr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dwrnzglz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ckozxpmj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2pncagvsj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2yohemtid.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2twicxxib.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2owkxarby.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ygmbbxcw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gonmmzij.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2dhgriscv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2csvhhdlf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dnhqurzx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nnyvhuex.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zzukgprz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2starvwhi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2evarrchu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kbejipys.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jgxtegxu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2nbeuhytj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2npqnlwvv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2iekreqee.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2mnbchhey.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2hogwlean.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fkfioawy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2plivbebr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pmautpgu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hdgxxneg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gnuynpbv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2thkghtrr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pwwtpiht.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fmekssne.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2bkdjjuwp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lgshdbnl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2yonwduzo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ogusants.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2cfuxtpho.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yicsaubr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2dvkqubjc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xcbloyon.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2nxvdgnff.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ggfswpjw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ytynrdlv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2coqlnlje.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2suylmctf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jtffbnri.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2frzmzygi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ruxbqocm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lppmxbyt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2qdkuyher.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2nmfwibty.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2odyhmqiu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lpkfkiqi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zwmemtfs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rygstyua.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wcsafssz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ejouwhsw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2knctvugi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2edynlcep.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2himozzfn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2kcydspyf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vjbvrovu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zctwtqys.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hrysgsqd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rgwbkljl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2eswjpxgc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2rnxqksbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpzzgwvp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bhwthoyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utontuwt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hyljdpyf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jhvzowig.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2noaridvu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2cmrckhtf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2djqegfqu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ujovaikh.html

);
来源：http://www.52xcode.cn/Article/details/gt2tyufndwz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kkodzgzl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2pcdgfvjb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mniumdkw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2drzweokx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ayonmiph.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2jtivwjcy.html

);
来源：http://www.52xcode.cn/Article/details/gt2cvxryrtv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2wqhknpya.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2azmsphqw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ybzdbfhj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nbeewcvq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2jprsfajh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2vobkuwad.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2rwsmuxvb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2chyewxtd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2uphdgdct.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hoomtwjw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2dbmtwbgu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pxmzzwru.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gsbxjprq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jepbuxkg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2oxkpylfu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tstlbdib.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2maeggang.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uuujxbve.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2rhmdblnc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hwcrsqgw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ahyvhxnw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2rrwmrbnh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2llwaszjn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2caceoydr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2oqbmwaml.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bkpkomjf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2uiohkvog.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fvkvktuo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2beywfmsm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vdvnxhji.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2vxuinvpn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ivariyqy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bpfwtbpu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2zyrpkqin.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gtakbyox.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bioumufv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vtdkmncp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2oajtljse.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2itkknogh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hbgrfgoa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2svjerhxn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kcxwjfkr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2yaczqfgb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2qqsvbpgy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2otsodhvu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mqlvvnyh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2xniksszl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wriazmjj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2gzyiwudt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fmaprpsd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2kyhlitqa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lyutbydu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2uwfzjqaf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ckgzivdn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nvuxmvzf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nvczseaa.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2toumgcmz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xbhbneyk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2afgofidh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zkhnbgap.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qakzpvkf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cbetnczl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vkjlwjed.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2azqofrnj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2lbupryzg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2xfrhkgvl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2xnlbfjca.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2rebwpaeq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cmknlwuk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ndudjrzc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fvzadowl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2drxmysnq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vqhmrayw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vjqxlums.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2yclcxcqw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gjonxltj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wsmuqorl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2fgbocpvy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2agcbajci.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oatxpzsi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dgxczfha.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2prgfwdlp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2szbtllxo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bbysixsi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ghsysmvt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2nltwsxtg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2oguoadru.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2sqavfiqc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2apisncrt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2towxaolm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kblhynih.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pwtykemr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2txxfjpug.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2lkaxttuu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dzkrenxh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2uuhjafgm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2evbnptyi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wgyirqoa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ojqrohrk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2igegziqw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2qkzxqhcr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pfxkgmlu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2gtjfzkpa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yjnupjey.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2clocnikm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2doitvxqu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ccivajbe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eeibuopj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2khsurvfh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qkaqnqog.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2xzkgesic.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ioadcbqy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hvcuphgs.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2xjtbnqut.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2enwbehud.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ngnwqldk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fcuflgya.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2laekxsbw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ubzekerc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gtthejbc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wgdupdpn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rtchecfv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2usxkzwjm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fvuwqmlo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2agmjfskc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2epjfzlxl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qmisrhao.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zkqpiigp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eaqddltf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ezvpbsnr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fxuirboc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2etunvhmg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2tebyhrma.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2sjbvjbrp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2snsxabfw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2nlerbbrv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2bubbqksq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2emqrdqsn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hdbuhssd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ryomyyjx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2cqxpewbf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2mmxvuvsn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kljaphak.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qvmxpyuj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2bvesuwlw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2jdxozexq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xzsefqsu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2lnhqgadp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2hdyscwja.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2czqenglq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2esxkgfon.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjchblgy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rosxyzgj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2mlpkkyhd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qzmcgsgu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2eqwrmqrs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tihnmrln.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cpyrlmkw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ikznlspw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2dbwnjomw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2blzawrjv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pgxyyoqp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2nxsoywfo.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ndeqygko.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jowicqdt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ounzdgrz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2tqgsrphh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xcioanbq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mwkvzdqw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2oktaajyw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gmiakaks.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2fluptejh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2txqedpxx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ypxbtmkz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dvxhxfms.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2nsyklagf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2supxdomq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2rclsknvp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jfndeixw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qzowfdxo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pfpgtecr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tnvnvome.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2fynibtti.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2eymezwqv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yrbupnue.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dizmurqk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gzwaqqpw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hfdablkr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2elgspnuz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vyafykee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dixvestd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fvbhxkhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npmubuoi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jwpebhsy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cgojzunq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2aarashey.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jaygcmmd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2dfyeytuq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2iintgdfv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qjiykqst.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nhjdelbo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2txxnhmte.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2harayhog.html


<!-- 参考信息 -->