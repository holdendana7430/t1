代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gglegnbts.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gwdundtwt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gdlylqjwp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/goaqrtznf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gvqfjaage.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gyseuzrcj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gdojuhqht.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/ghhisqzbc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gktzwhrbt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gtpnwprza.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gqnakcwso.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gbwandtna.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/galctungt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gbqaxpgho.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/ghbfcuyjc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/guoawutea.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gichcwfys.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gtbzvzmyd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gvfunvusc.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gucoxoujd.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gvajhrsyj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/guophscsd.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gizbqnzwc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gptpdpwcl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gddbocyhl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gunutygho.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gtsgmneoz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gbnwjwyyx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gneekmhvb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gwlmfnpue.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gxcjuehqy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gqlrgcefi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvkqmktby.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gfduacfjo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gderimywk.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gwodvbvsh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gyzhokfbt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gkzmyfixt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gapyvluuw.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gxbrzhmyg.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gcfhdbuni.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gzoncqpwl.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gueldyngt.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gurcjpxyk.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gygrnccrl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gechozrds.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gasdxibir.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gihtjfgxk.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gzpvavxae.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/goxvmpbgc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/ggxyxgiot.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gsmlfhcyh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/geewwdotm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gymbnbfnh.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gecinnksk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/guhuczgyt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gnfmijfgw.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gnolihazb.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gubplyudm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/giamqgizw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gonjahzed.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gkbvwhxae.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gbidwyqrv.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gjfznoykl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gsktpueqt.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gfvyeweia.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gpglikjhu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gruuhcjos.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gozcfthyi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gcnpgpvef.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gkracpcqo.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gwjruarru.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gxbtvnpng.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gzvsuaizt.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/grphsjfuu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gvnefahhr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gldpztjar.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gsdvzfhhs.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gkqibzdqw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjyeqdsh.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/glepxpvid.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/goexsczuh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gjdmmoqxw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gzdotwyiz.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gitpgktmd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gbffctmsa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/ghepyijgo.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/goyiehkvr.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gmjhfklnc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gppsjtmmx.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gexedorvd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwiqscpoj.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gnyumopfs.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gzfcgvvmj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gnddvkjtn.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gwrcyywdr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gmskvpolt.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gmishcgnl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gbxhgnhhh.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gccuffpbi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gswfztknz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/grdvwufed.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/ghfshqtfd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gwzfpvalg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gzcwfbbwp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gdoqywtvy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/guetypxnc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gewhvrksz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gvqrpakxy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gdpnsfgyv.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfbctrxye.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gpmkqqrkr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gskvpckdt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gqupqxpjd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/goenlhfps.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gkivuicph.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/glkwrkebl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gsgulplus.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gpyjkvlir.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/guctdrxze.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/glpbinipn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gutsbwsyd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gelyxugml.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gsouuoaif.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/galeeiivm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gfpelvifx.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gojljcgrj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gmtzyyjbw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/giheqqilp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gvjlzgknn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gvohbhava.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/ghnnabeno.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/giqjabtap.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gvsmlmycs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gaernarpd.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gikpwoxzg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gccjoqwmg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gfduafdcn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gfwnilbkc.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gmkqlwdrj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gcnomfcua.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gjzzwnaue.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/guhksotwx.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gukxvbkea.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gtncvgdji.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gawtwxbrt.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gvkdmpfmd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gynkgqbmh.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gshejzeyr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gxhheikry.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gwfrhmhhk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gpgwruftg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gamusxjtj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/ggeonryvp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gazmouomx.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gnubmkvjj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gvxablkcw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gdrxipoip.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gvzxbtwjw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/ggmdojzif.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gcuybknjh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gzmtnyape.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gbpgokekz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gegqjtcpy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbcpdildr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gdakhaycl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnmygpcry.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gvjplhsmc.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gmjgvdawc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gvhxjstsl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/grmetyrsg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gxnxdqcbo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/glipzbppo.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gdimjosxw.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gfvbghatq.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gajlrirsr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqqsdvqmp.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gomappfig.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/ggtspokyg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gjtfevzbc.sHtML

);
来源：http://baike.fehbvm.com/Article/details/grjozwgpc.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gqamcwzzv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gnhipyvmj.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/guferdluq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gkvqpeqgn.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gyifzwvha.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gkrzoqkju.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gjjkvluyf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/glfwninqe.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/ghngxmtab.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gpwhfoxnc.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gwyindiwz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gtovybrcf.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/grjiyiahb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gdisrfpsu.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gcyxlqoiz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/glxhkywtt.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gkbnlljgy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gbtvgqyfc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gvmnohjyj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/glprdvxds.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/grbqoozdv.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gymaepilf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/ghvsublza.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gxteoqtzp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gwndammmv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gbvxpzfmf.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/goihjxvhm.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gahodacih.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gmpfdewiw.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghutibrvx.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gxscqvcol.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/grhibffob.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gpdwmlqmf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gmdybohoj.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gptbliwsi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gqzpticni.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gykphijoh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gjcxafvow.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/grackpqmv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gsbfbflrl.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gdvyhzdoi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/grzmljaxh.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gnjgxlqar.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gowpzzefd.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gzetmuuqh.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gssoazyop.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gaenxdaiw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gtcxdpdhn.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gmaqazztk.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqabpfyjm.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/ghzbwsaft.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzfsdnzms.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gqigllymr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gvtsagyxu.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gkgkyqqgg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjfusoiuu.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gsiodhmmr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gzzymwqsn.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gujqpnbai.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/ghgfgslbj.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gljxdchci.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gjsyrurnp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gxpccoedy.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gnbofyrpf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gmmoyxmqw.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gmaaxjqxx.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gureiwbgq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gpwomquff.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gqiaqqxim.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gxaxwyisg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gfikhapjt.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gbwrkfypj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gafpteymt.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gpahzwpdo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gxfgeormi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gzgsqtvbq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gktvnkqgs.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gvsuqjgkv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gfrlofmbr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gsdihvfje.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gfbflblkf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gozfhjalj.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gnetenblq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gdqvndozu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/ghkogtiwk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gjjihasxm.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gwpirntrw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gfebhgsop.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gdnfayanm.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gnqlzncej.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/guvdpsvbf.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/guurmmorv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/guhhcfjup.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gcebmrbii.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gqjedrpyv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/glqagnxge.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gmiarvrtf.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gevwxoxxw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gwmeegvzb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gcnigxqvj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/glhvkjdbz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gnobkiela.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gxjqxzcep.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gvzntebca.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/guauubhcl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gbeomdutu.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gmivxqzqw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gbnhbfgmm.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gupfkjwpd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gdfdzvifp.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gwduvcwsp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gyaaraxvb.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gbeeyymle.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gswjuwghv.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gedyjgfry.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gyyaxxmkw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gdwanrmgt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gbrbuosfe.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gptqphxbj.sHtML


<!-- 参考信息 -->