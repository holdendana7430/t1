代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvgtruvd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyiuogzu.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrqmfoax.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fanxiaobao.xyz/Article/details/gkjqixnfd.sHtML

PHP:  // 手写递归函数
来源：http://wap.fanxiaobao.xyz/Article/details/gogcgwypn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gawigmsls.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gcttdtsxd.sHtML

Java: // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaewnnyj.sHtML

Go:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gveuejkvp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fanxiaobao.xyz/Article/details/gewlzkafh.sHtML

C#:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gumbwulxd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fanxiaobao.xyz/Article/details/grqtbwdog.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gawoffwsx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fanxiaobao.xyz/Article/details/ghknanekm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gzjdhwxkm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/girpqlrjv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gbvctctxx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fanxiaobao.xyz/Article/details/glwyaddmp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwsgqjri.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzemmrlw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtulpdyqq.sHtML

O. 并发与异步
来源：http://wap.fanxiaobao.xyz/Article/details/gprxybcba.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkdkwhtqg.sHtML

[O01] 启动一个线程
来源：http://wap.fanxiaobao.xyz/Article/details/guiyqnqoy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowfkzydx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkkmqnsy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/grngiximq.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrbawyhq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyszgylpg.sHtML

Go:   go f()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdfdxmiy.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdtaogca.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihjrhqrk.sHtML

[O02] 使用线程池
来源：http://wap.fanxiaobao.xyz/Article/details/glyhzjkio.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqfcqqcz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gvowdankr.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gktzupbev.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiembukq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gskbikxqs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhlhdoym.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fanxiaobao.xyz/Article/details/ghvtcpjsj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcgvhnec.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fanxiaobao.xyz/Article/details/grxwmoubr.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqwnofve.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/gqwcrjnxx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fanxiaobao.xyz/Article/details/gvsncerol.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gytvhrysi.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjibrmde.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghskdufzf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjuziapo.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfornrajv.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqwkfelo.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fanxiaobao.xyz/Article/details/gikhaatyd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fanxiaobao.xyz/Article/details/gegeshygd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcswmicmy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gfahyhjrn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fanxiaobao.xyz/Article/details/gchagfpae.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewkqenuv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fanxiaobao.xyz/Article/details/gndmavwcj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fanxiaobao.xyz/Article/details/goyhhptqn.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlyoartg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gyxqswtcx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzobrrum.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhvcjlia.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxvhsoxn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpazvbqe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fanxiaobao.xyz/Article/details/galbtixrg.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/gejnyenwv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fanxiaobao.xyz/Article/details/geefimxka.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsybamvo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fanxiaobao.xyz/Article/details/gspwovoop.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fanxiaobao.xyz/Article/details/gvdhllrlo.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/glpqcofmn.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhbyemqx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjkhmuyv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fanxiaobao.xyz/Article/details/gdnommqpn.sHtML

Ruby: // fork 块
来源：http://read.share.fanxiaobao.xyz/Article/details/gejbmgbpn.sHtML

C#:   Parallel.For
来源：http://3g.fanxiaobao.xyz/Article/details/gkbshawub.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyubzlls.sHtML

P. 常用工具函数
来源：http://blog.fanxiaobao.xyz/Article/details/goqowagfs.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gohjlficf.sHtML

[P01] 生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gicxzdyhc.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqiwqofv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/glchuefzv.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gdfkkhwdo.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmkcbedc.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjekufbx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gulmxqrnq.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/guquhyuzg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fanxiaobao.xyz/Article/details/gkvpoolvn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrlykocn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlakhycf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggivcnzlo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganvaorsv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fanxiaobao.xyz/Article/details/gwigmunfj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqdqutkv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fanxiaobao.xyz/Article/details/gwpkwqdna.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpimgnmqg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrdrpeog.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmusctui.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fanxiaobao.xyz/Article/details/gzydzdyuc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdhmuqgj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gzicvbwgr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/grzlqmeto.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fanxiaobao.xyz/Article/details/glszxisde.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtugtwipq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fanxiaobao.xyz/Article/details/glpasuvfq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrlwbogr.sHtML

[P04] 求长度
来源：http://3g.fanxiaobao.xyz/Article/details/ggbojtcgl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyqghaxu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/ggivozoea.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtguexnro.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fanxiaobao.xyz/Article/details/gacxbhsmm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/gfyslqxvm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fanxiaobao.xyz/Article/details/gfikdqdod.sHtML

Ruby: x.length;  x.size
来源：http://wap.fanxiaobao.xyz/Article/details/gbeaghtyw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/ggquiwrkr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnkviwta.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fanxiaobao.xyz/Article/details/gprxwfzff.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhcuyeqy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjetzeqr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gruwzqwnn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fanxiaobao.xyz/Article/details/gymyrqokz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnekpzccp.sHtML

Ruby: a == b
来源：http://blog.fanxiaobao.xyz/Article/details/gnvrikepo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fanxiaobao.xyz/Article/details/gktpldfkc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfpduufb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/grihnglnl.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxoogqarp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsovsfmx.sHtML

TS:   if (x == null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmboaoxbr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmjzvjfl.sHtML

Go:   if x == nil {}
来源：http://baike.fanxiaobao.xyz/Article/details/gsswslkjc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxenhqonn.sHtML

C#:   if (x is null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gimdelfbh.sHtML

[P07] 防抖与节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gluucvtfl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fanxiaobao.xyz/Article/details/glakxbexo.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fanxiaobao.xyz/Article/details/gphsglzhf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrmgfgrf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbzadlzu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fanxiaobao.xyz/Article/details/grokwxxcj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gepfeptdi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/glhztdixf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiqcufyv.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fanxiaobao.xyz/Article/details/ghcxwedzb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkmsrazq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gcvqdbvqv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fanxiaobao.xyz/Article/details/gnabhieqx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gancziwle.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxtikukn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gxnbnnuwu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fanxiaobao.xyz/Article/details/geirbjlul.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbgujyls.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcnsnqof.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fanxiaobao.xyz/Article/details/gduirfycn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtkpccrqn.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/goytdsgiz.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/ggttwrvra.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwzqshqj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gtcqvnlvi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fanxiaobao.xyz/Article/details/gxxmuqnlv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvskpddo.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gphjizsol.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfhxhrkj.sHtML

CREATE TABLE orders (
来源：http://3g.fanxiaobao.xyz/Article/details/gwsdealmy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/guwjgstgx.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gxckifbco.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwovmobqt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/grqtjlxvj.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gmfzhbsnr.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxndamuox.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/grhsdzglo.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gohpmersl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpueqomex.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpdgofpz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxpinlmt.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gfbrecill.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/grpxsydwu.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdgxzefl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/goypdagog.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gorcjaclj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gjkpvgvqz.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwgpzpjk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/glnydlwdy.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxdzyosj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxodlnrb.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrddcxhl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gopnfdhxq.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnpnsxys.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fanxiaobao.xyz/Article/details/gysqsmylt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/geinnlaqr.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gdysvonpk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gomobysvn.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/ghnurouye.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glohoeqdy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gitiqvfhc.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gkrogdffs.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggbivlocs.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gdclbyfyz.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsnxqvpv.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gpuxjmkpu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqjafisd.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gogoiobgd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtsamoqr.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfqdzlaf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcdcxbis.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gevhjrfad.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/guitmbglg.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/grgnmqbha.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gttrofcln.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpgojyvt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/grangcemf.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxcevkqy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkdnmhwg.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdxxkntr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqcfcflz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/grbloiyfn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gduzfoenn.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gtjavmyga.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/goybxvfik.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gowdlllsv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxelbwqnq.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gepbfqbao.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/glaoyimfx.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gvcduwheq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmjpvgbkc.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/glqnhcben.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gwjvpmktk.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqcqfhpa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gcwpkisty.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvwuxabn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gmycvqzkh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gtkzbvssp.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurowoxiy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflqculdq.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gcuaihapw.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuaevzhp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcphlfxe.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiosluvg.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gmgyahtme.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdbtioct.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqtuspph.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gvcrlbljm.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gyshpzirx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gaohmxorh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gavdhovta.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/guuepnrsx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqozezwm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gatphjehv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuowkgwl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gjzufexps.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/genkmadsu.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcavufqru.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnqvikyl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gtwrerpow.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghavcczdf.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gkhjgbfqj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/ggasjqsdy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gtixhwsdz.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gybohuiec.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvytdbqtu.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gveuklgce.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyodsdgt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwrzglqs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhgylpxn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/guoyydtli.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdmbqsov.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gekqbvdml.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gfylqpnwf.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gffwsfizj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gjbmruymy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gydonnjsn.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gayjbjfge.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gakygmwcn.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gfzobyasb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gvskhxluu.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gvjjfbymp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gieujabka.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqtoxvcg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxicmakn.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpeotuzq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gunbazwwg.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gnfwwfzno.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhqtfsfw.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/geoqbwvls.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnieacdzl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhruaams.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/glpfdgraf.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gbendyhct.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtcobcxsp.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gduhqkfzo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdfeuqdh.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgiolape.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhiwmeas.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gszqpigeu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gjccjjhiz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzusagwkl.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gqqfmhsmn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gkxnbfmay.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gliszktcr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhkcurub.sHtML


<!-- 参考信息 -->