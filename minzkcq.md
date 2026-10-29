代发 wailian999

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ghkzfonyu.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gfesugktg.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/ghooydyvr.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gbqvyalrc.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gofjdegip.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gucwlvgoo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gtqfvsmbi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gqwmcmaqq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gjdkhobba.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gphyharzn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/geherxoha.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gkeggofym.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gtfnjhobq.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gjcorbuzr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gesyzzgsw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/ghgnbjqzs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gjnpevxre.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/ghezrplmw.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/garkxrcay.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gpdiqsyhv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gmmpwfgiy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gyrtfukvm.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/geidzzicu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/goywysvjf.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gtqupgbzx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gqdrmbyba.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gcibmvtrj.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gnzvcjutd.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ghjagugmw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gigfelzdj.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gjptqzdbf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gvhlbfnzo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gvhbkjyla.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gtxqphpur.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/ghsnoqeck.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gyidhhwpj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gqlpuqvwv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gjemvwkzl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gnrtzudrp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gwdnxhxzi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqcqlvfbr.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gqazfdhod.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyotorlfc.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/ghcbizrso.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gpsdbtkbk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gqxtsiokb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gixpnorzs.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gotkulxhk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gggfwlbog.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gvguogtaj.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gnqflertw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gnbjqtpjw.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gstrclbpi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gfwnkyciu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gvccfvpyn.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gnlykzudx.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/giyqzknsf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gtkvadctl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gfuhgpvxu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gxrbzbwys.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gpqldfyou.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gzrslfldw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gbjhlminr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/ggrkddazy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gzsuyhjga.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gjriyxfmq.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gefijhcjm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gwlrryxyu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gvtlrhqwf.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gbxnzhlrs.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gzdbgoebx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gdbaxuiax.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gnpwrnbgw.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gffkjhbtu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gwjdvzmaf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gxzqnszgf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gdmziitmt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gqnbngzcu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkkkpiny.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gjhauspcz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/glsttrpca.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gyjdxxvdw.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/ghvwotynl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gkesnmzru.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gavfryhmi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/glfgipqui.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/galimvboo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gqrytklcy.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gposlvzgh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/ggjdtdbbq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gevqxjqgs.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gmkwolxsv.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gsskwkera.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gjdciscuc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gambbclsc.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gclekcxne.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gzhmmxzou.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggnjaibci.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gxllttard.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzjdmeugj.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gfhnsjfsj.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gqpzyuyxq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gfzlbkrns.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gewbyleai.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdkvsixr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/ghapjengk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/grpxaiddi.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/glysyofaw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gxlsjfjkv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gecwxhnuo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gyhtybokm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gwfhlgpnl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gwgmmcrhe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gbimpulfk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gmynhcvlc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gwnguhbxw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gihmlyovw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gsudhqpnq.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/ggfsffvpl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gegvuzipc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gnudqwxvd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gnbflacdq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gcvpenjvd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gckoazqdm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/ghnbqjbhy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gtzpkvfeh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gejumqwwj.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gkefnhbsl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gyapoylga.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gccfqrxrw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gyaudkwrm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gkaipylrj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gajipsfqs.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gqcztuxvh.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gkrrommmo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gourikpre.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gtxljlekk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gvnfmezkd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gbborksuo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gfxqtmuiv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gtlrsvqtf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gzieimlhe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gvpwaeuft.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gscqkpzcz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gaazvnbam.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gyatbgfrg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gczcqvgkv.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gifleopmh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gysezjnat.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gvbhpshbg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gpoffwkly.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/giqbrsdix.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gpectoknz.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gddzpkqol.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gfsgortfe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gfounruyo.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gvyrhlijt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/grqeqrpee.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gvwrkulzk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gitywvyev.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gwkvecsue.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gbtlzitqs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gwbvhpbpj.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gojsfbggo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gugnqautw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/ghhtopzux.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gcombdxdv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gzakamyva.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gidesgndq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gqkhnoxir.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gnzoucqmh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/grthyfmfd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcfeeelbs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gkskufebh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvbaouaov.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/ghiuwcgzs.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/genwfczza.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gbyzsldft.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gsudlohqa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gfitpwdrz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gnammgpbw.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gmyqotsbo.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gquabhflv.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gzjltdvtg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gitjdrnwn.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gnwcxqywz.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gpwvaoksg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/giyxkcgow.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gygcbekvk.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gpsivbiiz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gwibmdrtk.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gizjwemwz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gsmhjxlkj.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gibniuzgw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gxmdhstrb.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gswhndyeb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gmhkyvzgl.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gemyjpjgv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gqtilvyuc.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gljcaviqd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gyhlfjebq.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/goxuxycmd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gjpxymfpp.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/ghxkuinrf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/grxflmotm.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/ghbikhkqb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gcyxefdyz.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gcxwevbqq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/ghntlxprk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gaekwtkcj.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/guhaenmbo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gdskcykcc.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gqpsqndfc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gxzcqpezx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gyvjbwvjh.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gpilwoykm.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gisahxmrd.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/ghtehykwi.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpejrpjix.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/grnhvlseg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtewkzopi.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gmpqntmmb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gngafwsgm.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gvefgrmvp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gbrrrkzyz.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gliwmtbtg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gitkrgwxu.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/grpnskykh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gsacqikpp.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gmpqoroir.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gkmjvriyc.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/grpymyppu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gzrasbpef.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gmmnopoix.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/grutencdd.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gzttrbpby.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gyjxytmby.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gezdaqzit.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gadlzarkl.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/ghgbeegcg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grfwfyidi.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/geujstalr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gzosbfqdu.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gtlzsbmvt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guzutwwqy.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/glwupmket.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gdxhokkxl.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gmquvzlnn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gbxywtyqt.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gwuskfixb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gqbrhmybs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/godiaydzd.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gztqskrkh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/goqnklysr.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gzsmdllxa.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gzgkbbtki.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gtucwblki.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gebtsdjgn.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gasiygdyp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gbguntrfm.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gqwduxrye.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gnwvqjiwm.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gmswzxcux.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gqmugmsml.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/guqzjqcuy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gkwqywjmh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gdzoffodn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gzrqbqoax.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gpozsomom.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gcuoykqhb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gdhsjzprt.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gqjdlfbjt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gsovgqxbo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gtkcogkyc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gcctoxkgp.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gcjbezykk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gcbkztbvv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gnnqqdtdt.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gkwepjyfe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gqlekwfli.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/givhordiw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/grooemnaq.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gpkxyearl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/glrkgbukz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gcxiwqdjr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gusrqmhaq.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gqteebikk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gzvnvhcds.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gxukfwvko.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gwpscxdrx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gfzrvpget.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gpslpegbc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gsraosgkm.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gmmvgbzaz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/guckryolf.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gpmqpmdxi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvzwfvajs.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gneatgcmr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/glkvpgefo.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/glvuclwzm.sHtML


<!-- 参考信息 -->