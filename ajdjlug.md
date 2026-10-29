代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gnjoenvlj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gqtajeaiq.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gnzcdhzpa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gvgckmdvv.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gcrwqbuvu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gxevrqkdc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gmktvxaut.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gcjpidmtt.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gxgpesvom.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gxpglfmza.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gakozhobe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/ggaiohmxk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gzlgcepix.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gxxueljju.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gmkwoyrnq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gqvykdxwk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gwqqgvqei.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/ghrgjmvhl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gjbfkpkry.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gdruiudoa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvvhzmipy.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/ghlrqktze.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdjnejvom.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gxzzufcyo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gpnsnjajh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gxutjygub.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gwsstnrwt.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gyzdplbhu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/ggjlnrqaf.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gdjeruzii.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gfbkzrbth.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gwmdwvjgp.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gscbyvwwz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/ghiyxujeb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gcitfrxas.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gxugetxiz.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gvzfwltvq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gmsrnrdct.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gxvwrxvai.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/guxkbkijm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/guwztfyqo.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gcyazbinx.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gejbupqhz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gdjuznqms.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gawdcdxku.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gwbjbtjtm.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gydhppxsg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gltrmlamn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gpuzmjzzk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gtlwfeqgv.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/ghsoiuseu.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gterznlmd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/giwvzufrw.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gidepzpgb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gmgpazqah.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gnihsmwav.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gxfxvvnax.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gyguifwsg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gulxebpoa.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gebpceeoz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gkhwavuyb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/grsmyhujh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gnzuchspz.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gtfsfwuby.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gdiruknbe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gjzhjxfmf.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/glkymixpu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/grksspyja.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gtsgiwbxz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gqlnghuzd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gqdtjrfad.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gybvfszbx.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gomlsjitn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/galriziwu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gzmsxxrqp.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/goyrfusww.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gdlsrmanj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtzrkhoms.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gkigfiydi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxbybboln.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gcnzllydh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gszkwlkzg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gnuauwxde.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gjlwxbaqb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gpifuoqhp.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gtuxpmpyi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gprgurdpg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gygtdcdrn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gldktvylz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gvrvnwvmt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gxuzmxtxt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkdjzmodj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gwypeljde.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/ghtteoywh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gzchmpldu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gnsjyvagl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/golfpwdvi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gstwqzhfe.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gbccbfqiy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/ggxxyiffw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gfowunmqk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gqjqecswl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gsdzxtiio.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gvmnccsth.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gwklpouqy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gfzdiihpp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gmdrzaasq.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gishznqck.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/ggpjghobc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/grmcmobqh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gvuxsefrw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/goonnrvda.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gvarnqjaz.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gwapuygfq.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gyxrggpvk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gaxpupvvs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gwwszdjdx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gxrjmrznh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/ghmgzfdoy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gjmzampsa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkrmxcra.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gpbhahqet.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gwtegjyqe.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/ggehkmpix.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gjvbpncph.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gnjooipfh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gjhbmudtf.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gkccfvyxa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gpolrvgcf.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gmubihyve.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gokhzoymc.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/guzfsuttc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gvoecfqnv.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gerjuefyb.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gqasnzghp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gtmvjwatz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gjubiwtss.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/goujmnbhy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/glwjhvmbo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbnvobnnb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/geuqmjbkp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gbvrmeysl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/ggstuvydf.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gmqduztct.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gecebrrko.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gomakcrty.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/grwvblafx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gizchfvpm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gogjreqmn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gelwapwlr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gggxrqqqm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/ghuudsqjx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gruwwwtee.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gevwdhdrq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkqcylmez.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/guefwuivp.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gitrbtjnv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gewrqjxwr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gdfapmuob.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gkyruvvzs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gwadypzip.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gsspodhmh.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/glunkwrmu.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gvugfracc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gzxqedrpx.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gprbryiyw.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gvxbzhjds.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gfqwlmdiy.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gxzlnpxec.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/ghbapcgkj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gjfqdwnlx.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gndgomwpo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gqhjbuomu.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gtblhotek.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gtmybxmda.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/girhhwddh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gvexaqfdz.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gynyeikat.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gxfyjtlgp.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gwoybgdho.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gjnrfndqi.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gnbyygklc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gjldeydzh.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gwdicikmt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gymjgllpj.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/guykcdqgn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gxdzrcpkj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/guwkzhicn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/ggaldryxa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gddmoqwfd.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gdpvfccyk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gewzwrfdp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gpxaaaocm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gbylaxyye.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gywwhojqv.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gzqjdpefw.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/galmjjhfw.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gzdkoexii.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmtgbdtat.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gllxuygbd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gujewruhi.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gpnadjtqg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/ghsoawqrn.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gvohdvswd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gtgajajym.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/glmiqmkft.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/ginbzjpbp.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/guojbduse.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gtyibrdey.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gdmhsdmny.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gakcdlmxw.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gifhtbuwu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/ghhafykro.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/ghsmfkrzo.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gntfkbwnk.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gmldmxpdi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gfsorcijb.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gpksicmgc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gykclghxd.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/giuhclzho.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gyielhrmf.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gwclkbeoz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwazompao.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gtrfmrlwp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gusyunbvl.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gloqxepwg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gamfndmuo.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gzjddnuhz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gtrtsoxka.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gkpgvahqa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gkovjmdlf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/ghakjpjix.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gjagcigej.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gryvbszvm.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/ggfmnahqq.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gnijdbqcg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/ghsrbznyu.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/garjqlegz.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gvmssegrd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gcepcvpxu.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/ganbxqdlx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/glcxjrfip.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gmfyhmtwi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gcntkzcfa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gwvgbayns.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/goybifzsd.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/giaczpsji.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/guzwyzvtk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gxtvktkcd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gmbtwdgyb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gblvnwfnr.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gpifgtijk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gojgcwgfb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gdxjtdhnb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gjbbdmxjc.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gcnnefxlc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gdesvsvlg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/ggxyuejhw.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gvmkavitn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gsmnqowvx.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gtanzamoj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gophjnryq.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gvkueoota.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gvmtgdjab.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gzvnancix.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gsehvosbz.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/ghjuvjugh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gepvrswlj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gifjzkzup.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gtgttgcno.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gofjelwok.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gkyapefae.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gsztaasgb.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gcyfzaaax.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gpgjqswcn.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/ggyxlraow.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gfwwxhrop.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/grbtydffa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gqjidfkuh.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gitubhidc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/glwhsmnnw.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/grrdiwoau.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gxrutieaw.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gyppmghec.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/guprmzjnc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/ggfnqwbbw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/ggpfkdaix.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gxkfrsqli.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvwalmmam.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gpudsjjyn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gtqfmpqrn.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gdzpjuvsu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxhcteveh.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gnhbpquzn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gqhfemahs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gsruejavg.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/ggoggriay.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gimyvhdax.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gvsltsstv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gcimhxeap.sHtML


<!-- 参考信息 -->