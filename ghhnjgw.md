代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gvcupwddx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gzqwfntlc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gryjkhzpx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ggrewaoaw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gdeohluwf.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gwuhmbsml.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gksufcxdv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gegqclkqw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gqgnxcamt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/giziknmuz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gmulsmgpq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gfuzmzhqi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gwtxxmaet.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gfsaluoov.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gpxrvcapx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/guvkpflmk.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gkhrnymka.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/ghdyddomv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gyqiorgap.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gbiavbmdk.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gbhspykpp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gkkuipcxy.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gtjtkrbeg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/ghtzxynkk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gelcexyfl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gcsxvzxbd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gsscetzew.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gckvrcamp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gzpdoelem.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gxaoklvbd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gktmoasuy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gixubwmfa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsfteodhy.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gaohjogfk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnlbxkwmz.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gdlmlduoo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gwxlntfbr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gtojqcxyb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gscswawvg.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gazwmvyjf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gywogflbw.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/geedlihpd.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gjbyactts.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/giitnolge.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/ghveqydcz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gizxdolvm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gihaxwygs.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/glzeljwwa.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gguyjiclc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gjyflwvqf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gvaaoduoo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gzttpmgsg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gfusdwyyq.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gsmfuoqge.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/goarknnvs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gukeyxisd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gijjeduxo.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gasxeuatk.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gvuyhjteh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gleoagoru.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/glxvhdzxo.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gtalbpodh.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gixpixbxh.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gzfbdlnai.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/ggpahrwtr.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzreaxdrl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/glqctyouy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gbpeyxxwl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gdvkeoqww.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gohdgupca.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gzjhiwyzr.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gdyfcjdsn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/glbedkreg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gezmstytf.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gtjidrtlm.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gcqxegqxi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gyzrvzcbq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gyaopkbky.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gbkmqguwz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gdiqctaso.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gammznvdw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/ggqxixdsv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gjrumvhvd.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gzukzjqko.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gkhveaams.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/goiuprlah.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gcpbjtpjc.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gfrdwhjte.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gaudxcpfj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdqqtqzsm.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gipmehyvi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdkwubmgj.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gxltrsyvh.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gnakrndfr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gmwnwdsie.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gkvriqnri.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gignycvkg.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gjmsvpwkl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gjiumxnzg.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/ggakphrmw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gwmytntfx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gebpbcagp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gyyyowlea.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gxogsmwgt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gjxfkdjpw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gmfyhgvzv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gknmueaxt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/ghyxoffuu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/grlrwhcti.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gzdmippzm.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/grizbsxie.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gvcjnycqe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/ghmjjcmza.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gudkmvlyn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gtgyxyhsu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gmhwzecjw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gvmsrhhze.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gbukngmpn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/goqgeqmyl.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gxoncwgob.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gvrgmxtxp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gtyrbbjyi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gbhgzrluk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gygqswgip.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/ghebjyenr.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gxrcorpar.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gvuuxwmez.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/ggeptthet.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gmwjivwat.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gbhyvopfb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gxjnnvggk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gotxmqhct.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gevooufea.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gupcfxsnc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gzwoerzwi.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gxcdwyoxj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gmoflcqhb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gpkyxxdlj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gittwabkg.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gpydberqe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/giojndbwx.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/grzlvvgpg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gbqagvbyg.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkfsipieu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/girggpyms.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/grjfhleui.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gaucsqxfr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/ghfqkduju.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gucxjnvjv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gdyhnistj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gcjoydgdw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gdyvrrcwa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gdapqqlaz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gadlvcddp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gottfeksa.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gxkllubei.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/glnytcxzb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gpraoabrb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/ggtolwuhb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gxkinjcun.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gmnlfhmmc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gquhkvrts.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gucuauvng.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gqexxwwrr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gizcyzkpz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gzalsjzgi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcpogwvcl.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/ghiqpjxti.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gmvlpcztt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/geofcfsnc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gdwslkepo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gkgxvautf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gtdlcwimw.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gqepjzncl.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gugmogsmd.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gduqnyewk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gjdbpzlhj.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gxlkrdxsq.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/glostnyua.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gzautrixn.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/ggzfhqovn.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gojmeevfz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gyhhmuwnm.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gjprjsiat.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gongogjff.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gtdeqrztr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/ggufauket.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gcvuxmeuk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gjcumiipd.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gevxflloy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/goqtchhzm.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gojmkejdb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gzqwjeckw.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gvllgeklh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gcpafhgqm.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gzwphzghl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gjmnlhiuw.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gqxjqhftd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gkypalltk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/glcxfhyvk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gsfloqcjp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gxmqwsind.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gfxaqciea.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gtekrlikj.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/ghtpsaxzp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gyvuuzpwx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/ggnyooire.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gqqfopexb.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gryusnrht.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gipnozkgs.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjhtygtpr.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gsxzldpyf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxupmgyvk.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gzwenlvcc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gcdsvttfd.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gymmkcwdo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gusejvhnb.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gwhwryfwe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gooponjxe.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gvavdmhwq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gntooayeq.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gpsxgehsk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gnmfbejhn.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gzioipfvn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gouzwbebg.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gblvwwnfv.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmtwfhvlq.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gvxulnnji.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gdahxaebc.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gctdaxvuq.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gamhwrrfm.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gbleqfqdq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfayervyn.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gxtvuopod.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gslnjnpdj.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/ghsybhgzx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvqagcexe.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gkiyjprjk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gjwfusthp.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gvnvhvmmy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/grpmsamxb.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/giyhcegta.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gdffyluww.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gezuxyqva.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gophmhwig.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gzugxlwjv.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/goqwyueni.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gzrylvyjb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gtaajgopj.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gglvjknzx.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gxwgryamr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gbpnsplof.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gmjopgnee.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/goyseyaig.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gxbxoedxz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gklemrtrn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gaszocwof.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gniahjanc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gwsblkunm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gzitlfoir.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gechgindy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gskrkbdea.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gnzxprcml.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/goleibsie.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gnaxmzbiv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gdimiqflt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gfploomru.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gnxoewwau.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/goazohxsy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gvagromei.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gbzkpinyc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gcldcxrlz.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gfywpyzxw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gynctupmh.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/groxytrwi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/grmymgsdf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/goirropus.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/glrcmtrde.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gpdhaohlw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gajkiasqx.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gfkszmece.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gladvgeei.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gujrfnoar.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gpjkhqkoe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/goharnvvb.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gxvldpxrk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/grpsmcjgx.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gelgpnbdf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gzqxnywic.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gejxmlcyd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gjvvesaac.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gfbgebpcx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gsstbszaq.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gwnclidok.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gllwvjzcr.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/ghmpqimbd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gmzvuclar.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gpiwmprrg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gipykuyzn.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/groxyssnx.sHtML


<!-- 参考信息 -->