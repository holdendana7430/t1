代发 wailian999

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gnwkhhywv.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gkowsytkm.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gddhucpll.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gywumlrgl.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gtcnitvjw.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gqkbzzhkl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/ghapkkhwi.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gegbgavby.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/ggjmejqol.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gtwrgzaxz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/glubkszzt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gvrxvypsb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gjlhutzbh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gnewqxwec.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gzvcnszfo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gourwugil.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gcdoaabkw.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gminkipdg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/genqpykaz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gqpdazxyx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gyebdijrb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/geilzougw.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gtrvnmrzf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gfmizilmu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/ggozymrcb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/geavxhoqn.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gsokttmxl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/giodpimfd.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gqfsweznz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gynokpgee.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gwuzsjdmx.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gglqhjhwf.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gprayezii.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gwmswrcjw.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gmbeixvoh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gubbqnpnx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gwehwidsd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gkbetxile.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/grsdcjrzy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gqwuqvpom.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gbxkmdnnw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gevipaktg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gebqqkcsm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gqjadmtzv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwmvjtjte.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gueckiqks.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gusgwbhsw.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gyfoolgqk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gsagtjunc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gmjcpebfb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gqoqiwovr.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gykcempnc.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gscupugdy.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gtfxbixvk.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/grcmdkxme.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/ghclkezrt.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gtjalwbbg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gldqxeisf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gacyjyjzz.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/glvmatioe.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gnkyhtqyr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/grprzdcyv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gyyzkqegd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/ghjaxlqzn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/glkuycdct.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/glbjusgzq.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gptpulrqd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gghrllfvr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/grrfkvbfi.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gqruuhkov.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/geqcpzazd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gjwmkialn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gumfaitbt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/glkkwmalt.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gvpylmngi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/ggdbubawh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gqxfglahb.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gzztaxkvv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grnxgzokw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/ghmzrmboc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gmaekeqcs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gujiswgun.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gztrqovop.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gwdkppyqy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gxqrbsowu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/glrfywlht.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gabrcrqwo.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gdjgsmfjo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gclzzfryt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gbqtbrycc.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gzhignjpx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gyxdqgthb.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gieuufbhk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gbhmhwddj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gznzxkdlo.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gtcgqqbpd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gottteuij.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gctcmumir.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gvtttfecq.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gptpgznnb.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gpxboxdew.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpwnnoetr.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/grefhzfiv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gibuxumfo.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gsxifnfxl.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gtudacgky.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gwiffvxwb.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gpnhccnql.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gtdoajdbd.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/ghaqnqzyl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gwfgwloxi.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gtcmzhxml.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gbuflkxsp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gimcgatpn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gyohfjxem.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkoeasbfu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gacsetawx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gzinqgidz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/ghutovlug.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gxamgebcw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/geghfckot.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gnirbisup.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/guiszjuxj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/ghabbnbos.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gdqeuuqha.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/ggpxskhec.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gkgnkfbxm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gacyxmizf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/grkhwcjap.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/guxkgnqvi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gnejfgcwh.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gcpaatzuz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gyrfjbukr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gtxsgrjjt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gjkdthxuv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gltqrqdhb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gjlwkwost.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/grjxieoov.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gifljaqls.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gfmvefdls.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gmmrdjigs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gximyiino.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gdeahpkpa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/ghfymfobo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gwnoicldm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gohosupoo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gpchcrxbl.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gkmrlqxsu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gmgjmedgr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gfdghteqg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gfpjrifdi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gxjduscbe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gjvrclqij.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gofsxkblc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gmrymixit.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gwzkmkvla.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gyitvzdqe.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gdyrhdmzq.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/ghgrbpkas.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gvzqkuhpb.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gzvuqonmn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gdlwzzidi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gnzqxtlel.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gxtegxost.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gbrooxnth.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gzsdcdmum.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/guhqmwejd.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gikgpfffm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gpizuckfv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gzhhoxfwz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/ghablimnr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gkemnyvyq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gpkjvcdmo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gojheitrk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gmnwkzuht.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gfwsbawma.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxcbhtbtz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gqsfbwcmk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geqscpenv.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gxwxcbknf.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gpgbakehy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/goceclpnj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gmijtzkqc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/goghgycft.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gbhwjsatt.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/ghpcllkvj.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gxovutsmx.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gtvmqxwxj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gjhnzfesy.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gezwiiupk.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gxealoakv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gmawuerul.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gmkdplpxo.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gqzfesifc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gdrqbfayu.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gpmonneum.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/ghlodkmhe.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gkgjfwjau.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gdmrrsbfa.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gpqnwvntt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gbifuwngv.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/glbqbbygs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gnhusozbn.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gombkrtdu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/glwdolthk.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gntikikuk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gxuebtfcw.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/giualzzbv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gxyroglcg.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/goqvfsowl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gslybbjli.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gwfqpudlf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gntwudjmb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gjcdbbkpy.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gvwcrprnd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gvnkzcaiz.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/guhomecbp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gffhwrnqt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gzbhrseuw.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gslfdnpmt.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/ggevfcgwm.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gpbfpgcqp.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnunqflaq.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gcorjhorn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gjnhhbmpu.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gbbfklhec.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gvbeupwah.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gliblgqrs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gngddipup.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gidbfvksn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gppqjneyn.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gexbcwhsz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gyhxkvamk.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gcgfybkml.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gfnyzyhgq.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gkgerrijx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/guhhtrzmb.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gfjbxrwuk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsilbksis.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gzasntoiz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gizkemfjc.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gjljfzleq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdxcfpdcy.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/goqanwbxu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkdpmifhy.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gsmvkdpjf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gjghhhnin.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gdinxjtth.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gwvkpeuwg.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gzuifcjtl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gityjnxke.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/ghahroqdy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/glitlfdmt.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gbtuymjpw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/giuuhonff.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gxqqluqub.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gtblmvbwu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gkxqgqyzv.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gpaphyfcg.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gyiznapvy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gruztqdyr.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gkqqimzmr.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gbxfwkcsl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gmkkmgbmj.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gtakqqhum.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gfglgcxvf.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gmtyxfwfm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gqpnhfwle.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gkfdvspmn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gihhcdqzf.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gnydxwsbg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gwxaappev.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/guntmhjul.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gauncrnnc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gfsjgwbhe.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gcvgwazfr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gymbdgwff.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gfowbdgqf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gipmpcujp.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/giwreaeol.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gxqqzrivp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gftkoxgrq.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gqdbwokak.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gzumekagp.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gnyuccmhq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gbzkjllll.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gxnxujpuq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gchzaqujb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gddddbsjl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gczxilyjb.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/ghfyyhpmb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/ghyhbwwhl.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gfwcylnke.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gylkgsyga.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gjsewmdkk.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gucdyzrfg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/ghyhneqve.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gcccwazyi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gidijiwep.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gbdsplswh.sHtML


<!-- 参考信息 -->