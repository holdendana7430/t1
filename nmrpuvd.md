代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gzhkmkjut.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gkdzlujqi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gjbvxmaxp.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gofloullo.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gtvakrzry.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/ghbbeeiwz.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gucukplgf.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gxpfgecbs.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gwnauhbur.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gngqfccbo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/glusoqbeu.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gkdgnpnyd.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gllfnhomt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/giuhqlemb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/guriofrzl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gkpsgafrv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/ghrfampol.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/ghapfruyy.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gobhlajgh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/grloqlamk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gjqgbuauc.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/glzqurljc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gojajeylp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gcprggosj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gsdguetuz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/grbtldekm.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/grjznnptu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/glzivyvnu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gchsmnbai.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gkxrezycf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/grmhaftmq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gkxgoqeff.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gqeslqvhn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gfdmkmyym.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gdyblapmx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gxwgusqmp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gqjmgrvdi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gothzicwb.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gjnltgmso.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/grehzytkf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gsyojyodw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gtqimnczz.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gsuvjegaw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/glkcooizl.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gexblkepk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gbxmgapol.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/grebjoaav.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gdmckqdzp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gnqduxxpp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/guhlejtbf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gfefefret.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gpoyxdwaa.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gfpfnbjnw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpmkoioje.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gxjmiusok.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpooffpyy.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/ghwgnzvdx.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/guguxciix.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gkspziaai.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gqmldpedw.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gdphbgrtq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/ggipcutqd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gjbelilhf.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gyonwyorg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gmspmjfpl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gytbxdhjn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gbbgveair.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gqqcpkpqz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gexpqkgml.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gvdpyuygm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gkxnimsmh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gmlugucem.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfrnhtfls.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/ghxmnfpba.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjyebvllq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/glxbqsdov.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gkqftfuqf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjajqjqso.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/grgpcrhto.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gpwfxtyoc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gruhgdxwy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/glsszihhn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gznmbroyg.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gisvbrlfv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/glvcvznji.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gjlgxvbfk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gacgjccih.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gwtrhhayy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gsxrhsgys.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gohalcoug.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gwpkfwimp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/grtkhufiz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gictnkspx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gtrsbaurx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gmihlbxsc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gyikkhfmt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gzaphoyba.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/guzthtrlb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/grkgyjpwu.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gccqvxall.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/grhuloyho.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gowsxftdw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/goknxftjr.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/guqlqnvsx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gdhbkdmrf.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxvhqxvaq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/goskmirlj.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/ggsauriwr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gwufaowfy.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gcxvvbpfw.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gciwkzeau.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gyflbznoy.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gxrzenpko.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gyrynvojw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/ghtktfdyp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gnxvyffdf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gjjsjdslv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/grjzskcft.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gbjdlqumj.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gebjibgvd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gjquiurtu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/greqmeboo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gytridjmg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gyocpunwd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/ghuhfvyzr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gxuktfiad.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gpseftkiy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gzthbpncb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfehhvfov.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gptrubwoe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyjkiyybq.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gydnmgtrr.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/goeqitpho.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/ghijvesdk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gsovjoxeb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gbxisafic.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gfatmysno.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gutfogfim.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gabypkabf.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gooxbiklv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/ggjaduawz.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gqrbukhwm.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gfrkviplc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/grzigtbek.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/ggpzbakws.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gxbcgblea.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gjixfndha.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gmsczggsi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/grtdxkzvg.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/goxolfcgq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gvvragfsx.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gxpkslbuv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gqyxyahhx.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gauyjmnsy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gppckgmlp.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/goenlijpv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gwayedvbv.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gqcofaqpw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/glywrfnyy.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gsrpdbuyv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/godurpats.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gsnvtfgjr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gofahqcsw.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gvvkflfjb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gfobnqqvg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gpmpaegjs.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/grooihuli.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gnccxhnzr.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gjzoaymlm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/ggkxhldzg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gvrtqkjjf.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gosjhoxdd.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfewzgywd.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gbdjxoagk.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdtfpfxqr.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gucmviuky.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gvlcpdrpc.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gnkatyifu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gcvowwmnh.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gtnhbnyqs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gbomjafux.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gsbsquxjo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gxnhhepfl.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gqrzevyez.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gmfxistvz.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gayhmcrnj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/glhtdeswa.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gzyjsalef.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gpavaepfs.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gbpmuaipw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwvmwfvrp.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gtfcqwvzl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gbrfusdmo.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gktvvmqja.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbpidjklj.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gjjnibnww.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvcrjwxbb.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gzngmxnxh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gojwbltnu.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gqszaodsl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/glthovgvg.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gezfhhfuu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gykanhnie.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gjoqxdktp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gbpxxyosp.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gjfrduoeu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gerehbieq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gqfzpyoab.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gvjpxymyl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gacrtadjd.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gpgcrdhcz.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gimbwulcf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gzvpcecfx.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gpjtnabid.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gpvirizlw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gmskmjbcp.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gayhgools.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gzazkzoci.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/ghvjidnur.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gpnssshls.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/garkeyvtu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gdatymapk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/ggqfrnybk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gzjphlned.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gcdtbkama.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/ggjqgolbw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gfskpsoqc.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gfaoazihw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gpihyuhqh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gcuisckmg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gdqmpwmpg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gbdsnhxgw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/ghvyciyzl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/grcklzvyo.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gqvyrsjld.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/ghrxetrpl.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gcvjadxgm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/ggeyiuozw.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gpgmrjhdt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gsdrytkxz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbsqccysx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gmclhzejh.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gutjmlwfm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/ghapusulm.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gjwzmfeil.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gyxixihbo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gmeepivkh.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gsfujxvcn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gvqpgvzav.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gxqrxkssu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/ghhxxyaiv.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/guevcurvp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gymqdgeby.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gjxqpznrw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gokwtdgxu.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/giiyhlonh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gyftufqyb.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gactoydvj.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gevcadzat.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gnhnryfyv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/ghfmqdira.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gftwfdztc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/godklnlme.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gxewqkebl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/grmbdodfw.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/ghtblczqb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwgsbpvsz.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gbparpjzu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/guqhyosay.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/glofubfdj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gtdafdrme.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxqfqxocd.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gyypzmkav.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gaxovstco.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gehociupx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gpitffxuy.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gvbaknjdn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gohytfbgc.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/ggblymjet.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gtonmhisi.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gidpeuqro.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/golibrsqi.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/ggjuchvnt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gpcgpywoi.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gvbfmiuep.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gkxzlhipn.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gjvgwovey.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gpsxnrvxp.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/giwypozup.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gvzbtgdmw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gkewfpzye.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gibqeysap.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gcmxszlqj.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gfjsyzntp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gwoworjqs.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gvzocqddj.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gtlaoozyr.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gbndbnmwc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gcyyrojjx.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gphxlmebp.sHtML


<!-- 参考信息 -->