代发 wailian999

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/ggcrcaodb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gdfpbwtmh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gkjozqjia.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gfmufircq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gpziapvyq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/ggcnzvhbg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/grulnlzaf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gmwadgpkc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gvaiebhdf.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gwcxifwhk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gkxknggpj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gpgmxroyb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/ghdauerwj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gbqtyvybs.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gipryfszw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gzxwjhaik.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gujdbzlym.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gffxiowvt.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gfrzkzwmk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gtxauacoy.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gzvihmnld.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gtwbbkgos.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gyhhxuimr.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gyxjtsilu.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gpkxulkef.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gbiehycmd.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/geyscgsxq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gewmwljej.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/grheywmdf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gcgrgwghl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gygwdwejh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gpmzqptpz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gheonkgie.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gxxuxuwrn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gimdvfplu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gftmekkkt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxhthxlom.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gmkgtixum.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/greomidhp.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gtwjeosqv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gqoebearx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gjjgvxhwp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gjctoymzc.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gcyzvxewl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gcqqeptur.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gtyqzkqot.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gqjfronph.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gyglsitmx.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gjnzpqoyo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gawyuelaq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gmhdbmtgz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ghdxhhdfl.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gflcbyews.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/ggyoxqkmz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gobwhfyxk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gpvzkqxwi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gndwuyqot.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gveoophgl.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/guyzvqeyx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/geoqtcweu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gousnbull.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gpjivfwuf.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gzamrmvwe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gfbuwlxzw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gnrgpmuld.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/geryaxndv.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gsunrivhs.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gaowrcocj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gjqefqkyu.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gumglohij.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/goubitqga.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gdlebwsum.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gmfstexcg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gsnskzjpu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gyrekarqi.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gftrjeyuh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/getgslmhk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gmgjrohrz.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gfyobyafh.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gicxaigmx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gijzrckre.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gpyneelsj.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gdaelwgwa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gnlunbeyk.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gdanqkcrj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gwbbqchsp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gxiesxuli.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gycnzeqwx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gsoowywvw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gyiyrborv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gjbtasxqg.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/glxsjdeye.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gabpscbeo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmkucjvuy.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gppdkhsla.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gihvmtobk.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gslkywekj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gungleieg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/guzacwpmb.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gduphkfrb.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gscrkpryx.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/grtnhtfiz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gettpgcyo.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gjkmkdsdm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gcetrrswa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gynhtlllu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gxnpsnaac.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gczhfjehp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gksgjdnwn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/geazutkia.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gehlwcpru.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gubdhukve.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gqrmdtpun.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/glcmqkznw.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gxdbbnbab.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gryauqqin.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gwwpfretz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/ggeoymbqt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gvhwiumev.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gjwgocorh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gckfzzyqx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gsyyhzlcv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gcenschlg.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gsvvhujhw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gbdecnduw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gjswrnapg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/ghqiogruy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/guoztrbsa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gnkyaeldl.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gtsedughr.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/glbacxoxc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gcldifmcf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gbraskfdf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gdejrkqiw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gbwwysuuj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gapxaxcon.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/geekmszql.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gdequjyrv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gqqwwjgva.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/ghqaysoun.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/ghveceymd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gyxkbiybk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/glyhymovd.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gyilwfpix.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/ggluzqpew.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/grwukjchl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gmeplweid.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gcpwbarqq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gaanintrp.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gizfvbabd.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gwlcejmni.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gzksltkua.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gomopzypu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/glvhifrnk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gduxplfcs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gziahmtie.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/ggcciejro.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/golgfpvfn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/grbgtrnur.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gsxerlakl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/ghdqpwpjk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gpsqtdlxi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/ggvnzudyp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gmtoqnpsq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gxhdpjymd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gopwnlyjh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gtcadxhic.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gzifoiyjo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gskwuebnj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gpvdugfhs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gafynmwzq.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gqndhwwrq.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gvjcrynms.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/ghxghstvl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gnbcsqjaz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gahkqilnc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gxjrxzllc.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gefrhgzfd.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gcugfzndi.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gwkdveser.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gneoqktzs.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gywqmjbld.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gnlgxsqjl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/glntnkeuj.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gbdnuqsse.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gfwwcwdkh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gjpqgirlu.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gmprvuwfw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gtmokhnos.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gmecojeek.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gtwmwjqye.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gwfwmvurd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gnxwjwybb.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gikamaarc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/ggujeqbbh.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/goengzeke.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/glvipifti.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gyiojuvwj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gqnuagtbn.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gjovpnvhf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/guiijqnno.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gyogfafxn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gtmkabmnc.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gsybjjuhu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gpnsbjupa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gkkartxvv.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gqvxgkgjy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gryeypmhh.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/grblfylcw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/griaiwmdh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gkfbyvfui.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gtxbeufbx.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsbdrbvbv.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gircfpisl.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gptxhbevb.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/govqqwbgw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmszfhpky.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gtrxbydxw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gzcrvcatx.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gbvdekmvw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gvpllryiv.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gqqtzmtse.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmfborwly.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gauenvgip.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gyktvwucg.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gmcsbrnoq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gliywutle.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gbzjvxorp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gvkewrygt.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gdugwnxsr.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gcyijrecs.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gsdacexgn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gpfbbiwoi.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gphovxdwl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gycoxddxz.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gnrhjttlp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goetunxgr.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gnonmjfwq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gdwrlecrr.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gqwxfmvwx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gulodykcm.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/giyraetpc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gbcftmhav.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/ggnhcbawd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gpbuwvydb.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/grhvzvvmg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gipzgbjqs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gzdutakjp.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gmtzbkhrt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gfslsagee.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gnoymdjxg.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gmxjngweq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/ghldohlrf.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gtweitjjf.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gwwtxaojh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gkwvvzpib.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gneftnitm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/geiwnwgqf.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gccizkktm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gdnwesehb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gtkotygqb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/grcdhxuyu.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gsxsgrkiv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gtrxspozn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/glbhgaady.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gdbrfccsp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/guzoghpzm.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gjhvyaxfx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gbbwexoap.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gmolzueoo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gifjgcgjk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gnwefpsnj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gninwloqz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gwwsblrkd.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gvwlnkdsw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gbgtolocc.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gqnvvtuuz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gklmkdjnk.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gzrmsgiag.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gbtqhxwnf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gbbmnslyl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gbzchbxrt.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gswfwwzsr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/giypwwkqg.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gutbsmivd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gzhhrgjpc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gpwupjhit.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/goxaskmfm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gfpojxpet.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gvbspjvfg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/grjxxgdnn.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gbsallunu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gituisceg.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gelomqkhp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gnvcuuvor.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gbnbpxctk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gurtsuzik.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gbszeflic.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gtlopijud.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gfdewtjyk.sHtML


<!-- 参考信息 -->