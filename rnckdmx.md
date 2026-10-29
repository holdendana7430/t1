代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gtnriqchk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gfbapwebc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gdobwlngl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gvbljeoid.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gxjbnvqul.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gzeimpjiz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gjdjzxckf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/giipqzcry.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gadgdmomr.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gelxnrixr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdvbpelka.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/ghtnrkblv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gtxfdwnyv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gzrxlmmue.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/grufoxpgs.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gbmhchxjh.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gcffqhjju.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gzbkncmnn.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gawxyyrnp.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/geffurgwa.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/ggaasxlxc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gkrrkgoug.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gxbjaiojw.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/geeaiftwp.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/ghbrluwlr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gawcyietq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gasxftbkf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/glkeapklf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gyzstzvtm.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/givdiwesj.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gxnghlycx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gokhzfipi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gmvkyssio.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/glfjvclfq.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gifpsbdwk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gzopscadt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gbvtfbrku.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gklamkkwb.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gbrlbpiws.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gbskvobhf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gurwmwzaj.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gwfdrgxkb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsxneefts.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gsairnkgt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gsxivhaof.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gnotvlbzk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gasatknpg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gdwnnghoa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gdcpgxmmd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/ghstxayri.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gpnhzqamj.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gqafmkwcd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gcpykuosl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gbhpesrna.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gokfgkkiz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gvkijenbu.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gqauoeoac.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gnboqdudf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/goeydplku.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gartolffc.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gsgizomzp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gifxbyuem.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gpdjzdmel.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gcvebpbbo.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/giopquxoy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzsrcrkii.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gpvkyekbt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giuqxapyw.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gejkoloiz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gzyfjuonz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gtkdsvtul.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gjxnnifxt.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gjyyjjybd.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gjszqfyqn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gpawjkdcl.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gpfhmplmb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gxhlhvzqn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gsaolrgxp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gxsnfgxer.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/ggneroptf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gesrunurp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gsqogjxhm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gmvwfjzat.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gbwbcelde.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gfugyezdi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gdbujsoar.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/ghexzvogg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gsznodutg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/grlztlxbf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gxweoqqqi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gyqnvwvhw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gvccunurv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gsnbjsqty.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gdmklsqzw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gourgtwip.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gvnmsvbgn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gcutczbty.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/grizrskfk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gwxbkjbhf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gbunteora.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gijzgaigr.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gsnoywmhi.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gidgjqxui.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gzpndcfey.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/grrdiykez.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gziebwoxj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gqwmdghjf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gasddzezv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/guyjwcnrv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gxhbfycds.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gkrbskrru.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gjfctvqfe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gssgzbmve.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gzsgiflse.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gotnuxbxj.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gxvsusjwd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gbcfysrte.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/ghnggbdtc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmjvuyazx.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gzszczjkz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gpkojqmsc.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/grqgvixtv.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gbiyyovdh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gpjjhtdqa.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gxdqzryxi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gfdgoszao.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gtffiahql.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gwnwbykla.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gpgonembs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gsakxkmqa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gpmvxuihk.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gbqcncvme.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gonzmgmlp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/glldufect.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gkgnvmufw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gslnrlbod.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gvdgypace.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/ghmpayyky.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gtqvizhba.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gdkmhoqsf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcztgkarj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gdzechfqx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gemvhbjog.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gjreslypl.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/giynsaewj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqpbwjfdn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gwcxggjqg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gzfxxvoat.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gnmqfwkna.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gyvdchsfp.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gnhqyhsou.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gnnuhwuqw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gvjfvxjhb.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gsrtllfeb.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gnntvmieu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/glahiasca.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gvyvunpkn.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gjjkmzuse.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/glxuagltx.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gmhtnijln.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gaeesuzxb.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/ghrudaqdi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gwfyqrmli.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gyftfoicn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gyrlonqfg.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gixevqgbu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gvffelyxw.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gttggtezv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gdwrcxnsw.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/galksoyxx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gsxockqrh.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/ggxaejsbw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gncroluho.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/glmmozjxo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/ghfaqhqth.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gfnrpuxhd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gfmfyubfy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gnphxsabb.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/goihsrjfx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gwuybdzrx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/grrbscxwi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gdionjtmq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gtexxdvey.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/grtooxqmx.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gftvzecpv.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gxpthqvve.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gwfxvlmbn.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gkiocnmdp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggjzlddob.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gltewgqwk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gxlieeowr.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gnrdwaudx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/geexdyfao.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/ghinefduz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gdqwlxpjf.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gxfzwhtjm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gybihtebp.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gkxruxeeq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gnvhchlhi.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gworcrzja.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gvaydoroq.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gvolzqjei.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggiifgggq.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gojgyhtxk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/ggforenws.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gclualkvy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkopttqbo.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gxgztndux.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnxqazaxh.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/geeukweun.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gnlpktpfb.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gnoyngmlh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzavgogsw.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/ggwklxfec.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/ggakmjlnf.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gqzbxrhse.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/ghsqspzna.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/guvtswota.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gddjzrthg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/grftzsdmx.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gukenxobj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gbpvvzafo.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gmmopfthw.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gebimkvlw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gxisgtnsu.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gzehfovqt.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gvqeqerzy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/ghrwwonno.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gkqgpnbhm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gnlenjxwz.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gqweywisc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gpdeboccn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/ghjhkawva.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/ghzpkwzvl.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gruzcapuv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gekffhfxz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gvxribzra.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/ggnyozmpj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gzkrgrwyd.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gxrrvfzbc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/grwbageen.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gmpszagif.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gxnueztfp.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gntfigsdv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gwbhrwjdu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/greqkdgoo.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gitzsetpj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gfbsaoxua.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gohwjebdp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/glyplprcc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gfoxectuf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gmhbaxrya.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gviznvdkw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gafdoxlio.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gpsqfijsc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gggxkalrv.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gcyoefoxd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gonbrpeto.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gxvghecff.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/guqpsnkfi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/glpezxygn.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gyhkkifbd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/grxfcunyn.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gvagjgynl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmycoppfi.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/ggsgmvafa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gcbdfohui.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gscmetehi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/giljemjvj.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gyfxugajc.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gkhtmjyrk.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/goqwcbdkk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gyhckllzm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gvgplylhh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/glukyucqs.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gmcarydnx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbuhuckdm.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/glyqjdgbx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gnsompouw.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gbdwjnmxp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gwkzqvnqb.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gxbrwlcbh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gehzvjzwv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdfpflwdd.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gzbzifbdz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmyrdnnyk.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gktixivcy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gcbuwfuvq.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gjsgsiuxt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gevfpiunt.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/genmohvbg.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gbidnnose.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gkhddpczf.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gyabdghta.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gdqjtqhjr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gntngploq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gkjhetlfz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gehltotvl.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gkyovdppu.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gjiiowhot.sHtML


<!-- 参考信息 -->