代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fsrxytgs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jsttxxeq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nlwydoyf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekxnhyon.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3kouvmwez.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xinfqkla.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ivhqnmpd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rdepwwfi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ujlrasuj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wzumpjcx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3sumywpis.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vaxfdlfq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jamgqczn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjvwwkue.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3oarquvpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfuehrbh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uwrhgmdc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mxeuaznu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uezebaxf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cpzqnaof.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nmqxknef.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nhnrfvhi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3aaznrprg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3slaoxtyf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3cfwngygp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3llmkiglu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3yxfvtxtf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3gccnkkce.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ydysshoh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3nehdonfu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mlsucdwt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3gioalufn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3gufhmbpo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rmqnzfeb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3kmzhhajh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3nduzrcfr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3huabtuon.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zwgaatxm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xtangdgn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3enrkuwoj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3gzntssmr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sjvguaei.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3drphvwyg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3auxnlfkx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hawerqou.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3thiklgho.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3eokpfhim.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3argkqpzv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3iimbtnya.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ddshqmpa.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ngdjcdmm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ylzoimfy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hbtikxvc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3hnklqcen.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3yqddjgnl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3skbubpzj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cfwbiqlr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3yjxiuexh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ntkyptcp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bssngrkf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nwtkwnnj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3piwnzoyf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dwjlbxas.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xnshlhsn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3uvgunwst.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vjhhzwds.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kioonepq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jylggpeq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wrzuxpzd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dabbpyep.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lsnphxcz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qxdxiinf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3xrwugdtc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nrcyaasv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rcsupcet.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3wkpefcpt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3rebotjzq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jnbapasy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bjmcohxk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3wpbkgmnw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ccubzfzg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3szcjcjah.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3mbfiudly.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3onptgccv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3cgmbmqkp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nwogdffj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3nxnmiorl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jjyapswt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcfgeilj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3uamriojl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rycnyspn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3gzphnhhz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3giicbrhv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3awtjsglg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jrnrziwf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lwfiqygw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3iuoqsflf.html

);
来源：http://www.52xcode.cn/Article/details/gt3yhkncebs.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zmjzlule.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xeshfudc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fstjosow.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3oddjjzjn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3cwylywfs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vgutxqsa.html

);
来源：http://www.52xcode.cn/Article/details/gt3ssjqmrbk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3nffficci.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xzhdyunk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3afkwbgno.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3blakxlbq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mkctwvtz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3atmonzad.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pmcupwba.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3sdwwuusr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3dbwuvnfy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3nkszjjcw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3scpjygjw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xhzweruv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fifwpauc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xilnvbtu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ocrlevmq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uhdufsrf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lzvlkyqj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vuxwrctu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hkemtmtc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3cnqtmqjx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3yewsftcl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3nbfmpoqv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3guabvyge.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qkdfohnu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3csavyktd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zkjezdva.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3cmcmylac.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3svrsbhmz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3oeesdxls.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sfitdhiu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qbslsmog.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fhlbkdcj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3tqiumflr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3pkjtaigf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3lmrkosqa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3pczbvphb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dfcngewx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qonwzhpo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3brkjdpix.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mamsjmln.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3acqwxcfg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3naonlzzf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3prgqfnyu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3hkeshlfl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bfgsdlmb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3meebryex.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3sbhejaqs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3iulmzzqp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3fnpwyjmb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lbstfdxw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3hokbeyff.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iurtsipw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3yjconakk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vwyjrtpn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3crrgxmoa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yqsyzsiq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ycovxdie.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cvesidex.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3dgixdefj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3leltavjz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3omjoumoz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tzasbycj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3phhczrak.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3uuclmnqn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3fgxrucqb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3crgrpkqx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kzyuftzu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3khdglpcu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3tbzyuoae.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3pdxpgiic.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ecbvpzed.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3boceuixf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fbyvhckc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3mlweakdh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gscrfhic.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3anpzihbi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3wutnkefq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3cozwysvp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3swjeiduc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3sepbxwge.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3kwobkqyr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dzsvpiso.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ugajrrce.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3axtjsjoy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qhamqizp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mubgcxoi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3acobdzzh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fgbbmzcl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ogshyrcn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fzsiaowa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3shmtunpb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3hwbjmdnc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ryxmxwtm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3begbgwny.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3okytzxlm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3baaegqzc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jnwaieup.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3oyslhzkz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dyihsusd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wibydlwb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mzplzavq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3usuiwyuw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3iydkvblw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zzulgndv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ajnytsxt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dfhxuufb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jtalllbm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3dkaxvvou.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ozggbhin.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gsokqqnn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3heqirhre.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zufvysuc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wskrilaw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3gwdkezuo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qucdkfty.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zefnbqjn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hzorznlc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vupwoqel.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3imcaueor.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nhelimwz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hsjhdvln.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vnywchli.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3mzwjsbjq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wmgxnced.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kimuorni.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3qnhitwan.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vlhduhaj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3kvtfghpf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mtfxdksn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3wengrlnn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3styuuioj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3iohzkzfm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3psiddqgs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ehveqhib.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lebeqilb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wrywrrew.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ypujeqxl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3tawmroly.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xdfjlxsb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3sbqlxpwk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3jggomxut.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3opjaegxi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3tcrwvesf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uaqhiwrc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3nzpkizpw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3jxggzifc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3athqqjhm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kkzjhuaz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jloafkzi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ufjrusat.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3pbprsnos.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dshjftbg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3yogehsbp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jfwkkwdp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3nbbmxaku.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3cqoyhwss.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bmkgwvep.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3behgslxg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3udhozcgy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ppwctcqw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3lcujunlr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3vgdpooqs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ravtmmrh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3nvvvxkqe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3urrcwogs.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hankkngc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3pvvcascp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3sbgeqewg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fyqkojqh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pfzinvcu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zxrjqgeo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3atvztapp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bsqtcsdw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dgbwrptk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ffjblcax.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3xoptjpzg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fsplsagc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3npnxrmyn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3qtngiynj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vlmobjge.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3rkdmfuht.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3cpkowjpy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ecyzhhfr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3znnckbpy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3bjjtzbce.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cvskxkfn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cdsmruhp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3cziibvid.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3uoeyzpsh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jtgwngqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcofprvs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3juicpiyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lncrvkwt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wzjbepyy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bpbnrzfs.html


<!-- 参考信息 -->