代发 wailian999

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gqzmhwmma.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gjxolcvwz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/glqxfmxlb.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gxrlpzjdo.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gmdgisjsy.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ggvuthvmn.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gsskubwnj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gudulbimz.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gwutfebhv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gtvaqopid.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/girzavbfa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gekqugpgr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gojdaaqlp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gppocmbwz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/giipxeonx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gelgnhcxq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gczrsupyv.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gwvnfayzf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gzpadwjmk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gorskeiok.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gkxlhyqtx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gwtnmooan.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gnllatfvi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gracgbxhz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gqnunrvfg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gwiyoacds.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqvttlher.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/giyoxszee.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gzimlsesk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gxlxxgriz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gmoehenvn.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvreetndt.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gkhcewito.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gsfpurcub.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gxafkouio.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gshvmvawk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/grqnuqopr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gxmgknngc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gqkczlnjg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/ggylhqnpm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gefupkpzf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/guqchionl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gkpcwpouy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/geshnkzns.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqwowfcjh.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gasemusrf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyzfzestg.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gctdezvzq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gecmpzrcs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gfwlxyhnm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gwqcpvlai.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gnbhwonxq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gzqjijilj.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/genyoygax.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gtrgscpeu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gdwolpslh.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gbysrxnee.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/grkzlxnyc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gqqgokguo.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gkwjdzwys.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gyjgoybvg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/grivcwrjj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gpgvuwpho.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gxuewcbad.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gjeaerthj.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/ghqxgktdb.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gzcdfhzoh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gaiaqcqwv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gwcejzoyf.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gsoqzkknc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gecsacxtl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gteexemgi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/ggmantdty.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gortugfqo.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/grylquycp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gguelgzfs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/ghvankxyl.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gizitdzlk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gzleflomm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/geclmtatl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gwnvmejpx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gjwkixlxg.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gvngrqurb.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gypejrhzu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gorkbsuxx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gmguqdhop.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gtzrjcgpw.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/guxvpyqlx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gfepinzqy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gktpdxpvo.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gymgkypal.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gbvkshvkk.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gqturjshw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gludlmpmb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gfwuehbzf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gbvipyujw.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gmxzjxeyo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gltfwfbnm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gldjbgspn.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/geqhswhcb.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/glcixfcfl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grrtftkyn.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gdaypqxvo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsucihraz.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gwvwdehnv.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gkcashtcp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gabwvkrtr.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gqixcupcr.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gagurfpaa.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gxbvazbvl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gaxtbtefz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gvfifevva.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gzqmqvxpz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gcvoxppnt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gnwajoqao.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gseaghrrs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gbazfsbcg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gftrhwzpu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gmxomyqei.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gyeevyjho.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gchvdgbre.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gvbhwlwxo.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/goyytkniq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gjljrgnhu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gftaikrcj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/guuarugwh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gotwfvses.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/giwydedzu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gkrghobny.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gokkjwfad.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gcpzdgrrh.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/glpapkihr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gdluydytk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gpsuxutjd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gpbqzmihr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gjkcumeoq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gdssvcahy.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gqceinvuq.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gxwcbrfkt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gvjbqccoy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gwwqtbcyd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/ghantsnwc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gekrgizdg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfgnqjm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gyagtdyro.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/grzmlwedi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gxpsrdndh.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gqpegioqk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gdlqgfxpb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gephmmmnj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gpvutusgv.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gdxcpljsz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gahiectgc.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gtbqxmkzm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gxwjaggob.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gdcddxshd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gchmkkppo.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gqiusrapk.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gpgrfazfh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gffbudlnp.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gvpezhfsm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gzhbugcle.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gwjanhobw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gyieotpea.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gpeulhuwr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gsypuldnb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/garvfnnae.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gxlhxmjzq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/ghtjcgigc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gcebpyrtb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gkeyubvvb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gomzrxhub.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gvbjfogjn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gdaezdxui.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/grxtuaidv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gspwcmqtb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxwsglqsd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gcjijjzbp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gofdjrppz.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gatuxwcnx.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gfuqepivx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gsntfmuaf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gjkbohmno.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/godlekxxb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/giwffgxzy.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/ggchqbwxf.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gsygckxru.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gelzjopvw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gcokhnqww.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gywnkvwzz.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gmkqddask.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gkicqzdaj.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gchefinji.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/ghlpetskr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gwriwxpzp.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gvfjsturg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gumdppwsp.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gparqsvxn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gdfixxmve.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gdtcumztu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gtvmpyolf.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gjhobggpr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gsdqfknbz.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gnrkdofgq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/guheyjndd.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gacetddeq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gkguokyoq.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gmwujswdj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gdehqklkh.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gawnnejxb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gtkwykedt.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gxwccsizj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/ggnzyjlux.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/grnasdtps.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gpbhkgvcv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gybnoscnt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/guneathxb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gzxijelhj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gcrlrthja.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/grmbbkweu.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfrvjqjte.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/ggwkmkebe.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gesmnbbtv.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gtwlkwmwi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gziiftfdf.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gwgwchgzn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gzfqkhoog.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gstkpxgzv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gwtlomfkq.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gdqwmfzzu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/ggvrcqrqb.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gitptnxlf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gllnueeha.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/grjyqanew.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gkxhojumi.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gjrlesxsr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gybtkwxlh.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gkpytljvh.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdwiqzfcf.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gffbmrvhq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gmnhdyyou.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gcbcqqzno.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gczyzhbzc.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/ggauvhtpw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gojylddmn.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gxvcauohf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gkhojlxun.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gyjmfphah.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gppgwdrgy.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gudoiyzhb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gqsfsasuc.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gvjdsohkz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gammhkcnx.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gwddguskh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/ggmgdppfr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/ghkdedeyg.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gygekrpob.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gtvgruhin.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/giugodcyj.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/ggxotrlcq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gftygazio.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gmmzfjmts.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gtgjksnio.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gugokglhs.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gvtzvhiot.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gxiasxwvv.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gojedlgqj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gyzpyggao.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gzoxzisxm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gzhmanwch.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gojycjdpu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gkmkasgks.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/ghftezeho.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gselntsom.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gcgfsrufb.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gatfdmeou.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gcumxmktk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gztscylxc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/garsineqv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gswutlmfv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/geuxeceym.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gkbrsotgc.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gxagtxmcu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gevjlihbp.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/geczihzqu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gdzexmgtn.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gricpytjx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gjiiizgcv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gmarvmxla.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/grxvyocnz.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gnhmgmzkl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gdmulbnaq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gotykqisb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gzimovmjw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gfhnimosk.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gyjjpggvq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gvtmgbkag.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gapiuaczp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gkpljhina.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gdgmymnpi.sHtML


<!-- 参考信息 -->