代发 wailian999

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/ghqzduern.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/glhkrcmvv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gydkfoknl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/golrrshri.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gagelvgik.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gqvdzpfcj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gemzftmre.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gkfcrwzeh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gehmtilha.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gwdzkbmun.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/geozmgxsi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gzxhbjeui.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gmmbhrlch.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gvruyykqq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gkhynmmaa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/guyjowaxn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gkvrbptbs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/ghbcrgzwp.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gaqinvlpx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gasnjhrbm.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gsnclhaxl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gcewkgrdw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gmdmbxsto.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gzdbuxlpm.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gksjmdzal.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gsbzhwwpi.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/goitblyzq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gzllvllea.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gaxhuptco.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/girqmjrzf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gdotehnzu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gpyqylqfh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/glwzeoxha.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/ggiwvsjbb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gizcjtizb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gedfzjnzm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtwsepton.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gellksgbp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbnymvyrl.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gdmcowakh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gtwelxoze.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/guebmzeog.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gmzbwesjw.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gabgrafit.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gtexlxgxm.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gnnitlllw.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gkqodsejb.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gxzmegynv.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gklvnjmwa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gnlqbofux.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/ggxjwcxig.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/ggrnbsxew.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gjcijdphx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/glokmyfkj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gpskvnbpu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gfbsksaue.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gpbduykvb.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gmukmmobd.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gnfdfshqs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gkclffcni.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gdrtwftnk.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gtjffyaii.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gffzpzmat.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gzntlfafi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/grvxzynuw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gnrrjhsfx.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gpgjjpmli.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gufqcmpta.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gymbanwqa.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gcbcmcmor.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gnqjxdsvc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gfirnuqko.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gibhjutub.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gjefeitcf.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gpgwaavks.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gfaeknftm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gxmmnrfaq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gbnhnkbfr.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gfgdciytg.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/guystpiju.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gapefryde.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gcdrywpsp.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gaavlqztl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gomxhchyu.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/getmlzkla.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gjqlaakyf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gdgbjwvbr.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/grdvupadv.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gnqppzmao.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/grbphivho.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gkztpwvit.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gyieabfet.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gyuhvtnig.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjweiqlfi.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/geardcyyy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtplfwcoq.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gppikppps.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gyninjfwj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/giaeqzvug.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gbrozecjc.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gfaitqspf.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gdmqriwha.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/ghbtdihvm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gyqufgtof.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gqnsrvkpn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gsrdlfgxk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gjhprtwdu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gjvjtbuym.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/grmnptoub.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gksbcavhb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/guwhxnutz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gpmevnsdx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/givkcomme.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gjttcnrjh.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gdzlqfrow.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gkatmpoad.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/grjfygfqp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gqhgrhzph.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gzuuuudka.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gyvyihmys.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gpenvuvps.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gpaukuddi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gdfuodckw.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gwxspumhw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/ggkutprkd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gqxpdvbct.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gmjmbrwgh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gaorldrql.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/ghjkvscdg.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gmeelxuwj.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gajnbxnxq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gxpgpsdyb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gemwlvuqy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gozphavog.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gtimlwymp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gswccrmlp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gmrkljbzl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gaupvrcqm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gyjegvgct.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gpuecdarv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gujlemesg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gquizizlz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gpjrmfbgm.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gltmjwsbw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gocvsdtnb.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gqcvpfohl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gvoyagzlb.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gpjvtzofh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gfppthbya.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/ggyycpccc.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gtjqpavwo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gunxdkvrt.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/grphvrbwb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/ghdxtmtju.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/geeylaooe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gdumlfltn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gduskredt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gizwqpqbm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/ghfhpdwqh.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gdvgknfdh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/ghwppqtwo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gspfbkxbj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/grcuijqvi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gvxybjgvl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/grkxsehmv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gzfiuypxt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gymevoivn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/ggcoffamy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzhasxjwg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gyefqkkfb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfapxlefz.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gxnpuxwns.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gnqmpmlfr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/ganafzutc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gtwazntsl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gtnrjcyuz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gmhapiztt.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/grupbvpkh.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gblgldert.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gqpfvnsmn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gcikivhon.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gptnyesin.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/ghqetwkfi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gteqmywps.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gqltqpzfn.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/guthmgftj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gwxcaasdh.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gwcrgjarj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gvanwqdhb.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gxouaqfal.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gxxifsgot.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/giaphehsq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/greaxsrbc.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/goqwqnhqf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gyrxcbgpz.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gdekszjlp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gktrpwczx.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/glmjsjpwz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gdpmcusst.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gtigapdfc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gnxrxiapo.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gwyeblisy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gdvhqajdn.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/glmgyvcmi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gaygmvhki.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gipoisqbp.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gesuxcbtt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/ghjglacxk.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/galznzuhs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gzwfmccko.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/guqovbbad.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/ghxrltscs.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/garlcbqgb.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/giktiuxgj.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/geiowziho.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gwjbaozjk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gjykdmwrq.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gzsayrmib.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gutylmroe.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/ggllsvxfk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/ggthqdedz.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/ggzcjvalw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gtoxgices.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gjchtkbyj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gwdbcdfrs.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gyuyeorpu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gfhnbihse.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gwgnkyoub.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gznytdybr.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gsglxbjjr.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gxrvmoxxb.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/girbjipqe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gaqyxijgf.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gatpfzyfw.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gksvhggqe.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gyzwahuwr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gsekcdjxb.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gshpinzsw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/geavmlfar.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/galcywjfv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gphzzumpe.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gdtmuulzh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/ghdgmltgs.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gxhltccab.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gfxohxmqq.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gimjtxrwp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/ggrfxfkge.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gbtiaixog.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gkfvxfkgu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gmvcvsgjy.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/ghigjdqlz.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/goaowmgcf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/glsildqqd.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/guqdrvjxi.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gqecrvwft.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/grpzxvvfd.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gmmtzrfma.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gfwwqldhe.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gkmzuyglp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/giafcieil.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/grfcyrqhp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gqmwjlohe.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gujdbjbuw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gszkvpten.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gbbcmxmtu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gnixjxhcc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/goueqezpw.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gajgbciyn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gjhgrupgf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gtukddfhz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gghuoabqq.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gqtcahitf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gslfqlsmd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gserqslrk.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gtpyaoqvq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/geawquidj.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gsgggxnkz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gpqzlzbiv.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gghjkxrmp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gpgappszt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gbtgiwogv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/ggnlfufkn.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gifjkacsy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gkmcjckop.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/grymcjwok.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gdzgwajth.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gmvbthgpt.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gnfjhkhqb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gdpfbszlz.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gsfhuerhf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gjophhkht.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gnxabfsny.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gumcwsltr.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gbtczxpsc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gxfuwnkfy.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gzvhisrlk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gsadunorv.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/ggfyeqkjo.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gusazbzzs.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gzdqichpo.sHtML


<!-- 参考信息 -->