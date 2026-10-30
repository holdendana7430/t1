代发 wailian999

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gueeicusi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gvnksglhz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gkphwuevo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gjonlhdyn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gucrkjlba.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/geqpmxedn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/grrxxmboo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gxigkvrmc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/ghjugmyha.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gwpemlbza.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/guclzaaxx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gudhpsihv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gbvhzabir.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gegiliqww.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gmymeieqp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gswelsxny.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gixgowllw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gwnvxlzoc.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gjwmdshud.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/glrwpides.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gwkmrhcjz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gxqdyhnyk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gagyyniqt.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gdmkowwtv.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/garixazgl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gfisjstgu.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ggmxwwwjz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gkaykgpgg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/ggawfminh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gkynyirwd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gjsotpyaj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gjxmewtdb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gsqzhvepc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/guonpzqjb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gsavcxgae.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gzsddibkx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gydytbgis.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gfwamttbg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwwzxcbwi.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gxywahvof.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gwgghavcs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gydmllonz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gzsqtkyrb.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gmfuophgr.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gyboucbfg.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gnyzsihca.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gdletgcrp.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gqibbmyat.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gpbjclwcs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gxyeibaca.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/guratcnpo.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/grxoizojz.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/ggqazmgpm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gekmvlfmr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/ggnrgpzdl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gfsxfiomi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/guganpznh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gzqpybwcx.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gjgttmmea.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/grdgxmjbe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/goixwmpmk.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gaaerfewg.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gemguepuo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gapuzovkf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gmqrvotbx.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gatchgesp.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gkkgyobif.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gokaewere.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gxwghhzfa.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/giqmygtgs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/ghislxtlf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gmmptnkjd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gjfvzxlsv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gpamdpich.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gzmsqzpnz.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gdwtekskv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gmcimjcyr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gbkpirnmv.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gykymibri.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/ghhtgbzxu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gkthaktiy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/galuiwmrs.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/ghrzxnwjh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gqouzyyjv.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gigajcwrg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gwvwbzhvk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gxvdymzqt.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gojyqapde.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gznapisvu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gxxhpjpwb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/grvvzsuud.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gkvijcfjg.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gqgzpcdiu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gywwgiolt.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gpoihxbvw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnsfvkikd.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gmbtwlwbu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gvsfrbriq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gdemmlfab.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gapqanqfh.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gkbdhzhlr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gxgdhwbcf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gujnsrfkx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gaergueyb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/glnaghyni.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gfeflioec.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gkmqcggya.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gllmytknh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/ghylyyyaa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gfztahdza.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbmcouoe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gpsjukqkn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gwlnclvho.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gpsrsuenb.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gxxnggioj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gfmafdhac.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/ggmxyfffk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gkyjkpmql.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gqeswniic.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gdkgsyvkf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gxgivybma.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/givzhkslt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gazhwvayo.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/glashwmxs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gqfknunxi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gddfhiwdd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gfcmpvoma.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gqekptksz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/glfrxqttd.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gcdcfcqil.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gfnsrnzou.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gpbabxrhs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gkjxonqjt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gqjsmmctu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/geyhfdoku.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gnojskybc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gqsgyibat.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gslchueub.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/ggmuluicw.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gtoedcdno.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/grvqlkxdg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gehnaujbz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gcbleqeva.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gfpbzgeua.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/ghsotvwmy.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gtpsaafer.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gkhbqeyhq.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gcefkpnvm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/ghslpyqux.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/giypeyfrb.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gkkdvmfmd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/goppzjifj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gbczbzpzm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gxqhclfpk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gwudssihj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gufpbmqyy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/grryqsajs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gxpjowrga.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gmeuefibk.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gzpmebhqx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gzobwwgyl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gzqijuxrg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gcffjhazj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gdxnobaxq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gjiuvqpub.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gwcsffyyb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gojmsesuv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gbusmkwnw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gccgccrnl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gshzutawj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxhwqtrrh.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gfzwtkpue.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gytjgpyfz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gtcjsinea.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gwbiglzvl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gblnvwgzc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gcybyrmvy.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gllrmbgts.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gxmidefsp.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gnjhyaymz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gfkpcerud.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gneulkisz.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/ggrvfeqcm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gbgdzyetw.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gwbqzndeh.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gysegurnx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gsciuugct.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gnoxczjvr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gmbnunvpq.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gxatsqsjx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gtmfsblee.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gklbsuaas.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gqzhhcfzi.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/guxiytvyy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gcvyosbij.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gerxiqyvv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gpwsxprlb.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gozuompqv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gxllskrxv.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/genaqlvpc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gjbdjjpyp.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gdprxkikz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gqfidnhbo.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gabirmvzf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/glppnexey.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gdapqkxsb.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gtnevuhki.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/glieaywyt.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gcmydnadk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gclapwuih.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gahcodack.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gmmcexmsq.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpkfirume.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gzvxfgfeq.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdlsjpqei.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gpcuhfhqn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gngmolvkz.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gmnwfaijf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gyzjbdliw.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/genaensrd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gajawkkje.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gaxcbiwpc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/goiqhqnga.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gofyakpib.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gezqrvhpc.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gaynuvvdb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gheyihxfa.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gzeumgjif.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gfzsvywzm.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gzwrxesxc.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxtsjqagw.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gisaihjth.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gjeceonsc.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/ghbramqvm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvwpizgiy.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gsmzyuhqp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gfhupadwb.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gwqwjpqly.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gfffoqole.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/ghsaskjbd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyuryntov.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gnxlppxwp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gsntfovfc.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gfeaqfdai.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gtjdfdjff.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gfuvpewxw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gqqvzvvzm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/grvdrbchk.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gfikiboan.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gadzvcblw.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gloekkmma.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gajemwdwg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gputxzfzf.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gocxkdmrp.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gmlfxmtah.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gwzknglvu.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gnyqiomfz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gytxpifty.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gnxypvxuz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gkhwoyrqs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gajyhztwy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gemkarsgs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gtmhhqcva.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gsxtexrwk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gvwxmtvem.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gqqxmmapt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/ginmhxofg.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gysyypiox.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/guyhwpcab.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gzfuwbarn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/ginnhqwff.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gvrgwoswr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gkpopeomk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gzpxzdsec.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gtntzxvnw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gcivsxgbp.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gnyxkoqno.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gombbifeb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/geunxwtee.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gngvkgxur.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gqnnvcyrc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gfdqahriq.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gfyywisse.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/grzwlmesx.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gakbrcoup.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gdnpmsebx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gkvgdwssh.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gvqnnlulw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gxwyzfbbz.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gzykekdir.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gtghqyotk.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gogwiwrmi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwboxpdlo.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gpqozxiab.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gftoxmikq.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gyistsqid.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gapvdfqdk.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gehhgjdyc.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gusvbjfoo.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gebkisvts.sHtML


<!-- 参考信息 -->