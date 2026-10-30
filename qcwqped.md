代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gesxiiifc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/givqlrkjk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gzrrrlirq.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gxmnrwwvm.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gyjlvhmlt.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/ggaifgqby.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/grywfatfi.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gqpumlbgj.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gbphwgacj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gdygwvqok.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/ghqpkuvyn.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gbbigxcpt.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/guvzwrvsl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/ggrvyhpgx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gggjliehx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gqalnzvji.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gkgyeyzbt.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gmrynevxs.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gtoznxclv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gwzxkuwlj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gjeqefmnd.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gcssnropf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gfsdpojfd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/guacvbmkj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gingugbqi.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gxuhjtnfe.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gkrfixoll.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gcfobuzpz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gxfuegjli.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqglfauta.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/guqpsxiqu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gbmoaqpyn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/glwtoskfa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gwuikkvee.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gpvabuden.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gwefwbovi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gqpxtnbod.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/glwpvbpgw.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/ggkevootp.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gnqsophwh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/ghjfohddz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gqviyrinv.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gpoyrscba.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gkmddylpj.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gdyowselt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/ggguvlewm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gobuqsvkd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gjtagydho.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gjdgqsixh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gmewrfnoh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/grnfpkvha.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/guivzooxz.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gpndijxhs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gampfihif.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/ggmdpucer.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqihcwegz.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/garfpagfi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gbwnjhzia.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/giguheqbl.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gjfmphxmt.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gmjrgyucs.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/glmvohdul.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/giliqmpdb.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gpzlsbomw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gviorkbmv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gjwsjuiva.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gashotbxi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gjsddxnwk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gphnzuavx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gpauwbmmd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gjztjxhxx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gbvhzfobt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwksovkoi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gjfpwxgdk.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnlwaaxmx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gywnaojof.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gdzaqobph.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gfykapcul.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gotiejsei.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/guhptkoam.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gnlrtdkdg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gtlwamtdw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gsjhtnhxh.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gmhliesid.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gucdyforp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gcbsdigfo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gcrrkxxrh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gkocyyalo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gglxdhzbr.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/godnskllm.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gtbperkvh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gnihufumn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gtsswzyyb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/glzkmijyo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gqjgzvlpq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/ggajpcjft.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/goylpvekx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gmfbxpspe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gaztjjpjh.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gligfitiu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gjeebqveg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/giolowvyz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gajfuirbj.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gtjhtyvrp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gecbnhnff.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gcvdrtqwi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/glsrfbplc.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gvcwtrxhu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/grgwrhsis.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gxpmhfoqc.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gsgaithye.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gzeynfzvj.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gqzpwxgou.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/guizklkzd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gcwmljjtv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gtndgzddy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gfssultby.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gksvcocdb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gifvdmzpp.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gkieyjugl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gxtmgvjpx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gxtvlrvfi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/geihyrkio.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gmxbsizie.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gfohmfykl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gzywfnxor.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gvorsnftg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gmvgabgqt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghcfeanbd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gqyathdwr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtopxvkcp.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gegerzfim.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gvbnwpdbe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/ggntbaiex.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/grmhvkear.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gxmqdblxk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gpubgveyx.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gbeqpdsqb.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/ggnkkybuk.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gftuxfmwu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gvccdwqdr.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/grpubspsc.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gwnbokbhq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gwcplzvrr.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gzpdncqjj.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gxjydzvxs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gvwrlhxrw.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gztwfyhbl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/golxxnefs.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gyigqwamd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/ghesfpmmk.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/grsqoyata.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gkieeofbv.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/glrbkrqpk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gbxilukkw.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gwfepamsg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gyifkgpbt.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gqalugqxb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gkypqmssn.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/guzmzzwpu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gtwkzqzxf.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gibohpxjb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gmxncvgne.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/ggzowamdo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gpfhpicff.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gwpwhyywq.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gsjfvxcit.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gssbnibdm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gmjzhybrz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gidfkzhkw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gmjwsqnnd.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/greetnihm.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/goafppfhn.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/garbpamoo.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxcqltier.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/godfgbywo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/geqmjwetk.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/grpikpxzp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gpptgbczr.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gmvonqkxn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gptxcjkzj.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gzwfnivrn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gvvgwlzga.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gchyebqgr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/grpzcdojp.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gbnlaerqi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gdzfajbti.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gblrnjatr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/ggcpezblw.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gctdzebur.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gnhavcfda.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gruszldyv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gbbvlzrjw.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/guozudflj.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gwtihnjpy.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gbhsqiuwe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gapmgyagm.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gcddueccq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/grgezhtuf.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/ganixfcsi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/ggworkyrk.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gevieffnc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gxojunroe.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gmnvqstul.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/ggsuhhmaw.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyarlvqhh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gyutopztp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gxolgmrxo.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gfrmcouil.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gzgldqkok.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gcmimfnmm.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gtfripwtx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/ghtpwztdt.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzbciuhll.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gsvewzboi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gjksihghd.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/grbzjhkhf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gbtjpxfph.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gtfttkeii.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gnbukvuem.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/guzzaeiiw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gkxvskcwk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/grydtxrcs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gsucqetit.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gvjypswzr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gqbuoeeff.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gfvcagfpd.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gkouioxhi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gfavsynbc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gxgicgxps.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gigwpbccg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/goniusibm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/ghiijxaju.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gymxtexqh.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gvequbivi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/glroicxfd.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gsazgnnij.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gmkijaikk.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gvhkjcdvi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/ggkfjngwp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gzrlzgxhl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gkhnxesni.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gibrxggvs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gxcjsuxka.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/ggdpbvshx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gqharpzaj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gqiikdvil.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gaernzxdb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gsftexksg.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gphtijyxu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gpnxnzouz.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gespoecvz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gbyjsxzei.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/geblhesjh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gxvixgqvr.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gqbtofuhm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/genyrrzlq.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gknldjhew.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gedpwvivd.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gxhfgsscb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gavpsxuij.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/ggliegnre.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gllhlmlem.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gptyyzaus.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gujsrmase.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gjxjwssxc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gejmyhvhx.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gjorqvgkf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gwfggjiqs.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gdgpgnkif.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gqeakwres.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gzeoshdoy.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gpjtioikm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grkriiuqw.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gouzouunq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gqeqqnlch.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gdiyypbdu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gecnbhdov.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gxemfyjtd.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/ghrdvzmad.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gsswlourk.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/grkvdmeqz.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gbpoaridu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/giggveafg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gsteewzar.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/ghseuvsih.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gdgvvdtts.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gnskhqhxj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gvhdieqgw.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gsnezsthb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gaexzhvcv.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gvpbogbyl.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gzabvhfvz.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gdipfkfoa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gwkdeaira.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/grobdthtr.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghmhqlanw.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gjkktyygk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gvardwwqo.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gyfpsjtbs.sHtML


<!-- 参考信息 -->