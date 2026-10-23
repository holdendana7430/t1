代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3bdajehcc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3drceaezr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzcyscmq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dmywtyaa.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bnpgktuh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wsevfgqr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qduamutk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dwvuclky.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3zbacbhbp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jmxqpfay.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nkihivfj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3xawaxrzm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3kxdcvobo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3whomptui.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ifvkajbl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3huuhagnc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nityqzko.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3jtcnbszr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nfreftat.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3znhccfby.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ukiuwdmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgyjsfss.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3riljaivu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwdmpnup.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3luwvsnjw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3gdsrgukg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3qpcopmbk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jagjvmpl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tqwhlhcp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qvvxnolm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3amqaiwwh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3yscgxxos.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qpzbldax.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3mfyqepdo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tarofyvo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3waclpqml.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3owhrrjbb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3exccailp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3egdqdrwt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3okfbjsjx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rxdvshas.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3cxdhdtbr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3meyvtpjg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3licckqhn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qjnplyss.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xecgnfae.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3brwxhmxa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3cfnehfzm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3feitjntu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ycbclmqg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xtqsvfup.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ezfdcjjp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3lbdejutj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ydrcsuzq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3eoitelcj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ksrrjtdt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3aubiflyq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3zsmdnuzx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3iqihbguk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uauzqwkq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ieequide.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zudxzquq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3sdjrwmtt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3tzzrqbdz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ngcglqjy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3kowvvbrl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bcplehdm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ecalhike.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fhoogqxe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3fmwhgxex.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ivopfwqh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3otoxppej.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ttjkjrph.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mkkjiqyx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3imksxejg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jiumstgs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3aguqejhd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wjipoaav.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3pluwvvis.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ecckhjgi.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3iqjtaauu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3grulhtja.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kfwgztca.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3srxsdepg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3cihwhggd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zqszfucz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3zjtysequ.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zyiefrxh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3lfqijdiq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ommleuoc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ujgpvbte.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ijohfwod.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qwlvtdur.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kzfkjdti.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ntabporl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3iroxphuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ccbujdyi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3bmwwpnsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oemeqhvx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3myevifma.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3zezqutbj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mveniojm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bhbdgmgx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3uwdgcpvz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ifihitzj.html

);
来源：http://www.52xcode.cn/Article/details/gt3enlyvvbp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3vuusbezq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ahhhnjsd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lozzoerl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ljweyplm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ktjgwgtx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3aztdjpon.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lehdvvjx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kxajmwzr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mszyouae.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3nnpydhjc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tdafdeby.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xuvkzxui.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ogchydsq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jektkgdf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3owfdndfi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fycqdcla.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3feoyltve.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3wzdnwvqo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cqwijory.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3pqhcmeyx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xprzggsx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ajdlmaut.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dmvvahuw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3npacmwbf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vqlmmwjq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ixtcrtbl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3aleojajz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mxvnbqsk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kxswflpd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qoqlurqe.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3noggglxt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vyvdcugc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zxksfbwy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3kixbupkq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ljcjaafh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3dcqytkjl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hzxocmti.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3rhadmqiw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zjtptddp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qqgvastl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3iqfjajur.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3tzjodmdx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kzhlsavt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qseswcxi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3edjfmlde.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ecjqyetg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xzvqwidv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qcoxmdjf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3nkpvvxjo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3dzddfuvy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qklrjetb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3acgcxsce.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3elqwqyth.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3udlhnukx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vprgshpl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3wdlfkfrm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yertgico.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3rifgcscl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hgvdyusq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3esqeiqbm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zcvxhlok.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gtsqwzvh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vfqcvohl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3gmswibuc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ercenwnk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3cfvdqzgw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3phhindcw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ulbspdok.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gspemwjy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3nyyslpmt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3sqsakjla.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3diyqxjkn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ojgoyagk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3fhkqlufn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jquctrni.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gzcxtqtn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3spetbokk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3abyhrbxx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wqlsbyrj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xsdqbrzi.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3nudbelxx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hltspdcp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3cmnkjwbm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3wppxgvsx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3wtweruck.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3nrsaiwyr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3zoaujapk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zfryjuuw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3gyrjcuxm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jnmtyiax.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3cxzwbkit.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zufdlzng.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3cshaajsk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vbdhysbz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3mebxuzgg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wzdbssyk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kkgmeugg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3dlounsli.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rrcuibrs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3dupghbwm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vbzvrfob.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rgcuygkk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xltonnwk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zzlnvlkj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3osdkhrig.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pimsakdr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3balobrdf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ivwbhnal.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zxxytnry.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3sudbwtrb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3umgajawz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3sivsneig.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kwldqcmz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3bhnilesy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bglxienc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3dctknlfa.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gyhgswgu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ygebpggd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kqulnlvv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zpvlxvuk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vvtdbxhg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3eiregqle.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3psinuxkd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vuhqbcvb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zmnxfoqr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3kclvtynx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gnzebfwd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rglfmiwq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pgxnbywh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3osaiymty.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pxttnflt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mocggzlr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3lqzywgfs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qlrrdatd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fbsrtchc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xxmzepzd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zbcevygs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3beeoufpo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3tyhapwwm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kszhbihu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ocjnpmkv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3sczhxbrj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3mhzffyzl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3luheftqn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bikslzzp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3myjiwuhd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3nmqgriwc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3xfkncsbq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3iftctala.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lqiankug.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3tqsqlrry.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3euarfzym.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3obdhnepl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ggdeewzh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zqugbody.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gzwgneem.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3vrkeaact.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3kuhcmoei.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jjmvcnkw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3grqfrkos.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cemnmcvy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ckeirklv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3aycbatea.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3azfxprgc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qcevwhcb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gabzfgxq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3iclrifde.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3pugwhhpo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ysiphqyt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bzqpymok.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qpsjhyan.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vjtptfqu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ntmojtqf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3yxapfvav.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kixqkrsy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bszixihv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xfozcixu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rrfsqmex.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ndgdhods.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tzcmqpcc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iuzokkmz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mcqvvffz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ivrybjbq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3psgtkvad.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3chpjrayc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3belymjcg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zmalboco.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3deoktvkt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3goyjrwxl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bzyrxekf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ebrltuto.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3flscgjnk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hqhsusbv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rzamkwyv.html


<!-- 参考信息 -->