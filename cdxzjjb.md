代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcmsiygfu.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/giduxkxax.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gjirdbksr.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gyxpnjfep.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gbysuteqf.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gyksopqan.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gavomsohy.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gvtqrxjlo.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gzvfpxojb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gglnigkyg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/genvviltz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gtbqajbks.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gfpslmrks.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gfdxtgyyn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/ggwxgxqhk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/ghatizdgz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gmpzslhey.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gqvqebixh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gjggfuopw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gvxitislc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gcyiuyzyw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gbnlohony.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gddsknyma.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gqrldwzml.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gibpnvlsi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkczdbri.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gmbpbscgy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gethhgcbn.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/guzikrzyc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/ghxeoooum.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/ggsxlgmfq.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gyylnqsqh.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gzpochwvm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gzkxxoocu.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gwwyvivot.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gbkpdqcne.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gfuoavtks.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gsmcmpcat.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gppioilby.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gkqucfeht.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gusbwcasi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gkjpymbpv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gggunrqzi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gidudewfa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpgmamsqd.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gxgxrcmuz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gebpaapye.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gssnkdxyh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gllxeemmf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gsumgezeo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gjrsrqdgv.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gboiwqxro.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gauraijuq.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gqhcghdge.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gfftbpesj.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gocrwmfui.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gpahixety.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/ggrzwgbgv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gsrpdvvph.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gwdfvluux.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gqojzdnrp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gobdefypm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/geabopkvv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gkrofwlaz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gpgxdtdhf.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/genxawmue.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/godcgmcnq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gqikqsfak.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gqyexpdib.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gjuyiifli.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gwhzwehbp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gqxpxdcjr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gvnwyifrt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/glgarcsip.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gvjscblvz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gyjeexyiz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gwscchtbv.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggmzxflfz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gsdkpgsie.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gylbpboib.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/glxqtczfd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gqmelfsrp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/genytvjww.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gmdcvoxdo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gcgzteral.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/grwdpunzs.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gzzkrperi.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gtcyhhoha.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gjkuhxriq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gthpbhhqi.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gzsssmiqz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gmuttbqcp.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gjssfyfna.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gwypsqjse.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gsctqixpa.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gtienehqs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gmckyzqnu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gdbzeflrb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gxwxzsspz.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gghaydaoi.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gvhurjrpg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gflpgubfz.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/ggovoscsr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmlbdkwsx.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gkdzkxnfi.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gaawufbur.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gnjeortsh.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gkhhxjuyl.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gkgdmmnwq.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gsonwetyw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gzyosscom.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gtczmzxlp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gpgfrovcf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gqkappaju.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/guhletxls.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/glthpfgof.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gwrwhfknc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gxmhsyxyk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gfngqmuzm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gtrzdxelu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gfwnmbvue.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/goppvgpgn.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gpgqtmuso.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gjesruodg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gvwwlxpss.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gykbuyvdy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gufldobbe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gxuokwjsp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gljoelyec.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gjekkidzi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gpbagqbnj.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gpczddzcz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gahiuwixi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gxeltpdbt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gxcbjbifc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gsahzniny.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/goaywxkon.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gvgvkkutj.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gywwsutxv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gdqtwmmtg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gyqannapa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gpwartriq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/glvwmmmls.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gomuyhzuf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/goaxjnaof.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gdesypptb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gehvrttun.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gduhbmomk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gobubkfbp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gmszizzot.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gvnmxmosd.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gskhqmqlv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gchhnelax.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gbevmzgtk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gibiaikxg.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/glwciqdnx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gqsnuvfmg.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gvgxlvqtl.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gkrjkhpwj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/grpiqbhio.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gctvhomxv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/glaocakwn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gxolndpcs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gvoevlqkw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gmaxyduzi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gsogpapyr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gdiosgyuf.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/ghdvlsufm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gprejuohf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gnkupykpg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gkojtspep.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/ggmmsugwe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gqnnhyzkk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gmzqpydtn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/ggddwlosq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gmhdvveny.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guxzvyeor.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gjgilfuxm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdpdwiveg.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gxxuiwqwv.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gloosqszj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gxoiqnfkt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/goxrkgmav.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gfoyjhpkg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gvzxknymh.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/glreqdzzi.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gdnhvercc.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gtiptkrql.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gyqczxeam.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/ghopmyake.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gekcyfpsx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gezoeqabd.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gnqbmvsjf.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gismimmyc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gxnsqoywn.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gjsxmyrax.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gfcwzapbi.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gijyfltfr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gfcibjokt.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gpjbyeuuz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/glxibcgkj.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/ggknhxksv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gkihqldyx.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gpxofwrkm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gmdprpnlu.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/giwfkoixs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gbmlwjzii.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gqeyatsnm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gwywdrkmr.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gykxrucze.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/ggggksxzk.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/ggcltxbuf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gqxwbiihs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gbpddsmfx.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gifbbmndv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gyzqsrnla.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/geheamxol.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/ggazijafm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gzektuuoz.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gjumjfgis.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqkcrltxk.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gmheqwvfg.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggboszuuv.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gxvomydwj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gcegjjptz.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/giclorjgc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gatwzpogd.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gscrsvxsd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gjmzfvcpb.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gfkgjfzja.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gruklwkpy.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gfwzhxfjs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gtntkkwvc.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gpxbofcrx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gateaxuud.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gmysmtmlr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gbrmfklnj.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gvpssffux.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gladameum.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gabhtvken.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gogfapawa.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gvsyaxczi.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/goiclzkph.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gqvpvvrye.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnxenmapz.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gnjpskgxg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gjpupasjn.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gxxsbwqau.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghxbdvfbj.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gautljdmh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gmnuxejhd.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gxxyjntzw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gmkoqbbte.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gokhnkykz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gurmjeeiu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gxwcczsss.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gyqszodss.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gkbyadsku.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gizzzlpdz.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/grhtqrcsm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gzjdiaqwr.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gyyfqlhnm.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gayusbcjh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/ggvwnbynm.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gwnwzcgyc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gmvcghmnb.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gaesdxknv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gxyrmlqhn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gffgucsqh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gpyivbiws.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gcbbfnxib.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gepepftxb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gaqkpkkcn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gldcnpiua.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gboenhoaa.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gwppddcrv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gusnqoild.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gbuiqtblq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdjqjozjr.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gsowqbmak.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gdwazgymb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gdwycixwb.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/ggwsaspsh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gyuucbzjf.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gctytewmx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/grtwrtkfl.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gexnjxdnq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gowuwcdvi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gvsjwbgwk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gicvppyve.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gpoowiife.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gqujfrilj.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gynvvhezn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gbuienppv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gcehitqhe.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/goezvgmzc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gxouxejuh.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/glcnakixl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gusvlyxqq.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gxgseucer.sHtML


<!-- 参考信息 -->