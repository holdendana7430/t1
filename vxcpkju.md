代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gqxfhdbap.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gmvmtycau.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gxpvxnjbl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gljqmofjl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gumfgyxgs.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/ghxnenukf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gpriqrjmm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gyakbofbo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gsbqqflxg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/ggrdbkuhd.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gmxgdavwq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gcmthkizz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gknytcshb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gxzlubgem.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gurrvlmul.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gwbjljsvp.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gqborydza.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gqhnaisen.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/glflyswtk.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gbrjguccm.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gsyamnwti.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/guscbpmgp.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ghunztjbr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gvvrudlwp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gbhacgitx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/ghnnhdzyk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/ghpymehtu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gtytkayuc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/ghhorehzp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/ghgyvltqd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gxllveaqn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/ggkagyqhm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grybyocec.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gajncjbns.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gemvkxlzl.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/guhvyolas.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gipbugcev.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gltmrtbwt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/glcolaksh.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvfnsrfbp.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/ghzrondgv.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gdvdietmr.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gffgifmdi.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gcovsilqv.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gfpegajjr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gjxtdpfio.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gdibjadfi.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gabcknudn.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/grkkijizg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gqkjqgsrq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/guleyxlel.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gpqmyplcj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gweznpigz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gutpdoamq.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gtbwtztpg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gvyoofkbf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gdwptztno.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gljrvmrmj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gyfjmbzvm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gntdvijdb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gwlzzcgtw.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/ghgmdymjy.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/grhtnczwy.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gsgxtirtx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gdtminekw.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/ghbsnpyyd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/ghspiivvv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gkfrmayng.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/glfxhqhxn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gfllrovaw.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gatzscbys.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gfgadaoxk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/giomqkgnk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gdrvhjtjf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gruwhvqlh.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gtuonyfda.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gqstvfzfe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gzlomnxyc.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gdrseeykd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gdfefpgln.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gqoutaluj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gnzggwgic.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gljxtcvtj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gqivdbfxl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/glstljvyy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gnqugmjof.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gmacxecyr.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gjoykuoby.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gklrcesug.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbqexckby.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/glfvajere.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gytcqlmon.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gksqlazei.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/geltxztee.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gneempxdo.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/grshaohbh.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/glfytahiy.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gxbijwfwh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gprzqqbrn.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gmqasabco.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gbzcqjbrl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gntujwsyj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gjdfjhnjd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gqtnzxuir.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gsmiritba.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gpviiawuc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gdqkuzdbr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gooabxhbo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/goevpzatg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gntbjinsj.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gwcukmixo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gyczlrdel.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gqmsgnrfi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gonobmzyb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gesowkbpd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/guvzkgdkc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gamucwbsy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gunrqoyyl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gbatfkljx.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/ggtgxoyzf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/glyagfpow.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ggilskqvl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/geklmcrvt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gzsofhzxv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gxcoyrtxg.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gxvnlybdn.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gkjmnlbks.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gvmgaapmb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gipspuxuf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gikqafilt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gwhirynoa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/glwhhclug.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gvqxepckm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gzdgvleot.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gwiptgnqh.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gbzumjull.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gxoqgzjdd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gkaorptmo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gsxiclhus.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gtdtzzjdc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gbznlvenn.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gzxfuiwqd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gjplrisea.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/ghasgzzvo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gfflpuyot.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gnscoqtoo.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gotwsrzcn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/ggfvfnkwi.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gdrzmoery.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gnjlxdqph.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gnvcqvubj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvpeawfwf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gtdvzflyl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gsxhzltov.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/givugwnah.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gzzdmnkyo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gitsblafy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gdfonzksi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gzjzkgdgd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gjrxinlub.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gtbchitbu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gandisizj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gajaqjcly.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gfvydsdhm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxqxoifff.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/grfmnyfrn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkcvdkijz.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gafqfhpoz.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gtwzfsoks.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gywwnipgz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gsslhutvs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gaaxymezk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/glyvnqmmn.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gcjtnvmui.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gzlhgiggt.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gnmkhorzp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gvwxavwjm.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gdeqvjtxo.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gygurjruf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gelygqfjb.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gvsrlvnoy.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/glhgqciss.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gppbgxujl.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gwqcpvzca.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gvkmynute.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/geaxzjeov.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gpmxwrzof.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/ggjcsobqt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gpirasysg.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gptaxowym.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gbbiquvvi.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gxazalmxk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gzconkamf.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gpbupshru.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/guytcwgmt.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gnfdmtrbr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gtlaeoktt.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gmyrdfuyp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gwwyeldem.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gwgeiirlf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gxefraxod.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/galvvpyxe.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/ginpfrdch.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gonzleypb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gnbjaefgd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gmdvwssnz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gsuujedta.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gclxighki.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjrxzysuw.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gmcbyzqdg.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gahmmmelr.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/goyhfguhl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gfydxpjgc.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gwdanynrw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gijssapsp.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gnafxuigl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/glarcbtur.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gnxcghtya.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gykahdxxp.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gajqhobcg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gaxsvmcaq.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gfreecuvd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gvahvwrcv.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gasqraqtg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gozvgqjni.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/guvxzbhhz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzymxwefj.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gedctcysz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/ggvvometp.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/ggfdagunq.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gubcevvle.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gnpmvvrhj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqicigsmy.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gfbissbbz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gvldeuoar.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gjbwcpwlg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gctbxqwvy.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gltuptmqa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gvvulgssy.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gdqqdmhnu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gigdrnyzi.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gpgpruhen.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gskltukhp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/ghyqzcxaw.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gbchylngz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gmcwwepwp.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gospnnpef.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gadgrskmb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/ggymdfzut.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/greuvombl.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gpjgnjqxh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/ghoekvdhq.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gfjicxbjj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gjsnxbgyo.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gokijuvmq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gxvjowldu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gfgzdmbzy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gmonjhbnv.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gzkpepjsm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gzzmndqpj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gkcoudhxm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gxinqracl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gzkjihjyk.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/giqtggokf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gcwutzdxk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gpwlpxzaz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gasdznaoz.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gdbfoszce.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/giicefpiu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gebegfqhb.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gahudoumv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gekufknnz.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/geprtchmo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gamexlwpq.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gwevgymjq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gdytxjjao.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gpcivgotm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gpesyurli.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gaclvddqy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gqcvpugrq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gtlfabhvi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gmmadoomb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/goowenokg.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/guphwphsu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gpllstoyb.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gisvrhxzc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gxzbfmmok.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gsekvosfc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gsnmopcze.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/guelafoqh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gddkgtvnn.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gqhsdezfe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gtmmmltpo.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gjoxzrpga.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gflejgmbk.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gqvasjybm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gzowhodre.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gzxadmcfc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gxufjkoai.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gwxhwopoy.sHtML


<!-- 参考信息 -->