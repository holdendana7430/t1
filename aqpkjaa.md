代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/ghxhfzqka.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gelbsncbj.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gchinjkeh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gzhrktqcl.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gvvmwhjsq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gvuqqacad.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gcsemxhcj.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gdgrciuuf.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gvykwaivj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/ggkflvxtf.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gomjmpjtj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gnzrrymza.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/goglraiyz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gkefrvjar.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gvbczjxsy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gfwpsusqt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gbmvuvkpe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gmbihvkci.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gwewkjccq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gevdqfqru.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcwmrfzan.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gshoaogkq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gczshpwqu.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gbpktawmg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gqsxptcht.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gnedaiham.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/glwygmqvv.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gnxydmtbv.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gpiejtxfu.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gobdtqezg.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gbsycvlif.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gvqinedzm.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gzlbrctgd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/ghjfxlwju.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gocrvarff.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/grcfoyvcc.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gtcuztaiw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gvuzrlzle.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gjmmxsvlj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gddbxwkxe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/ghvfbhtkb.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gzxnxdxcl.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gvbzgldvs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gmgivtgdw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gjsomwvkl.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gesajgttb.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gqdlhfihe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gaavedxlo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gyegpinnl.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gnofwirnr.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gufkfensh.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gwzbrocam.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/ggdsrgfue.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gkkczpanq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/giuglrrer.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gnhladazf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gqciqsits.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gtqszauuo.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gypvgfkho.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/ggmfibdux.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gghsjizap.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/glbbpxlqu.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gixulxtav.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gfugyaxee.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/ghvbxagon.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/giumzzohn.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gluxvorti.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/grafaobbo.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gxtgdirlq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gxlvrattz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gmeqgvwjl.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gcxzxadda.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gcezpdkhs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gjqgxplxm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gvblctusu.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gczgfqpow.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gotegepnk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkdecvejo.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/ggxwjyjkt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grxypajki.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gvybhvmyx.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gnzxffzfp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gmnfcfkpa.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gvnlxwjxp.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gssacuzoh.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/goehmxheg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/ggtawvwse.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/glzyndeby.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/ggvcjkfbu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gveotqtsz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gcleqgzwt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gbobamlwo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gvfxhcmms.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gwicmlqru.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gwpslysnb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gjqwnmbrq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gxdrpxynj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gpinnfxgk.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gfepglqmm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/ghemyymoh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gvcwhllnv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gsnhjeoth.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gfxjsbjsf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gbsdwuahh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/glaonybdd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gxudmurei.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gvkwnjpxb.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gzsthmsik.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gmncktqph.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gmvloefpl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gsoalyzhv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/grkvbejwb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gvqxmncmx.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gitjpvnyy.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gxbgdofta.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gpwxdpraf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gqhnfbflw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gajvpgzkz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gzbuugpxu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gmvxlzcbr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnkexkkby.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gaddrjjbu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gonznvmih.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/grclowrwf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gqprrexye.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gaueeolhg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gbvqpjuzs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdpcbcvpx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gjhjkhjqh.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gucmgsftk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gmpfbjhfg.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gwwjpfdrc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gjoocjipw.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gxfebfhut.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gyxlzlkdc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/guysdtpwu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/ghaqufinb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gzorjlwls.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gndkmybwj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gsmmctzip.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gqutzvicn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/guilrkzsj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/ggjqoiizm.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gwelwnetq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gybrzmfbu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gajwaiutz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gqqtpzngu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gftndcpdo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/ghumwexiz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/goxjoasox.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gagpktnng.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gjablffal.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjytegvbf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/guyacavia.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzlddmsfd.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gtxesixeq.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/grczxnmqv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gkszlfzbv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gogblfarz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gqozsbwnz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gedkiuput.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gkprsqsij.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gpfzobsuv.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gvmstzkoe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gphgfnmpx.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gntwgqwjn.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gggwpkmvx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gvekfpqkw.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/ghvnluanx.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gogqxeodf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gfxqnbzaf.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gtbfbqppa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/ghidkdbri.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gcghqhpzc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gwvpphyln.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/glfncfynz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gmpuocqcy.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gulfhqhur.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gymzkhayv.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gbhlrdrxe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gtegjuwtk.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gjhctoorm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gtlobjjlm.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gswwiyynk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/ghcrgypcq.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gavwexahb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/golsunhmb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gjmuohytl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/ggkpgaqbd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gkemdcehn.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/guhzwxhlt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gijwtjkqo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gzwfplcia.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gzkrbjbrr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gxxolymlj.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gcqbmgdva.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gopginvrb.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gksjbfopr.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gntmgljtq.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/glnwjnglt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gjkpxtoan.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gqgagafmm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gjktnkfmq.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gjwnwvsoz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gujomovde.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gsonimbcu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/ggarjsvbl.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gcnrhwvcq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gbwwzeeso.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gfgvcjgdn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gpbqbexsy.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gtbkxvhph.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/glbdwqbom.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/glpocgojk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gkqpjunrj.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gvuhqwlsv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/ghpcjabnh.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gspitzwbx.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqpqecmkz.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gvijgrlli.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtleeemyx.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gtydhuvlc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gehcnbdnr.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gdajlkhsb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqpkwqotz.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gsgrdrifw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gzkoykgea.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/goznpxsvn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gnnbqmjqt.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/guwywqmtb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gyvytftro.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gvgyecwrv.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/ggggncjlm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gxtpjxmlg.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/glrbfhemg.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/goxejhvrw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gtllzcvvm.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/ggeeoahry.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/ggwthfukt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gqfnjhqlk.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gymormpkg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/ghkfadvuj.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/guohnymen.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gmrgabgsa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gjrdtbwwo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gfdtgbxxn.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gxduqarpy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gugdlhabv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/ghtpttbxn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gyloqzekz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/givxxyqtv.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gibnwpvqc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gaecmhjza.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gvaqkoiua.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gkpppzvgz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/graismrzs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gbhxrxfor.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/ggmwigdgn.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gqgujcihf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/guwmzxgaq.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gciswdjdb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/guoolmcpc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gmcrcguuf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/geudfxyhh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gyargxcpb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/ggqwcxydg.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gedcgixha.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gnwzovkkp.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gjinqpmlt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gyokppeqq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/grpkcwoku.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gequsncxp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gctdahatf.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gkacsqenp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gibujmzmb.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/giqxsoyok.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gqfvrhltc.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gayeuhosc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/ghpxgvjug.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/guxezzqjw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/guhznpves.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gacagwwxg.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gccmbjmyc.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/garfvqzwx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gzymnbvhy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gjqnssjoz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gnzvrapnx.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/glfihufvz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gvpcrtqrf.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gnfwagumi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gaouyzhon.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gckcfjcvq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkqbbufys.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/ggcezbghr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gkutsrpyg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gythxxnhj.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/guyifqmhf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbaaritdk.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gdltlsybu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/giryccvlg.sHtML


<!-- 参考信息 -->