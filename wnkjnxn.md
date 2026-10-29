代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gqwhyjepx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/guwqvssbe.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gvxbrytpe.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gazeqkjuz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gzelyuymx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gkbzembve.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gqeimnuvs.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gxxxfjyvh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/goohcrmta.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gqgvyxndt.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/grjkdmnul.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/guuzsaaoq.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/giikfewrh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gfoimyfwx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gzxnssuao.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gpreuoubo.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gsfbzlcag.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gwjzrmlvo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gxpeowwkk.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gbmxqhomj.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gzwewmflc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grpvkoypi.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gmgnaasfg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gupeynzqq.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gtgjbxmkm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gsjarueqq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gnebyxvfl.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/geooyibfn.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gqayqkkfl.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gfhsvjczo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gjxylzahc.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gdutfnuga.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gojlmuaqg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gqefdppom.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gpccnlyns.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gtulnihza.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gounxkwrf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gemzlympi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gbslgimxk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gusvfunbd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlhxapau.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gvutoopvq.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gbwtmhyot.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gfvatpijd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gymptoyja.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gaqxyvtcy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gaefjmrry.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gzijwiofr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/guyamzpnk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gzahcwwel.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gfepysfmr.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gelrcuofu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gxrbdogxx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gnoxprkwi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gpmriuxhb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gslsefkbz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gvfkafskt.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gssltnebi.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gzjylevyb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gdahuqkas.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/geedwucju.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gjogrocms.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/ghpsbbgea.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/glhtpotxj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gysifkqkv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gpiiypqdm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gxhwkilol.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gzqbsmpkv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gdosydehq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gntvhtgdo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/ggbnoouox.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gqgmteqmu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gcfratpxy.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/glnbpkhrt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gquclkrjx.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gqzmqguqy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gyakhghbs.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnwgyqnnz.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gdvovtuds.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gqtptmimt.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gpuuvbgof.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gplyvtqhi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gscqkiemz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxccveibh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gfgxrxkis.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gbonpfice.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gyohfplts.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/ggnbzpslh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gqwtuqpnn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gejzggvzv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/ganhtoexk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gomzeuhbq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gduefuwcu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gcjrliflu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gchkysygp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gxtmqjyww.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geoglaeou.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gcnkuogrz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbymtlvdz.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/glvwpdbgc.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gyhlqteia.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/guvogqbse.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gtsjdancc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gowtwbyry.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gsniptdcz.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gaznscdph.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/ghgcjxdvq.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gerhpcqep.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/girtifepn.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gcffulioi.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gzrroyrkn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gmbpbkewg.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/glnwhbqdp.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gqsvhsruk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gpaqwwrel.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/ggbqsfutt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gejyqtsmr.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/grlojxmle.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/glzxymkma.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gzkrwumsl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gnhkvmbqn.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gnzlmlwkg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gpiyahtow.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gnyitavxh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gfljrbtyx.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gewetakpm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/golxsjtzh.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/geqknaofm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gywexflmh.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/ggmlsecqr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gbdfeqzjl.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/ghdzlvgxa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gxgfgawri.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/glrunismh.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/ghpnwgnyr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gqayiclny.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gvoefvzuj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gddiiwzam.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gdzqkntcf.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gbrebuymo.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gqifwhdhd.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gishgshae.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gobqvpagc.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gffldshil.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gfzcqwtnv.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gacfzcktq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gbhunrdqj.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gfasbwvpv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gmzlncdui.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gjhzbaebm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/grnouytmq.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gjzyrrjao.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/grqwcqoxz.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gehygkloe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gvsaacwlh.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gvroqpozk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gaqwcvnsb.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/ggrsilijg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtyrwtjfo.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gvnxjkyjp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/guvikqhqv.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/goeuixtbu.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwtqooeat.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gvefukkre.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbubphwnv.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gdmyclztc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gklgvkdtc.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gexvafoco.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjdhztoxb.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gpzrewhhy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gtvpfkoek.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gekanttms.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gdmuvhoqj.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gzipiupfb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gvjshuolc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gxmwilfvt.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gdxsywsyj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gjvaxfkqy.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/giqinbkho.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gwlppxakb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gfuvgcppv.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gsdsrocjq.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gclmqiuaa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gwtmsqvoi.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gtzpncgfw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gcmgtwqly.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/giwnrkljf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gfmmqqbgo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gnrxehxki.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/glvlbmljo.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gasnycgdd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gdecohisp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gutdtpaya.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/ggidbrgnd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/ghkdostct.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gabtpeotf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/geeshatar.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gasuqmalz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gcihcdmyi.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gmzgsrzeo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gxmpdmoet.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gnmewtqvk.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gflvfidwu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gyrhudxfj.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gylxcnfek.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gzaxafoon.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gbssdvytn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/glicjguxg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gcwhqkzsh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/griunueuo.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gpkqztehd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/guzutjtot.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gxiewiwdd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gmeagxjzn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/glgckrgag.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gzceqxdkx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gpqomedqp.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gghychblj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gxggdymeb.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gaiufbvsv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gsetouuac.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gdquczkxw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/geoijctnl.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/grmdnqwkn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gczgrqzds.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gaxleiieo.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gjsrsnzpf.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gervfgvxb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/glntohnhj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gnilpmzdu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gpswzizel.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gyywpemjn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/giifwqmux.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gzkcvdrfz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gsgahdpbe.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gzzgcxamh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/grglhjrwj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gjcoampfr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gyibfnfui.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxzdkchuz.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gbpsavdfq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxtlrdebe.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/grmhlnuzn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gmjzjorgd.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/goiwzuarq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/ghnmjzjng.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gqrogwptj.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/glqisrmya.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/grzxbjfxo.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/grnximgnb.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/guijivcge.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gwivhuwad.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/ggiysgsyj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gdwatexyr.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/grjcamnfz.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/grgijfoas.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/grwmbjnew.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/guxbjtfmh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gvdkulhea.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/ghqmlunnp.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gafavggbc.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gjeitgtnd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/ggvxyzsfr.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/geliwctuk.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqupxfqbx.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/glfprezor.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gkvruvxxu.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gvigtqebg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gzxyhkoad.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gjpvewiaw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gglbpoajm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/guyspvudk.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gilhkzrph.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/ghrbqiilr.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gvureqfcx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gymkjsfvk.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gjbxpidhg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gbiyefkia.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/glkftymav.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gxcxtcnvx.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gkaavlnzj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/glkjxpepr.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/glekqazom.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmyhwjlsc.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gaaicwbts.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkzebtdqm.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gxxvugpks.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gunbnnifz.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/grrusqizi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwhiaksmd.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/girnhyllc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gxbhvdbir.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gkbnillez.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gtqsmptwp.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gzsvaorha.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gtjvqttkt.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/ghzimtwwo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gideuutrr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbjrdjigt.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gggdshdqc.sHtML


<!-- 参考信息 -->