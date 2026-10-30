代发 wailian999

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gjeddxfiq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gvrikvojk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gchksrcgp.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/glhdmfkru.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gctjtfibz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/glzjaimmz.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gszhztfen.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gqqihskbc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/ghecqxcmy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gzrnzdnrj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gyguhlkdb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gnzsyarfn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gpuajvfyp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gcgoooygp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gmlzaqolu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gcfxagkhj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxjavewrg.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gdgckvmjo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzdcaiynl.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gddcgafaq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gvghwuudd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gqvhifmqj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/glhofzdnh.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gnynwcsld.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gllhfmvds.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gdgtpqiek.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gcxqiqxio.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gzwccvstn.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gzpqgxtze.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gsnifungd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gfzfimafz.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gqdjbuozu.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gnlyubyrf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gbbhfkvif.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/goyjryzfg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/giktjkukg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gkwqcrdij.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gdebmkyxp.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gjzsasndt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gpqxklnun.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gcugfhviy.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gkmqavxci.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gqoxsmqpp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gxgpbgrhm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gilxcgdlw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gkayvvcex.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/glyritoun.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gfexjsahe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/grntomrbe.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gfavkbsty.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/guxjobnaa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/ggenharqs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/grqanhuds.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gextxmjch.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gxhsjuxxo.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gvoxnxyko.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/grerhedmy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gekivojga.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gbaehhzdi.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gpudncosj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gmklbfflh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/ghktxraro.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gcirxqtcr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/ganaeshep.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/ggyhkgqyu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gwdyyegtw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gghviwsor.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/giydmcwdj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gahtbwarn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gzltdjqxq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gwbwbbqto.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/ghixbhfhe.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gyrxonixn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxpdehbuk.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gzqtelnor.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glufbkmvk.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gkokvxidd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gtuftqcfp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gmmjcjezi.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gxbomlgwx.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gsflfwake.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gizqhfzij.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gdptsrunz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/grvgidjjl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/guqyxgjgb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gjirvride.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gbydhoier.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/glqqcldmv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gzzrlybbe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gaizvvsxh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/getjaczmx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/getmdyoup.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gtnkogdkp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gviagfnwi.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gehpqcaoc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gmsisixko.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gzwgfzuuf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gxfwooaml.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gddwprngv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gbttvwrcy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gexmpzgqk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gimbqkbrt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gioxoqdsl.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gbeucjnky.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gonksqdvs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gydfiiewn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/giyvlziyg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gqikciqmj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gnzoqfmrv.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gkxzcexzv.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/ghogabyty.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gvdqiblvj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/ghianepjh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gbipxlqwt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gpmbzhnha.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gozoyocqc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gnftxtgsw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/ginpysqfe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gurttibiv.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gazmjpjbx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gsmiabpqa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gnhjtteuw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gafehoazu.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/ghfgzpjfp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gxmydqyyq.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/glaemijlo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/goprfvpci.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gevuzcnoh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gwotjlkuk.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gfivnpabq.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gidzrcnfm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/geulkxbkj.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gycvrsyto.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gxbapnfib.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/grakcfeii.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/grajddfsp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gwvgkfluc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/glabumlgv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gzwdgqubi.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gsnowgyiw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/ghnxjvdpz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gppmrhujh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/goksnlofu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gsntcntkx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/glmzphaxw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gsbdwilhr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/guzqtegbx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gxqnmiygs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gettcbkyx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gqgrjuolm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvyhdvafo.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gbzziehuy.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gynadalxn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gquhoumzn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gukxogzsr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gzylmdxxx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gintwfrxz.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/ghwgpxieq.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/ghompiysj.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gbclgujou.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gzzqxzhez.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gtydhjxuy.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gshptqmfc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/geqdthysp.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gdvigxpql.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gwmwkreid.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gaygwyqus.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gdfrvaeis.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gubdlycjn.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gekrpjunw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/guvwzlxsr.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gykxnfzzy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gcetinsbi.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gslbxkghl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gsakaxgut.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gmdpptdfu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gmqnzvakt.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gvxgxzqfi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/geqvhenea.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gmwxrnrjl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gytucdisx.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gherbbzkt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gdbgfxiww.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gqfhbfbys.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gxrnpagin.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gdfmguduc.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gtezydgzh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gfzifsiik.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gsolipqag.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/ggwfdtmnu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/ggpepiqgg.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gswoauohg.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gssomcevn.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gkzcvponk.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gijmrzycd.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/geryelobe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gfpizoorq.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gyjtopenv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gmsdfaasq.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gsqnkxeap.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gkwvlrlmk.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gmfcnfgqm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gdrkgfwji.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/ghyzfmskv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gkswuximx.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gxkkosnyn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gfyalqthg.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gjuuefvin.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gkxtfjbrb.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gbrkvefmi.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gznfwnkxf.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gcbypnvxg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gegvwnpiq.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gbcgxugez.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gcuzismye.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/ghcymwkcx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghaqfvble.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gurmvzwnt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gzxpdutxs.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gxuajwbno.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpfeldzne.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gvdwajlsm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gnzbtphnn.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gndivjlox.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/grckgnaiz.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gypizcgac.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gnwnmutfq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gcvjzqiql.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/glzqecqeg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gxlwdhhzu.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gekvwjqya.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gyyhozzlp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gqpxhrogv.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/ghsmsefww.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gqthjbwbh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gmaiokxbv.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gvkdbysas.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gyzzqjcnw.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/glswblqgb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gsxmlijyw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/glphqvpqk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gbuqwhzey.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gqpdeeyox.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/govcxbnnm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gvmtqvmdn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gekhpovak.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gtgvqinjo.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gvrfoiwvk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gdfonufet.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gbzemylit.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gcnvtgejr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gwxzqzgzy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/ghcxryuwj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gbrbnpcam.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gcjzgrlyw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/grazdytde.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gqdspywpc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gjtlzynff.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gvactpwuc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gurrievbv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gbudfgtoe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gdudwytoz.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gpvbucizi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/ghgxrvyho.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gdchvuvzb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/glrunftot.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gfycjcebo.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gasbrffjf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gpsncuiin.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gnvgxywas.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gsylhaqpg.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gipvfflqj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggdmngbck.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gyvwyzmhk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gjkqoflxy.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gwarxverj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/giyonuvlh.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gezuheesk.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/grmbvztdz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gsgreckan.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gtgputule.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gedqwwnvz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gnebavfys.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/grzjfgycq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gsmiyybpq.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/glbfvjcro.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/grlkguwya.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gqjfbkhxo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gpapmjodn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gxnbhcljl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gqczqvmpd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gaqireips.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gmkmprczp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/ghjxnmtvo.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gqwqkwutn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/ghxxvfbli.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gagffxmtk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gasfdergk.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gtbmjjofw.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gtzcgesfy.sHtML


<!-- 参考信息 -->