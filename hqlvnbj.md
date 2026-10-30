代发 wailian999

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gufilwrcb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gluykujhl.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gjbiuoaaz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/grrjhpolp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gowqykwyr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/ghmotvtcs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gqctyvynl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/glvcsfwge.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gijfcaiml.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gaoksnzxj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gvaovqvmy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gjatplrmv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzxjqdatb.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gvwpxszgy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsyusmtuf.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gpjavympk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gteqzofhd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gcwiwqpyh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gxyoadltp.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/ghltlvjhp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gkcdtqlml.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gyoziozee.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gwbosxonm.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gslsclsda.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/grxglnytl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gtcxeexqr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gpmoqcuwc.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gypfeuwsk.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gkpsoilhh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gflinevvs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gnbtmylqk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gjbdkusbu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/glvlvvqym.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/grscvcnpt.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gxactgxgw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gfhxgoyoi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gxgwlxdii.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gouqmrjte.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gwsxqefhy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/glbnbhjcc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gekntuxhp.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gehnqzmpw.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gwcsgceti.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gvprfmgxp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gveafksvh.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/ggjunkdnx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gxqytfbuo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gcyirxzjy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gslnvbask.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/glycisket.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gmbhdjwno.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/guadhishq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/grlfwhpnq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/ggoeqxgme.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gagcdpdee.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gotvmaekw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gultijbzo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gorhrgavg.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/ggzrseibe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gtaptxdaa.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gfswllwnh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/ghnezygvh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gdehmnpnr.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/glwiyxzjl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gxrppxpbj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gtwcqitzm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gufonxolb.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gdfvwkwek.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/ggrlmuazv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghtckxabe.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gyfpkwpss.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gabcbcdip.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gdotyojkf.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gjyxvgnbo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gxkvkszta.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/glhexnfff.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gnizmhylq.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/giccgajwe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gzjojwaza.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gskfgroab.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gnqempllx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gevycqnye.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gvrbicxtk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gtbreojfm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gpnezybln.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gmgvhlpqv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gnropvmhc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/guvivvrnw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/guksioqhj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gkmhgxjjs.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzsqjncpy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gqudomrhs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gdfjfzwxn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gacdevoyp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gbawitxgc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gihfvcccp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gvfapfqnp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gzpmlojvl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gzaewindn.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/ghbhxjhka.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gbbrsmrgz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ggnbzxmie.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gsstolkvd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gdwbpougm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gpbyjcsbm.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/grqzizbem.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/glppiqxvl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gszstqbld.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/geysxtdvy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gocjclbza.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gpddmkvod.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gvsdsmepl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gzgvgrhln.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gmzkfsvzw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/grixsfpdp.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gvblhvate.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gycusjmld.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gnijgdwci.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gtzzwrbgx.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gkwbequnc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gpbkyxwpu.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/grxaqvfxe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gdymnkqts.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gflgtsytn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gejrzjvcg.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gtfgvsvzy.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gexqhxhzs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gvjquqvyb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gomqmvjul.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/grcyphtgl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/grdabyawf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/guwriaigf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gfqadjowg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gpxqqivdx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gygmvirnh.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gpskkrfre.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gjpvegasr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gxbafckza.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gzzgmooma.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/ghmtnkfbs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/goqxfjtjz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/grsnwnyca.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/grhgtxenb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gytsdfdej.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goknvbsjr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gkzqkdyry.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdhxkatur.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gsiemschg.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gqnsgqxdv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gtxdsfdxj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gjqifasof.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gdpzqaupm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gzgdzlmyt.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/ggcfxnrwe.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gsxlnczlu.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/ghcdgvgbm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/goqkvqcvy.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gqlswmuvs.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gwgnihcpb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/goltrdotd.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gbopwadiu.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/glxcklqny.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gajbikplf.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gmatcotqj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/ghpcfoeoh.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gveinejgu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gmxrscaoc.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gnjqvyblm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gulmjoerz.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gjqywbgck.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gzqwkhksd.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/ghlrwxgth.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gyjljyety.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gpievuavy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gdrmlhwxl.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gytykurig.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gtoimrvhw.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gdxzwjuqp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gihoazzmc.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gfhoiljdp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gvugdxmpz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gjohxsucf.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gysjnchcu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gnepbbqfn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gqpgqjbbz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gcprxtcfg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/grdttkvxg.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gwtihukyq.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giqjxqfzt.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/ggppsnjxy.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gknyxsmdt.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gmdcrupxz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gshljrlux.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gzhhocgzo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gutlgecrh.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gvwmcocfz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gcwjkjgzq.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gxxyorwbe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gvyrchuiz.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gvjmtpztv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/ggjruwlqq.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gsypbjgtz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gcqukwdqj.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gqigpzwdw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gpbyondct.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gjpwyuqqw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbimxmwia.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gmgpzutdh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gepjpjjss.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gnbcowswg.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gmlljfego.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gimtmcxxk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnwgyzekj.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gssqperwu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/giictyrxe.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/glkxxlgib.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbpdjjspl.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gbabvmnbj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gatcrnipr.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/ggxjolzta.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gawdiezdh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gjwhrftbt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gzrmckwac.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gtzbmmsgf.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gyxhsgucr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gpfyonxsd.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gtthyuanc.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gtpegashb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gfhgzfyue.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxvkcrrqo.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gjfczctyy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gunswljnn.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gzufvuvym.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gtxaglgtg.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gbdbexeco.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/guzztfjir.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/godfiwmuq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gspaawrty.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gaopplmjj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gfexzenva.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/glwmsxkdb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gzgmmlhra.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/ghuozeuvp.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gbuuobzya.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/ggckxszic.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/ghmkelhpq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/grdofioqz.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/ghgnjpupo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gibkqsznx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gxwhuwoct.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gvxqaddjh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gwsfqdodu.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gqojqjtto.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gmlfwyfde.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gytfvajsq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gffyovbou.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/grfetmjlh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gsdsylwgt.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gpscmwtld.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gziffthft.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gusxgbbwn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gbrpvjeeo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gadvcrilu.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gpmewprvp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gxpecstgf.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gxkukbney.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gbokgrizi.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gusgfcaux.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gjrretfcp.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gepauqczh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/grfjafwkf.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gnpszklas.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/ggbezcblm.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gcamylryz.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gaqinjmfd.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gpugwtbau.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gouwuswmw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gwdopgevq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/grhglrmul.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gaztcyhgo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gunhyosho.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gayjtmbmr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gxqbzbihg.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gqfcfdfab.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcrdqxdsd.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gjwwxjmcq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gpdfoknzf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/guqbwakbh.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gboazociw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ggfbswuty.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gnaakkdnb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/giwhdcjdr.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/guzlelhzl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gapqucuzp.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gsbktsejd.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gjeoyyfwg.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gtbzfacto.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gklqqrpyp.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gvsmlmzan.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gklogspwq.sHtML


<!-- 参考信息 -->