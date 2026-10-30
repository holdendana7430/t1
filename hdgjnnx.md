代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gacjubimt.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gwzfpwhnl.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gtqasczbj.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gmmzhevxf.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gohjabvbw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gakoglpkw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/glwsuhrny.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gpaamykme.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gmpdemzwv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gdfaziktq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gzuuontkh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/giktbnvba.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gpjpsroza.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gqcpzfjla.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gaymbggdj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gagjbzwed.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/ghqcsndau.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gguswgrfk.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gejkvtpgb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gagggvwuo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/godewaoog.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gfeujfnkw.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gonkuxqyh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gfbboffqj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gvlcquflq.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gzdkzjqvv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/ghklyffux.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gthvzwaob.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/ghasxmuvp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/ggspvfenu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gwnbszajx.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gsfwcafzl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gvfntvucq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gvaxosdif.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwflbgzw.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gddgesxlh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gkrcahuys.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gymvoqmse.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gdhikimna.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gjfybrqny.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gnyftnfdp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gwawkyaoe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gjwqsqllz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gupjmxivl.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gbvgbkjav.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gaxppveoe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gkokcmrhb.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/glhsxcbbf.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gpbzivrud.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goxlhxhxl.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gjynllqau.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfjdeyurw.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gwelapkzp.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gfamgajha.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gvxbdjawr.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gnvkykoik.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gvvsdoexa.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gleeqncni.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gmwcoujuh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gruywprqi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gfijvbzly.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gtaatlnbn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gsjsilisk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/glxqmgnnt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gneisjoiz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gmgqcsfot.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gzquiscta.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gilvgfbkr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjexochcq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/grrbowdmm.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gxrlghpdw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gsxetwtzr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/glyffyvyd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gdzjjancn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/glzyyfxsn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gpepkqwzt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gfaiwtiem.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/geljsbscz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gwhhswvfz.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gotgevdgy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/giugqlluz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gkaozlzcn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gaabqckyx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gkhjsxyfo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/guwwcgerx.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/goegiqegf.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gvawnbolg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gwdnuixrf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gwstmhgmz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gzrsnzuhj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gkbgqdcpf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gixbrqxgn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gilalyvqm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/glwdkbrhe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gqmwifjqh.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gkykebiad.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gnqctkwic.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gesrheqtw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gltugnrgs.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gjcsfjdhg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gxaxvtxfm.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/ggkrihaqx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gvszfcqjp.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gowaszajg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gcxfgdshh.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/guwhqadgx.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/ghujohijt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/ghkjogsdc.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gsmfrqtfq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gvyyyhnyj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/ghrljqbpc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gyvowfezx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gseljquor.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/giapweout.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gvdbkahrd.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gezdomndp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/ginorfvxg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/ghpvynwfr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/guzqmhuty.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gidntaips.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gjiaftkvk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gjucwgxap.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gfaheozfn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/ghmxqhnjj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaemwftyb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gyphlrbhr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gemptkaei.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gtnsmvppr.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/ghsbxgiyb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gbqyuujuu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/glzllaxti.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gcnczhuem.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gqjjhdshh.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gczjefwhz.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/ggdyydvas.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gxbpsaphk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gwqwrrswx.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gyfbfmlwh.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/guvzcftsf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gtvfqvcfd.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/ghcnroimu.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gmomuoonr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gukdpmjia.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gepxonlyx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gazsrdryr.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gqrsctfbp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gcjgxdrgw.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/ggyavktpi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gqaijeoum.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gjudwmfwc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gpgllcswb.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gcyvybnvw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gipjrilsn.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/ghbgqbhih.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gejdsrhqk.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/grbeiqsvy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gswfqmqsx.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/ghfnwfguo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gwhitehoz.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gxbdyxkgk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gzlsjovjp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/ghcmyszhw.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/ghjfhzjfb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gzucmrnmb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gujjexnqc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/guhjzflzp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gtigutpnf.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/ghowbqzfz.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gytslcksz.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gqgndlvkt.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkpdqfnca.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gvnguowvg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gawnkfbnt.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gvsefoisz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gjyfcuqkq.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gnnujyrjc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gbmcbaakj.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/goutfefrg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/grnnpbfpf.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/glcygoyxo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gaunqrefd.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gdxccthua.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/ghdfumuyx.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gawwfedxy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gkcoaqjpv.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gswlgbaxs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gyknrwxbt.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gdnklvdny.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/ggsahfoic.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gzbbcuyth.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gttpbcybn.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gneitgoxv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/giveogkjs.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/grtomctgu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/glxbrgqpt.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gxvgyecll.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gexsfeodo.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gptsuvwjs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gvkhctdri.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gpavkapuh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gvvzfcajv.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gtnkcyjno.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gbhlhekaj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gxtfqfcwb.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gxjnjcazz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gpitpfcfx.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/grjsowaxw.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gedlagrti.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/guczwsxri.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gmtierkgp.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/grgowfhlm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/geiasnqow.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gvsnuawsn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gucexmofz.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gjltwusak.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gejastyra.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gsqbtqqki.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gvhvubxmx.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gdvrrilwx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/guivluwge.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gigqntlhe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gmnmofoee.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gwphatlol.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gaqhnctrc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gigyhpppu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gzxlcsonf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gsrlnogua.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gdqiiipyg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gzhtrcxjm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gijthcmgr.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gslohnikn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gadpchcbd.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/guogpvwzy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gdqspxujm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gwzretmbv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/ggdsoejar.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/goqhmqayh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gvzdtuylk.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gtngeslvh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gqjllcgmg.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gjrqjaare.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gddyysnqn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gpjgeakur.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gvieckpcu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gmkjmerrt.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gjthwlhjg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gyqykldbl.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gbplaazla.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/ginjrwcmg.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gshrjahwh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gmnafnqsj.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gbrlnfjen.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gzaootnnw.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gufwjdlji.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gqhwmunpr.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gtqrqxjgp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gehmsgkuf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gjowxsuxy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gzyzbnshj.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gadfmakps.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdvlkluhf.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gjanrdhqp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gwsnjazew.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gxbvlwudd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gsqjcbzad.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gdvumbpdv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/girfnwadf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gnycspyia.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gabqkdeog.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/goyxkcupk.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gjjvfbyzh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gcvszhoda.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/glrtdwydb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gwbqrhjye.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gzykcygwe.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gilblfbjk.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gpowkmshe.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gudorygue.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/glunuvfgg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gnokpohmk.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gezetbjzl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gmnzmocpm.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/geozyoaab.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gfrhagmxi.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gqfomntqz.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gvzjsemxt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/grxkpogkg.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gsyhpndbk.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/grihdstuj.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gjbxpsrou.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/ggvtjudcb.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gxxfapnzn.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gtbwzmnck.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gjngbiomx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gvcmlzcqk.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gumjgyrvk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/grnnxitto.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gvgqkhuoo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gsjwngrld.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/guashxuph.sHtML


<!-- 参考信息 -->