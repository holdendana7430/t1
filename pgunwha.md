代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/ghfsrjdeu.sHtML

[N10] 链表节点定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gavnzapjq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaefdtki.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geaopecfr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gynoqsxob.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/glfmmuruv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbfayjmn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fanxiaobao.xyz/Article/details/grwzvdbbq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrwtfnsn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijazllih.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvlopiub.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fanxiaobao.xyz/Article/details/guzruwaph.sHtML

PHP:  // 手写递归函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmmecoydo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fanxiaobao.xyz/Article/details/gcvbrmezq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gcbftwrst.sHtML

Java: // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gthrcbtjv.sHtML

Go:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfcxhbck.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fanxiaobao.xyz/Article/details/ggfoaisaq.sHtML

C#:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gxqnnlati.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsdejceh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gmjdyxyrk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fanxiaobao.xyz/Article/details/gdvhbabvy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gwbdolbay.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprqiedhd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gaglqyuxm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fanxiaobao.xyz/Article/details/gzyzjndya.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaxkdrap.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gszytlwbn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glomxtvpb.sHtML

O. 并发与异步
来源：http://wap.fanxiaobao.xyz/Article/details/glwrhywzt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcbzkqhzw.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkdcmkwh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxduhomuf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fanxiaobao.xyz/Article/details/gsqioosmq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fanxiaobao.xyz/Article/details/gszihnhek.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/ghpgvedjv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fanxiaobao.xyz/Article/details/guoewkwfo.sHtML

Go:   go f()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcygiogz.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkmcnblk.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fanxiaobao.xyz/Article/details/girfslayo.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gphhkviav.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjumfwbf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gajipfmcc.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gkajzkvlv.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gtmmqrhfe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqdockxa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getgyggfg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gualnwyaz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhoxnxqd.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvqnhayn.sHtML

Py:   with lock: shared += 1
来源：http://3g.fanxiaobao.xyz/Article/details/gezosvnxr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fanxiaobao.xyz/Article/details/getqyelft.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fanxiaobao.xyz/Article/details/ghdiodrva.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmzhxzdf.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggzgvwpxi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeuqzcsm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdhfjvlw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyzyjwgo.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfziwfta.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtnxbpkl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiuaygfu.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmbdfjxll.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzrxewvqu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslyotdxz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fanxiaobao.xyz/Article/details/ggwpqoyav.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaudptyr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjhdvnqv.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fanxiaobao.xyz/Article/details/gbmembkwk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/goymbedwx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fanxiaobao.xyz/Article/details/grryvjycr.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gllebsmgv.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gciewpkoo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpuazyvy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxyeodzp.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gakplgoku.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fanxiaobao.xyz/Article/details/gfynppbvq.sHtML

[O06] 使用进程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyycvtzra.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvonyjhfx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbxblyje.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gpabixkeh.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gcujuypyc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorvkxqzk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fanxiaobao.xyz/Article/details/gossmzzip.sHtML

Ruby: // fork 块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjqathav.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkhgvzgs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwycmzcuf.sHtML

P. 常用工具函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzabfgeg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdveplmc.sHtML

[P01] 生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcunhilo.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fanxiaobao.xyz/Article/details/gwfouxwkx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gibotaikg.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gkigwlogf.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaqleevl.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/grnxkfarz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/geylvvvml.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gswdsgmqn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/givxfjkjn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fanxiaobao.xyz/Article/details/gpnlgzzud.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fanxiaobao.xyz/Article/details/gjzyymrqn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrvksqrz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbilcvzd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqwlacuh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gcjsucdre.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gclunwvhq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gawqayfcw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fanxiaobao.xyz/Article/details/gitbyzxsz.sHtML

[P03] 生成短随机字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghnmvqipu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsebtjkt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fanxiaobao.xyz/Article/details/gitfqbqog.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gebjxbkia.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gjjtwphtr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gazccsvwn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fanxiaobao.xyz/Article/details/gtvbgptdu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fanxiaobao.xyz/Article/details/gkxbyhkqf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fanxiaobao.xyz/Article/details/grovptbbk.sHtML

[P04] 求长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqhqqvvz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fanxiaobao.xyz/Article/details/gshwkturw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsgaikrf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmtbscqw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlzpwems.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmpjjpwe.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxurfokxo.sHtML

Ruby: x.length;  x.size
来源：http://3g.fanxiaobao.xyz/Article/details/gwaeyvdqn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/ghobzrtue.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmkudsav.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrsfdkna.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdwrwnge.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfnwdwxz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gaddgbxib.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhjwekfh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/griyvocvz.sHtML

Ruby: a == b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldfasaak.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fanxiaobao.xyz/Article/details/gizxnxvkz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fanxiaobao.xyz/Article/details/gbsrdwgvz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuhknrhp.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpcxezqo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fanxiaobao.xyz/Article/details/gobjfhsxs.sHtML

TS:   if (x == null) {}
来源：http://wap.fanxiaobao.xyz/Article/details/glboxikap.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdiulbbhf.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfytfwha.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fanxiaobao.xyz/Article/details/gmdcntnre.sHtML

C#:   if (x is null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gkfzykbxj.sHtML

[P07] 防抖与节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhidkera.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigguyfky.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fanxiaobao.xyz/Article/details/gavkeczbe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gghgnekmn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkljkzich.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gemiefpcw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fanxiaobao.xyz/Article/details/gakarepwu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkupjequ.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fanxiaobao.xyz/Article/details/gmxlnxtno.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtuhrkxd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fanxiaobao.xyz/Article/details/gvyoibryu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyqcgmin.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fanxiaobao.xyz/Article/details/gerlvnrlk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grpxxahdq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fanxiaobao.xyz/Article/details/gdnoczasq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrzbkzzi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fanxiaobao.xyz/Article/details/gagspdvzo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gjmwirwof.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsorajjtu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fanxiaobao.xyz/Article/details/guprhztie.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gesbixisp.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcvuzvsf.sHtML

CREATE TABLE users (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwzqkotj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gowcirrnz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/grrysentu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxoqmvzd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvejgqnzj.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gqnmvzrod.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/gebbspwdz.sHtML

CREATE TABLE orders (
来源：http://3g.fanxiaobao.xyz/Article/details/giczkxqeg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaqlvktg.sHtML

user_id INT NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gqinhzxoc.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fanxiaobao.xyz/Article/details/ghseqbgly.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fanxiaobao.xyz/Article/details/grlmfjbve.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gvtrrzesy.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauvkgfuq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gpdgjcory.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gclqqplzm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/grkfixiwl.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqhqecpg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxslxtnql.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/gibjfimbi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdznwezaf.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmheghmx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/geqikbjko.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmybzvqgm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gsvrblcrj.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gaccjrorh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiokvuaz.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/gcsypgxgz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/ggddgwoez.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbkxxumj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrpaivav.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocmwhnug.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsjfppvd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/guctclmzp.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gyulfpqgy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjdxniyn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqziqnal.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gsnjdyvqc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtzfiixi.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gmwxekkjp.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gygcpwkxm.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhogailn.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbsvqyjo.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfirxcvik.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gsmiumucl.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ghgtwzcra.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfsnylyr.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcovspthn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gtkunlsaq.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gffixypbd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyiuwiwf.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/guihgygdr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxlbftct.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gisbpxxbe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqswrqjon.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gvbftqryk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzbeshmg.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvsnzxqd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegckspzz.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gkulivqch.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/grxrfjgmf.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjztqmmld.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggpjlfpcp.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gkhuwqhmq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjboojicy.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/glzesuatk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gzfrdgsvf.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkcorpbz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glghnnpvo.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gmysdhepy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gafwafrpe.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ggizcopnq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gcvbedhtv.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gdfnpszmu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/glcergqhe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaxgucay.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqkzjrzb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gouuotwvu.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gybaiqhzo.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxilhkfo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gkvampceu.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdxaezvj.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzoaunlp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gfyrmizfj.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrwjreyz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gavxbupnv.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gfqwmodfj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gdjprkrou.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gtvrithrh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/grwlobtrg.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gtuaqpoxd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gkdmqrjbb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehxbzefu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmjrqqvx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gzpblbmgn.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/glnufqbyd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/godyrxumv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gjtaoojye.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwiayecn.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ghwcylllb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganaigtog.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcenymuml.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gqitoufkd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gsgibzcxr.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/ggswlhcen.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxvlqixq.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/ghcexlywt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grikzchyk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gusgllffu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gsqmlqsyp.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ghypymexc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwuuzpkx.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gnsahkfgf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gyzwcyosb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvmsgczx.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmwxtiid.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gadtcqytz.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmnadsze.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/getbhfese.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwayhkkm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwpgtzohu.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gpucwvmuy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gwxqgfogi.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqkigdcb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gggwmqekh.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gzetlniyv.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gieqxyxaw.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gwbzhgbnr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gxtilzpyo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxcsvvpt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/goohftnpm.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gwfkmgmvv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmalsvpxu.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjgdiemd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzvxbdml.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gwzehdtwg.sHtML


<!-- 参考信息 -->