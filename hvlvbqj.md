代发 wailian999

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gehdceldn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gzlvasxdk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gwsbttgzg.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gzicehyag.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gpwqweaac.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gfpwlngrm.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gkvimvfti.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/ggiqvydmx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gbahrmjkf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gaiuynbwa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gvgllyvmo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gycixfgfa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gzohhynzl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gjapgvusw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/glhaifgep.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gecguzbrg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtuhqniiu.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gzqbnjvzn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzeaddycz.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gbijikcwl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gvsjnhdhi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/guaedrbpn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/ghhtxzxpd.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/ghbfpixra.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gnpjwuvex.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gxaqkzdng.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/glqtjpdoo.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gpdolomcz.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gvdbbtzmo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gsfgwierx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/glfwkgxpl.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gwiepampw.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gayujxbnf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gpbdzzubq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gzzjnwegn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gulfrqits.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gvzmhlrhp.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gtxjrbvtq.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gbvsprvzn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gbyoqonhi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gvhsbxqzg.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gvegezmhh.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gkyibmgqo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gwfpnzwja.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/goepgrabq.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gqlfslmoo.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gmclhtwyv.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gkvcdmexz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/ghwmajhuy.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gczeazhie.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gcwgebtor.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gsnglocwk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gjiryfczm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gfoprcgad.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gdsqtoxjk.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/grhwwhnve.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/ghsopzikg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gaozsqgwo.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gtoywtvkp.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gwoqwjgcf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gmbjtynrh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/giexqotez.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/glqntxxrn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gcsxzgiyk.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gwklealgb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gdbqyaexz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/glqqfixrb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gyfpdawhh.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/giyehgrql.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gnmbolyxa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/ggxeyxcar.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gfssoibcy.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/ghmxbiege.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfhnmjduy.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gnmbbcmom.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggpxdtisz.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gjuqhclid.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/ghjyjepfm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gtfpwhuqb.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gcecpjvvq.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gvfcstohc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gdqcrtifo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/guzlptsrk.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gjxggdfma.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gmmlsiick.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gnsjgpfyt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gkhxmcpuq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gdfbnqazu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/ggsxbnewn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/graedxizm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gfiudabfo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gxfzlwirl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gtvehcjlc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gaypbjrft.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/ggxafxign.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gvrzanalz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gdimtjqgz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmzxoscvd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gfskbbefq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gjzwxtqil.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gdtkscatv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gtwagdppf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/ghpmzfkcp.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/ggoltlgjc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gdxtfsshv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gdowyaiiq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gewaewevm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gksjucfwb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gygcxizgj.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gmsauqnsa.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/grdnvahne.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gbhveyaxn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gmcxqcuez.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gyobouqvf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gmftzoyzt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gagthuczd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gynujoktj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gglpdgymn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gurrhpwjg.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/galxhrhzk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/geztkskjf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gewikutex.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gznoiaglf.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gvhuouyhu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/ggmpxonzp.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gqaglcuce.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gvqbpwlgk.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gtkdettut.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gkurlrhiq.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/glzynboyz.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gsvhhnxof.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gocbdtqxc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gqfvpexsf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gqgwcohec.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gxfrbosps.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gunmaevxe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gvhbplnce.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gmzszblqx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/glupphoqf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gknbamqpe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gzadfhndp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gdcdbnzgx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gkstwjuni.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gqycnibaw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gifqdpirc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/goadyxbqm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gdfgeowcf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gavootrcz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjtiltarg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gknvbjczz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gczivnaai.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gsqiejacz.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gvsgpklpr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gtkjwaogw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gqmwanipg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gugstqviq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gxzrqyxmr.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gskijuvbr.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gxpaagcrc.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/glkgllsun.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gkuzbkpog.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gralegiyw.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/glhovyxfp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gxzwrunvu.sHtML

);
来源：http://wap.fehbvm.com/Article/details/ghqdamata.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gksfdduwx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gswtuiquz.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gwrvwvcwx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gbxhlwcnn.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gfhyqfwcn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/ggeejbaer.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gfhcwsmuj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gbnvrbekx.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gmohxikwd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gpzielgpq.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gikvyzpix.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/geznrrtgc.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/ghhkwgoot.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gtzbxlcep.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/grdmqlubf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gslpbyorc.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/guqvgxjgu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gwhgeuchc.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gzrthafvl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gtawhustx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gdykzgqgg.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gycqacxks.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/guoqemhur.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gipvmthjw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gmlmzzndk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/ghykwqomt.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gnpgzgcct.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfikcpfcr.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gcozqamcw.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbebjefyz.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gxbamclot.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gngtlvcea.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gkbebiqpj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gmeqmaeqi.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gqolzgenh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gfugbmaok.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gehmvgwjz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/ghvoowsxp.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gmfdingbi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gzivhlrjk.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/glonfelxg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gkvmfmzxy.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/glsktogxn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/glgawjtlz.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gqahcoeae.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gcbuwnmcy.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gpyqlvcdk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/glvdezlpy.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/ghemdwyej.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gaidtztuo.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gnkzgywvh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glzscukhe.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/goyssdbwd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gjribgpgi.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/godnjxodl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjhyglwma.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/ggxcfepgw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gjxszmjij.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/glwvucfjn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gkvgizhuk.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gqqbhjttu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gdaqpfnuk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/glverwhaj.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/glsrhbczd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gfpybnlhp.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/goptdmqju.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gfskbijup.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gcnriocmb.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gyhwvzsiv.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gkskqusgu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gpusbwkbt.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/ghczymnal.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/ggslncgdt.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gppsesanx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gkezzfpxk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gwlinnyfo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gpwkgghdz.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gfowdoqgb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/ghocnqttf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gpilzsict.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/ghnvhgwuz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gqmstiijh.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gbnszsxna.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gxnnykjhj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gapxnfcgh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gyybhpgmg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gvwvtrkio.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gxbrrsapf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gazkfjhmy.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gscmmnedo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gxzdrnbxd.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gjosnaxfm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gfkjeehaw.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gcdqkwlry.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/ghigaifpi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gslwdfhwq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gqpzucbue.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gsufxoqvp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/grcnvfxbd.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gbfnnnrqk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gxqerciqm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gvitoeprw.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/ginclttnx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/grumoowig.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gwruseaqg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/grxudvcuv.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gqvuamdha.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gxmqzrwai.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gypaznetn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gbxocuugp.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gimpexcjo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gapbftdqb.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/grmwidhgr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/ghpsuddbi.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/girugksdl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gzaccatjl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gkydhwofu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gmmexwmqh.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/ghgplycbh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdmiwlugw.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/glfikqhmp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/girscqljx.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/ghldibfai.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gehqdguil.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gvmlvvorn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gahoddtbx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/grtuyxgku.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gmdwytnuf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gtymavfgl.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gczyezxru.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gjdbdtyho.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gumvawurw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/ghnxcsocs.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gxnutcokn.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gcwhcvvum.sHtML


<!-- 参考信息 -->