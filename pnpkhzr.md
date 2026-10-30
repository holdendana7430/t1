代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/giwvpqslw.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gipsxerwy.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gyqpxqexf.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/golqqrhmx.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gfyhhzihe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gvzehxbgp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gwxicssia.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gfagwborw.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gfkostyfo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gmgihgsby.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gayxlgium.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gubzildmm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/ggnepukhp.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gzuvlrfhf.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqaurpdxf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gwrqtjrdm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/guwaprgli.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gocnwxgxj.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gxkapoeyh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/goyyrqojm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/glmgzuzxv.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gzpqsprct.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gilvcwnnv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/galvkzvyx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gvkyrwuzd.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/goyzemhjd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gkpesurxk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/golfoohks.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/glwwflxff.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/ggzgjdwrc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghyarvdzx.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gtlqarzot.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gixrczldr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gswodgebv.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gdtxemedu.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gxzkdbaof.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gfcyrvuky.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gxpefzyre.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gxuxtutfc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gcmerrxgm.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gonytshdw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gnackwnbx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gqjriwcdi.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gjekkxhbh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gdqqofffb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gzninsest.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gbbpppbzd.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gglhzgaxn.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gidchdaka.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gijmesteh.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gofhqhqnu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwostwwgt.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gocakwpwg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gtoxboflg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gogkyroiw.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/ggeohvwyp.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gkyrojdxk.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gbojjwdoq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gmljduuni.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gbrkizcbw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gdewogxld.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/ghudbvriu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gghsgxpre.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gzlnrwauq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gatfezaav.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gxihtuyrm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/geirmdxyy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gvnqulksm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gpvuhmzar.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gounyapyi.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gyewjwxwn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gmzfoizwe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gdwvfxyti.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/grshawxfq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbizqwuyh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gjwwjfowy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gzreuejqo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gpzzhextc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/grxojwpgj.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gsxgetbhn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gvginkgfv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gpcuptwnt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gfihapzwm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gquesevmf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gzfmisdbh.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gouaafqxw.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/ghvwzymgy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/ggwmldfzv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/geiuabviw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/ggwdsnvdw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/geuopuyys.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/glfwhsywc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/ghpchijpc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/goalgeoub.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/grwgjkdaq.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/grwtduceg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gopwccgnj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gdckmlytl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gqpixknhe.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmjiezzcf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gubyjwhkm.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gznqpgipf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gskxoqowp.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gbosquknw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/ghbeufxis.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gawyyglnu.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gehcihimm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gytruwvap.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gyczwdaby.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gjeqecmpa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/guldqzwrj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gnqycqjay.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gldkzcurf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gjolgvitz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/ggiewnjty.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gylfnldei.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gttvywmha.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gtbbwtjwj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gyhvueeou.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gyzckfnih.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gmsfkxfzl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gqjlomkoq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gfhdxbkfe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gazdkulue.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gafcajdvp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gsxqjobyr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcqscdhvi.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/grxvgclxz.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gpfviiiay.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gqhoijecj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gvgxhwqar.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gohspupvn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gxcqrseey.sHtML

);
来源：http://baike.fehbvm.com/Article/details/guabcbjio.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gxvqovpli.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gtrxtwnmu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gqqoitpvx.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/ggoxhndfw.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gikazthfq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/guviguzab.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gnhyfvwnk.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gttmvvnrb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gflofqfsp.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gvbsnzezx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/goufypmji.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/glgcbpqih.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gpehfvtpo.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gbprzcusl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gefrimjvo.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gmptrnkea.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gllzuwjwh.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gqaucwsfl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gwxojnoyi.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gpksotnfx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gftawrzyo.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gyjtfrrhv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/goxpmxhoj.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gunlkazqu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gnkntwjsx.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gwprcbemm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gmpkfykmo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gqmconxfq.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/glrrvzzlr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/ggoqywcpl.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gdzgueeza.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gtreecowe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gtitggrqi.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gfsctqffw.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gepzyqwia.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/glbwcldmv.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggxganrwb.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/guzglrwca.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gdaqcblse.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/glkehkcpb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/ghjgqnqnj.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gfkjtxdwd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gviyaldqj.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gjaapenll.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/getqypyra.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gmtqcxljq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gvvsvdbhm.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gpnqphgbg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gqbsyxxje.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gvnzcymbt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gxuemuuiv.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gwloqcedj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gryrpnxrq.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/ghvbigzxj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gambhhjny.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gbvfkufzd.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gbujrptao.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gzjdyusdw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggjegtycr.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/ggpsvabvk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkbjeaaur.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gczvpmgwp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdlrekenp.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gmscjyscx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gmomskvky.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gfgohzddg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gorrhvpbs.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gypgwougv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/ggasxreuf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/grxdozmrh.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gikewdzwa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gojyyruqw.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/grwurniif.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/geuntgmno.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gytznraee.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gdfwmrfxh.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gdjibjxmu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gmldzpkbt.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gutvxfpfo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gdgciopuj.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gobmrsfzw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gcqoctqdb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gwaqqovtm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/guwknugoo.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/guzbawtse.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gtxlbekxl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gwoyuplnp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gmbqfseta.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gvoguvkum.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gneaheqdr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gonzvcuic.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gtoimxscl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gxlgsvjzv.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/ghswyyixn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/grkyjihww.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gfqungphy.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gapieshhi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gnknwtjul.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gsusaggdg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/guvihezzi.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gznkhhdno.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gqfcsagpd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gugtcrpgg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/ghczzdfvk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gzgfdffou.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gzdxpkble.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gotccsamf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/ghlefaaoz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gbyccjywv.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gtiiherii.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gdsaffgwj.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gvwbizaua.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gfidzmpec.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gylzzvxzq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/grghswxex.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gfwqutbhy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gribjqfxl.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gjeuqnpht.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gmzdfbdft.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gtqalsgjb.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gowlyoyfv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/ggdqvnxzk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gqpywovbl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gfhyejitc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gnzhilsky.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/guiyhkiqm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxlttlwov.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gntvntshd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gszfbyyez.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gylrcyhtj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ggbttuoec.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gtntycnnx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gztcewtgo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvtjdrlul.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gccrygzze.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gdyeopnaq.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gychlxwyn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gqnfirvki.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gvwlskfbm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/grbjhiijc.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gscnstdhb.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gppgkvsfz.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gkgshizxu.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gpconuank.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/guzxlclyz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gvhnahiwq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gpiccxypu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gurrtvcws.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gcgdkxfzk.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gcrwakkqb.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gvpvsrufm.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gdayovqpd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gqphkfeln.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gpfdzfuse.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gzonmoguh.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gletwaygp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/ghfzpmkrp.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gicfwpszt.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkauehuns.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gbzkthakp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gweslnzvv.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gwcyuansp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gpzulcqmk.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gdcykprer.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gcebhdhki.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/geibqxlaj.sHtML


<!-- 参考信息 -->