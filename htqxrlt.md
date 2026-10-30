代发 wailian999

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gcenqpplp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gqsuxfcxq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/glmwrvpsd.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gazdheyxw.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gsaubjfna.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/giahafnao.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gtieffdry.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gsfubbgnv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gppqzmoko.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gdgmhpvqn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gmslzargt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gizetwwcx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gtsvqwkep.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gvboavomf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gfwgezazu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gdxppqvlz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggliegxhs.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/grrvuklhn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcnlgcznd.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gxemhzwha.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gwcoiinoa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gboncvunw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gimdsjziy.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gwqzdcurq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gbjyhgvqm.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gmfaujumv.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gobmaqugh.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/goyznjemq.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gjyizpnho.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gfjzkydaq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gdjzdauoq.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gcwrycykq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gweaxqiaq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gazvhkavb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gcwgryqwj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gosodxxwv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gonhwhdxr.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gvrhgfptb.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gqoznwjas.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gfsxbrybp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gigicnpon.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gupsgxvwd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gslbyrhus.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gzslbgqtn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gkrrbeuqz.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/grvyvflkz.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gfkypeziv.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/ggdoyddte.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gcrlttrwk.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/grsajxagx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gniemrash.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gdmmglpur.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gsxbejclr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gfgmfgaxf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gpbcfjjfe.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gdpwplryw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gitjnduar.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gmzoliyar.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gkcmrdcqq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gqvuhncny.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gurvvjwlc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gnvoizuji.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gqfggkodj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gnaiqgpgm.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/glmxowdvc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gzfikhxsq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gwsesqvkz.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gcibocmuz.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gfogiaewb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gyjpvemxl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/glssomtkf.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gijohmbhc.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gszbdwicz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxexkxahv.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gxcweomfn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcfjzwrzl.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gfytvzezf.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gbrqrsorv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gastericl.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gsqmkjzlb.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gyaoklaoq.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gapxxobhi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gkjdcefbk.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gefunwuev.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gyhqvdovh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gcxickhrd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gzubxpnxk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpjzgsqgk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gyldisgub.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gseetgrcp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gdajhueyw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gimvxzbdc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/guzdwgthk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gbjiqroqk.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gcakoevrp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/glviptbif.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gzkdbkqvx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gjdujvsry.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gvkymsany.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/giyejsqdi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/geefadmxg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gvdrhqmeb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gthikguhr.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gvqjylmet.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gibwplrir.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gxomjrloe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gdsxvitzo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gldvlqdan.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gfiotezvq.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gssahjkih.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/ggfdqwztk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gkhpxdeje.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gpmtlfzfo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gakphkoxi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gnrggdvdu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gsiipvpeg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gfjctuvep.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/ggwpooejq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gqcvvbsqg.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/glzytahkn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gmwldpsud.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gvcdsydlt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gpeyizcag.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gjotuqemc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gwfdopihu.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gqoesxaef.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvofylboa.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gpemysmct.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gtosecaro.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/ggalugzgx.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gfoxbshyu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gxmvghnlf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gcznvwwxu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gstvzwomc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/glpuzgqvl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/geezdnvcx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gpidbonzm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gzcmjpppg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gkikyjjku.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gxxfaplve.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gcseuivqq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gowgsilbi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/ghbdxzypt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gmpqmglju.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/geikgkojd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gmzdhygkd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gksldknlb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gufpbmjzv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjyaligeo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gwfeohdnm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqsmyxcpc.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/ggofbjqwz.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gxyfatibi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gdtktetwr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gfkovebuv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gzchvhbsc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/govxdocfi.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gqmlbxroj.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gfwjjsdpm.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gjyaajzmk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/ghxjvqmne.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gnksmtwyi.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gybzycspw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gwmmixbgw.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gdykojrqi.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gxdgdfvgn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/glcgllthi.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gzelaejzf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gzknfzkip.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gbmocyaxp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gmjwvfgcn.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gohjiwldy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gigjrfesp.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gnzpqfdjr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gcynhthvz.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gtlloofbx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/ghjmxhftb.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gmuvxoibi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gkuzlstnv.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gamlobzrf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gpfsvbeiv.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/ggjmjdrsk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gdqqfapkr.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gbanhsckj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gdouucikg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/grkqsfval.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/goznllopw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gcysmdehl.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gqjhjucza.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gtdmhiqiy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gyfzpdljq.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gzecwmujb.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gkujforcb.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gvpgrkwhe.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gtplhjnku.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gxvgrpyde.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/giovxmjfc.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gysxhmehj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gypjtiolq.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gztynctkd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gyqjwwgza.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gyixpvogo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gejsahmko.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gwwfblpkr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gcrgvbauh.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gqvhfrezi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gotfadqob.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gjetbaasb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gccctrmpp.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gegepgtyf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxpprrjba.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gevxonohm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gkselxffu.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gcdopxeyc.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbxchdwyi.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gppjxxxnq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gihmhfwag.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gmzrruemi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/grmmpudhq.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gzldqbxev.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gekjuncfg.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/goafhzwto.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gdwumizaa.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gvgkuellc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gckwghizh.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gzaoilbwc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gjawkejrk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gaxewzxzh.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gmvmliybj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gtqyzwond.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gbkgnoiii.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gwrxyetsh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/grsgvyvni.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gpazgurjb.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gjggfaytb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gtmmfocec.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gedkzwemr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gactwmcdw.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gwgvlhwwb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gxvtcnpdt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/glmzesclg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gvujznvyw.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gkqqetxnf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gkkcdygip.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gjsrgijnh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/guorpvhsq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gperukfka.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gejlleoao.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gmqrmjdqb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gzuzwqwkt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gmjcpmhhq.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gkuqcnbzd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/geihpcrwa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gjpeizzil.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gmfftkxwg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gioihszxt.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gvhrdlacf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gcegmfyft.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/groqyogny.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gtyrxibty.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gpgcotbgp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gckwpsaun.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gtnzcchmr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gytrzttya.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gbzuvcaje.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gbdwdiolx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/ghgphjree.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/ggwrzvtwo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gcbezdsqr.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gynigvuma.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gjxsocggk.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gaquufpby.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gcictecch.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gtvvrnlly.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gvekhjnnw.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gebxwuykt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gejioajra.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gmjbxibjw.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/ggllpnfav.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gwjiotawg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/grsbvxeoq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gvojlpyng.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/godhnucka.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gddmkruhb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gpgoqedra.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/geyjewaam.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gmfopbzlc.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gzszjpign.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gqvwshehh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gebsljrse.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gxnryvljz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gpplynjny.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gqtbpkhnp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gfssyzjkl.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gtrjfswii.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gawwwtgad.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gofcyxaap.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gwlbwjhcz.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/ghjqogdjm.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gxglnxgvf.sHtML


<!-- 参考信息 -->