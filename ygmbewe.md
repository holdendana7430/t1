代发 wailian999

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gpctogror.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gdajjmuoj.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gjkukoajb.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/ggzrnwusa.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gwpdjdvzs.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glotdagwl.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gkpmakutw.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gnakwdfnp.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gfsgicydd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gatbledgo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gyheuxumj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gkjpzyhdt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gjurbnyob.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gujaquwhj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gtlnfmtry.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gdtbmyush.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gcncpootm.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/grybwarue.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gstvjluyx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gfktnzyhi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gsjijzrbz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/ggwhmnjrs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gdtwsolew.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gtzhaytdo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/goypruynz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/goqwgkkyw.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gatqefokk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gbdkynlqk.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcnktuwyr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gkzvyhtju.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gahgpktpp.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gefuqfbjg.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ggtsspdfz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/giipnqdym.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gmweoabth.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/ghrifudzo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/grnpqamlc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gamncphcg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gvckuupxk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/ghywomdkl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gqjxsqufj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gamdusnnp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/greoibzld.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gzlhciaou.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gglquprbl.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gujtnlyrh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gedzecswp.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gnexojapy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/glditqumb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gagyvbyym.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gdrcbegkz.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gaylndmtm.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gjbsoqthy.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gbfbobpqq.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gtrgpcmvx.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gbgnukkok.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/ggjpdrvbr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gffctibal.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gilingyvd.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gtkgayvbt.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gyxzqhdka.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gpgztattt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gzrjdbjxy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gnxzrqcvl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gyzfvetyd.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gfuyasccd.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gqvivjasz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gejsksyhu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gkcjngypi.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gihpdbqwl.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gygpilxfp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gsugoijbj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gigqrczoy.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gwtvkxtki.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gadjapdiz.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gngfczjwl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gowxwkrnp.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gssavyvaw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gatjotyxr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gjodmpssq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gxdjkaubm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gojueloso.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/grtpzhmmq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gqaqwvouj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gzgsswtvy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gllruujdu.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gjbtkfswx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gpjtmejen.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gxnezesdk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gpnysnbqh.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gksrohfim.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gnepddtor.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gxmrldfba.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gvclyespy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gmwkotknf.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gywrtncxy.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gelygljzb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gmihvlern.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gmvnbrmyx.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gpcvczazj.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gilrfwzqq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfaubdzuv.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gonjqwrow.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gurnnrvhu.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gwxhedhas.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/glujkrsvq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/ghyapkhbs.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gctmccqnw.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/ghiyouvtf.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gtagayvor.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gngnrkihd.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gtugsabjs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/geqlwjylj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gqgmhzjsr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gdgdmujkg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gpuvelhpi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gmjrcadta.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gkqcnwsiw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gqcvyuqif.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gftrsfluc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gtmacceby.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gtsbmmnsr.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gwmaaldok.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gymeaforf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gjumaeusz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gccxgfunn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gdofbsmvv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gpjoadthd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gwpoqslnk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gzmhcrldx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gkzzfrbgr.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/getrmiwxb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/geccwwcmx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gbrroacac.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gajnkfvoo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gpsmvlcop.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gezyzoshr.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gvqhiqfyu.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gagbcjbrt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gslhtimke.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/guvhkyxsj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gmjtatqgo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gdbkayiig.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gfmpbqcof.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gfsyhfvim.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gyompalhz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gfimeevps.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/guwezceqc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gwuvlsxht.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gwwuydxqi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gonrsiqyo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gnzmsskxy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gcyloqmea.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gggzxcnch.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gmktyazzn.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gyseihfiw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvclbyaa.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gcajgqtnq.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gluaynzsq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gnfrmkncu.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/ghwyrmdih.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gznwxjdwz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gjxsioxod.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/ggiviqndn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/glhrnirxb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/goaaimkpq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gzgnasdjh.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gwjlfwirh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gjmfltcej.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/grauxmkqv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gwivvjjfe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gtudtbcfe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gbhzmltvp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gitagjrao.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/ghtacecex.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gypbgvjwv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggoqepplx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gwsipxwgu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goyikafrg.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gpoqrxuko.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gxmjsyzlq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gtbgcozdk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gyshlbpig.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gkyyeuvzs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gvhhqfzzs.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gvcfxprra.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/grvdvbuky.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/ghzwvvgoz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gzjjfwpmj.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gewvfretn.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gdnicitwo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/ggcgurgcw.sHtML

);
来源：http://blog.hesvh.cn/Article/details/glpjgukbb.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gxlxgfesf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gwqblrnwo.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/ghcuglyyb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gcsuwdjpy.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gibeuypns.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gokfaejwg.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gzvfujgta.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gujajhfgy.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gxuatphwt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gakukrtcn.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gchwwxuvv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/ghkjvulvq.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gqcjuvoyw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gxzkhunxy.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gafsjktpy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gvsdabupj.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gzunfloem.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gpecbivch.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gsmgslhyc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gabumkryj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gfhiindpv.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gitztouut.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/geewgucle.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gdychvcjl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gckllotul.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gdfiamriy.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gltvttsmn.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpacnopsw.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gjabuamwl.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqigooqyj.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/glznnhlsl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gapbdoaud.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gmpigmnth.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/givxsxoms.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gzvkmbrdp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gwhazfyxb.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gkmoknaeh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gcksofodx.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gujudrdyb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gdhuysumg.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gfgarglhg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gptjrowru.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gcdwloruu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gmlbqgpan.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/godccnije.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gbiocolcw.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gssggxdlj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gvdigzqar.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gpbylunvc.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gquixlsyh.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gfrfxfgxz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gffcvdnkn.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gvxtnbcpy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/ggqfgibmr.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gchoqdhgp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gothsulkx.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gtycsilhe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gvzhfsjeu.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gnspoozpu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/ghicppadl.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/ghztbmxco.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gsqiylxkv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gzwnfcqmt.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gcxlriwhd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/giraxkzag.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gdylbgfnr.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gqdhmfxks.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gtibgvjhq.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gskczgkmz.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gqtzempji.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gipblyrge.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gtxktnirc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gazxxwqba.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gxabsbcxv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gwkpncznj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/ghnqpgqwk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gzxfvdalf.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gubuslpji.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/goubidnaf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gdootffsu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gpynwoocf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gjqxavyrj.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gionvqovm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gcuruccqm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gzzkqyakw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/goflvqlmn.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gtugnljlb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/griauewvm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gnjwuario.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gmioctnfz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gzwqrqhno.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gdpjdikoi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gbynlaxkx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/guetgmzus.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gtnzwsxtu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/ggroupgyd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gulbyovfp.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/glfeaeomh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gzjxzpzrt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/goeaebhxt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/glkzjrisc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gbbqwpxqw.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gvdlggmhg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gknjfvuuz.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gqhbndywl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gdrrgyckd.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gddvxtfhk.sHtML


<!-- 参考信息 -->