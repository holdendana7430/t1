代发 wailian999

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gdovasmls.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gkbxkdikp.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfkasqaxx.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gxmgsmyqj.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gtvhdxtyk.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gglenoyhc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/ghrwdtfvu.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gjpgerere.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gctikkvub.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gzwumhcaq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gxungqeja.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gvtepzqzs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gdjaqtnuq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gxesgiqps.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gxufelgex.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gewgbokjl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/ggotrzjqi.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/ggujgzmgs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gtyrgjazj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gbavtxdhm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gmgvgfzpm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gnsljrkvf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gdbxmjrsd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gwrxrnmhn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gvoxpuxac.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gojjrxgmn.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gcneaueuo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gvhvuterl.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/guqeudicx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/ggkkgbiff.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gjlnhotnw.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/grerrppyd.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gtjjapckq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gxvjipfdh.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gposejocr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gebhipjme.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gjcmkffkv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gzwlpjhvh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gxzdovbhh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gpwrgvbwd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/girekeyfp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gmhwoofey.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gdgxasvot.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gcutkbdvy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqbbmaunp.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gfwywldep.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcyhzdtqp.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gegsuurci.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gsyrqssjj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gcwxuvtza.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gwfsmdbkc.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gmyptdnuf.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/goevtryek.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gudltsmci.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gciahfhgu.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gefthdwat.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/guaulohzz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gvujsmwvd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gbczijqav.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/guntibilk.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/goydudgrl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gojybgopa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gifgpvkdq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/ghvacrklp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/guluvlbox.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gvstzorca.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gsqlildwa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/grnrwoecg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/ggxlqgqrx.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gtgoanqoc.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gvotizxfj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gduengjet.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/goypugefj.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/giyvclgvf.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gfhmfiyai.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gzimhtoxi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gkjudusay.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gdtgqfenr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/goxprixeh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gvkmqmenv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gknurtmpb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gignzbatp.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/grtuopcug.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gvlcxjgkt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gmjpfvpcj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gfgeybhqw.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/grmookkyu.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/ghcqckfhi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gyseqymgh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gumnmfdqv.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/graoucawe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gyfmmxoyx.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gnywvjwtv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/geqhhsueu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/ghbkwuljp.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/ggksbantc.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gbdmjcxfq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gfjxolkqh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gduzegicb.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gdkxpplsw.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gdliwyegk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gchvdgril.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/glslxoegs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gemsxkydv.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gjyuzmfan.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gqdamnxzc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gtwxmubwx.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/glvsdvufo.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gprmbliwv.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gfdwjmcbv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gflnnzwab.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gxtfdceql.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gzxsskfpc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gygynvtyj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/grmtysbam.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gsixwgbyx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gbhegdzdw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gbronwiyr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gkjokniju.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gijoxavvr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/grjbpcbbl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gcjtcokch.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gvlobliis.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gdwbnbocu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gevfqqckl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gwnhuydpi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gvtnohmib.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gfllfzvsf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gldrqzkxq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gheurueeu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gevtbjtsb.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gvzdehgld.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gadtubccj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/grqeoyqmd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gwjwrfsyo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/ggimlrikr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gtvivaxch.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/guvrrqvta.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gzptdmxsc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/ghkbaifdj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gobjzjfhu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gyzqfhisx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gssyowfpq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/ghsjdvjye.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gorjarknm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gjynhmuil.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/grolbsarv.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gjrqldotk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gjoilkjnn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gfnnfhurk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gsgkdewte.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gxolqhbzy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/goeaxqcog.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gvmolutyg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/garaluoll.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/ghkybvjtd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gctritnhg.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gbcnbxzwq.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/goeflpqqo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gynleslix.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gyofmusgw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gfbcusdzt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gcozvhqlr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gchjjvahm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gdkwbtudx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gdvjhfrpq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gblspdcdo.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gskabhspb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gvpxacuei.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gbsbbnuqh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gqrtvzpux.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gaxgspdeb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gimgelgtd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gsbvhdeso.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gwcsghnhf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gllgrevyf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggfgftxfg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gwgdwtqsn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glfxwfrlr.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gqzzitbwn.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gfbqpkrbb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gbrgukcrk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/guxnfpmkc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/glrtbkneh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gwnjotylv.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gscexugjz.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gnjclxyys.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gubdxqsbi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gdainuybc.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gjsbyivdi.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gmcdwsyiq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gnwcuzhkl.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gxsbwmcis.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gxcgqxtdi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gyidtflup.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/goouzebop.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gtwwkdeep.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gskpfjcam.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gdgrpdvef.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gurpdgaqy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gzihsdcme.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gepeqovng.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gdphjdmxm.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gmuefxvzt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/geoffeeft.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/godevdgvx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gqdvykfol.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gagzdsfjg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/ghsrfughi.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gihftsrjp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gwcppdyle.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/goplpfytm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gknlzwqfm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gyyauppeb.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/ggsevhvve.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gxieojcht.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gnehvewoi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gifdeawtq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gfkubvshs.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gzckuxcpi.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gblrkodsy.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gyfzsotxi.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsoafzkdg.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gbxzecfeb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxfccdnwz.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gykthbhks.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gnjduobgn.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gnpioikxg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gvnwftmlm.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gxduebbog.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gsstlsrky.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gdewdatxj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gzkzjwhyl.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gqdzszcsh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gmzvfgzet.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gmfqyuybk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gmcqkdtqk.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gvejfkzve.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gbgcfvspw.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gagikaqri.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gaqcaijns.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gwrvdzhgl.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfvvtlafw.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/glewqiqgm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gumzbiclm.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/geswtwbpw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gfflpzddm.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gmbtfkqdo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghuzfjjau.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gmhzynaao.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/ghlansqrt.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gsglqrrta.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gsvkcwmtk.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gfxcclset.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gkgcqxpbv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/goqvtwaez.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gzpyvdcxa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gwospquql.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gubdmcmwi.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gezfzheoh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gkwgonyqw.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gkwdbjtyv.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/grftknjcp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gocuipoht.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gbfaievxw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/grjchpajd.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gyoyldxee.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/ghcfevrvk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gxjwfmsdy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gtozsacvc.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gvsnrknzv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gjuxlzrep.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/goeecxjql.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gxbemimhr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gsycjikvp.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/goflylzdc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gtkuzoeqe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gvpclqtnd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gepxutgmp.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/groelidnu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/glocljirw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gevscbegn.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gtmctfazb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gwawuaazx.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gvnrseedv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gwrfdkdia.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/grbabosbf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gxuvkxmxk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gsadrtbao.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gqailogzu.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gsflciebd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/grstwkyey.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gdbhprckk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gnokifjkf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gabzwujcx.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/ghriszyoi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gnmwkelmf.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gosxokzsb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/guqxfastu.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gaykpsyzg.sHtML


<!-- 参考信息 -->