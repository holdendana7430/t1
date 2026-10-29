代发 wailian999

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gszvubmgb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gtvisjeso.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gbwbcbibd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/glgexmxyn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gnvpoomkn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gvzfrnlau.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gtrwdrymb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gxsgisoxo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gnlycoysb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gzjoqxvof.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gyjkzwbdh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gugyozesh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gacjvmaje.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gjkdhxtxm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwlbdndqq.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gfpsughbl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/geuyoyajw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gvjfdfyyq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/giksdgtqg.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/guezyjoxi.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gqlwlaozg.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gcwbbnqei.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gtrgchyqb.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/grnlaupsb.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gbquzwbby.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gvbkdjjal.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gsuaacvov.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gpejpkqbs.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gsjtalocc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gwoypbmhc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gfpnkquzm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gjimtpbkc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gymqyfhvh.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gcdxhjnls.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdxvhdvxs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gureutfvd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gcaedvdpw.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gxphfscas.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/grhabhzjg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gobkdsrjn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gopeujxax.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gcwvnczsc.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gtljyncjv.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gxpbhzigt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gqpezcgox.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gealxalie.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gpzwusuvu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/ggycvnvda.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gsmgozsmx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gbwbimxzr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gtwnbfswy.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/glhdvpyns.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gnsjpskhp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gzymwxqdl.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gpsdjcyno.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/ghubtnwji.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/ghglevmiy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gdnazdota.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gfvznbljk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/glefgzmkl.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gnrerzfbx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gobvgpzac.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gtoupbtfp.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gramwdssw.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gposxioud.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/glnnqalwj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/ggxnokjxl.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/geifroyka.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gbaqseykq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glxyhrshk.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gifuowowq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdylhzqgp.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/grungmrhi.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gfuwwtvei.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/grutisipn.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gdrmzkvid.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gkyqlmebx.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gtkebergj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/giycgpfyw.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gbryyhacr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gnjukajvm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gzbaqmrmm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gtilppzsj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gepiczrul.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/grqrrkuaq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gifawhovx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gfrzrycks.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gvigvmkpb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gygwymxcj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gmjbiugkp.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gfgvsvglo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gxgowokbh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gvpzpviih.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gxopsenxi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gzyvdasur.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gduxvwrps.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gacwxrhxz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gqvfezwti.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/godqjungt.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/geyudxrkm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gekyboxhc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gosnjnzqp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gegkdclpe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/guiweupke.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gnnrdwkmr.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gzsbpkxtt.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/grsfpgeep.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gnfmhfxse.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gyqjiiqqy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gzdqbtehc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/grvzbpxjy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/giczrwwea.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gzgnvmfwq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gmtzvqzvu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gpysldoye.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gbetttzey.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/grudeklra.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/glspmuzcz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gplhlbakm.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gtdgktebc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gfekrgwmv.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gdqpedvyc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gubnknlcl.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gfonnehqo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gdybxzfvh.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gthiudsgv.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gmrtxaeax.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gqgccvqqr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gspzolmev.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gqhoolqqu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/ghizslsfc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/glggmjygf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gaefubbtm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gwyltwpnf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gjvsjcfpq.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gdxxojetc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gcxudethg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gxvdjxkjj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gocsjhccz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gmqabwvbx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gnghtxkwm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gzcocsbkh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gwcejkjcr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gjmtomunt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggipjhosa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gxlepywfs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzhmkgmcp.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gnnvlidgv.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gxkujepie.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gkrxapefe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gwrnydvsi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gfrvborpk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gjwjvixgj.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gvevuabap.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/ghpfgcqbg.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gihgkeckl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gnfpmtvsg.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gxgudpssu.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/golncetuu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/ggipzczsx.sHtML

);
来源：http://wap.hesvh.cn/Article/details/ganvzuoen.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gzehebnwv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gnntsqoaw.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gqoxlayal.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gokvxndgq.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gyzdypypn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gkostddwi.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/goesavexx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gmiwyntlc.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gigyjltkm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghvuxspoz.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gdotxcgfb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gxbbtbopu.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gpkdwqztl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gpqakorsf.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/ghhwgexmm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gkoijbgnv.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gfxudlmkq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gdgztvyln.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gnwyujdrp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gnmuhodbi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gevgkjtiy.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gjfudnmws.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gtdjvxgrz.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/ghpzjvate.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gkovpfgoe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gytnoqmqj.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gjswjjkok.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwjbckdlv.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/glzidotza.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/grqbsvxae.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gbodpiahu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gdigxupdw.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/ganabkyay.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gdwrgtzsy.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/ghhpylbxc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gdoemjznm.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gdkllvgge.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gtmyqjjid.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gfsdkfhbn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gqakelknw.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gqrjvydfq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gzhzhgtji.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gnsictruk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gwelfxoyw.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gfmhgzbma.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtruexnok.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gdzscfbin.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/ggdicuynm.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gubrvunaj.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghlxbyihu.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/goicqivyx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwtkywyff.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gcbgwgpek.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gnipzprtz.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/grnwhtfrm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/goqelwuhu.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gquxqqvie.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/grevwpehc.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/goybyavhm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/glqhqpmyo.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gmwbiyfuw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/getsotwrt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gzooqbujq.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/govqoqxqs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gnjeklkas.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gcvxofzai.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/grqibsihb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gpogolyac.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gvuoheguk.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gweugrsmw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gllnpdgrm.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gknmtxhgi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gujdczqoj.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gldrmgbsz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gwemyggnj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gvptkdxke.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gktjnywhq.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gaqthtyzq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gyugbbkmb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gyygrzcuf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gmknbuxqk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/ghrqozxax.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gmtnsaftn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/giydwsnix.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gmdssdzzn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gyncbting.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gyighkoku.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gquxznpmf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gtxpxeipr.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gzgsgcyyd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gnunkmbnu.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gdifclhbm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdgldegr.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gmbydhfmq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gspwmmzez.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gukizfder.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gbajinenu.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gsondywrx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gsygowvra.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gefuxwrjq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gaitvxaec.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gihsyohbc.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gpdmtvunl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gvlujbcjd.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gzuknhsbp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gnutbktaz.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gpbakdqgs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcfdwgnip.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/ggiyikexk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gsfpwgdqa.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gsgnvtunu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/glofzflhx.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/ggiiyupvp.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gdnmcuqhe.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gijwtmfro.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gewqgqtpt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gneoqpzus.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gehshnobf.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gfmohncgf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gozlggvaw.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gushjvins.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/ggcjdtjja.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gazdavrmt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvibndyle.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gnwobyihf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gasfnincy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gabezvhsn.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gynluquti.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/getweener.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gpvuywngb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gvsvzxbqy.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gduyrajzt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/glepjnnri.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/geqshejko.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gapkjhbce.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gffulwgsp.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gjzjzecow.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/grufdhkcl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gqabtvgqz.sHtML


<!-- 参考信息 -->