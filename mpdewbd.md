代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gaogkofhk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjjcxjdvg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gsxbpaext.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gjcyihmdu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gnoeeattq.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/guxhtipwn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gosazrwzu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/ghnefsamq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtoeksdc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gwrwcvrbl.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gadvdoyee.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/ghbgzoanu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gleshejrj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/goffutqso.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gbnhlnaqa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gmrwuzjml.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gvmhlylsg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gmugzndoo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gtkpsrrup.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/goilebeov.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gqjqaefid.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gdkxtddmd.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gafdjjozv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gtgawexwm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gwbietvri.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/ggbgaudqy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/ggwkgzled.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gmtvwovrh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gfyccunvn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gzgwwtziz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gimfbiugt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gitortiee.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsbsqvcxi.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gkzclaxag.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guhvvxcbk.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gzkiehfrl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gxqygydcp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/ghqfvgsba.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gmbjmgnra.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gitzcvbkw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/ganswdegz.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gdvcrnqag.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/geqhsajfc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gllijsgkt.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gobfgmahp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gptrgwzfa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/glhseroem.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/grkryhuwj.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gylwrnjgu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gzfueffam.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gttxtxpxf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gygnqkpzh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gfjpclnob.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gzbkzzxiw.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gplpbpqqh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gokuyilta.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/givfrbpha.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/ggltfjzoy.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/ggizbuboz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gbzkgtqbr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gyskteasp.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/guwizxudw.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/guctxfauv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gmfyxfpuo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gtsbymlhx.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjyjugbdf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gzlwsvcyw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gfkloizdz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gqodndeha.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gmxhiifjd.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/ggqgjmoqp.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gnwtggneu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gguvmswgh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gpxbgeclr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gnbjvcskr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gzfbvoxrp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gdxnnqatn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/ggzmzvnct.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gsgqxbdmb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gydlpowwy.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gudawrlbg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gocpgeswu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/ghmjsieco.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gcedybdrc.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gctxwfsgy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gaijuotbb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gonxvcnsg.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gitqsnpwh.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gfsaoaiqy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqnqdtwnb.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gytnxqivj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpdxpqyxx.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/grkcoghbc.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/geadnrocj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gqnimbxtn.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gptvwxdld.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gvybgchfv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/ghcusydhk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/geqyakjsz.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gyqizfpdt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gqwdudeiz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gqedvdpcd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gehfksphq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/glpixkdup.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gpjoquhmp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gjjtuyqrx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gvvtgykmy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gqtqipvfy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gdtnfcaxp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/ggpaykypq.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gwtcmtvhx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gpffueidd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gxqmjrjdy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grdyceimu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gtuqigcdy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/guzdzjccx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/ggknommqb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gojitwqtp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/ggmxjcxph.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gxfxblcpg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gecvoakif.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gerumlubk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gxohxobmm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/ghowafiro.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/geeibwfpy.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/ghovvpmqb.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gmalvastv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gtoghvzpi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gqjqtxlad.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gjwqawsvr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gixqizyjs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/girgiemed.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gdtvofmjd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/guqacuvqv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gmqozvixz.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gyprzoiat.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gwbdicagh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gszooarcs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gjspraxuo.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/glxoacpuk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gftevqvgs.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gfnzhdrxn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/ggkfxbebo.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gszxygdqs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gyxknawqq.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsyxwvtfd.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gqnjfvivh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/ghfnmqhns.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gmwctvjoq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gofgsfkxl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gxpszclzx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/ghdedkgnp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gyjjnexbx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gmvmpvfwf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gfsggjkom.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gsbzbuxtl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gfrnhfgjn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gyovwnsjy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/goormvynj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gefooewrm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/ggvmavhvu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gdblmlcig.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gzzxxfxqs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gcokkmoee.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkzekovvj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gefxldbie.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbdheefbe.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gtprucuiq.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gavhtmmwg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gibhklwcy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gjvqorqgi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gmvxyczsr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gpyixymau.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/ghjpsrhtr.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gepdlahof.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gzsioggrf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gbnevunvm.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/glldducop.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gdoswuyns.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gpfwfxczt.sHtML

);
来源：http://wap.hesvh.cn/Article/details/ggfcdifen.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/goxbbrgnm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gavuqikim.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gkeuhvtpl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gwaqptvkh.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gmnvubnkc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gbyihlxws.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gbbagsxjw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gpbefkqkl.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gmfeohskw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gowzztvhr.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gwultonas.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gldiktiow.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gxkjxtxoy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gnzpdzerh.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/grkjsdbyy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gcebegmsx.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gaidfnmqg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gttymwwes.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gfruxqqhq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gbsvteiup.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gjiatjlqz.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gxrtbjlih.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gsedijdry.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gekxvlizz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/ggbsepdpm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gvhiusrdz.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gtpadpdte.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqlcfkfmt.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gkovogisf.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnhhbpvfg.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/ghjunfrow.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/goxsevbyz.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/glonrnamf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gnhejgsrs.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gucwuqblw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gkbeirjco.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gxcduohas.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gutbcxoqa.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gigytwwjg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gqotxbnql.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gzsoahxmq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gflonbnaa.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gpzsejcmi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/glmidedgv.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gmuxhnpes.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggnucqlab.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/glqatfgcf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/goqjdddxt.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/glkularje.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvoludwkf.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gaqhwompl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxmqftvtb.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/glrucwxgo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gwkjpzbqg.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gsothvvez.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkzqiqxwx.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/ganiurcid.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gvcuajbvl.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gbogfoond.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gjixhyiff.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqekgqojj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gjgcrmrnm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gmdhppmit.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/groepmmsb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/glljycfyc.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gqhwjjuev.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gsqhddwau.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gqoiuvcvn.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gazxscuth.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/guodemlxp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gfmgghqbv.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gfnshpsov.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gqotgbgvn.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gcgjunobw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gikmfvcoe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gssokpfqi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gneowddvp.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gcdgncgix.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gqxwlxrqi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gxqtmgdob.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gkuinnvbl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gpmkrbwua.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gurtwbeyg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gpxrtlvkk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gjchjslnr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gywfkxgjg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gmbvymjft.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/glhdfetqd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gxwzcvvdq.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/ghxsrjlmd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/ghwdwrppl.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/ggomctelv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gvaizgcar.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gzburjsgf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gxqppddiu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gcuhsjiat.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gdvinvvew.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gjvbopzcy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gbnmkfbqv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gtnsntyod.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/ggfkobxeg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/ggmosxbkt.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gtugzzkpn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gurnhgsmt.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gwmfuiafs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gpqykvpod.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gogdtmida.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gzsgcyeob.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gouhssipo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/ggilurzxs.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gdzyqanyw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/ghoxftnlh.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gbwzvqvef.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gftrnistj.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/goxpdgjjj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gaicynokn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gsdoyttwo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gsoahclkn.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/ghfvhfvyf.sHtML


<!-- 参考信息 -->