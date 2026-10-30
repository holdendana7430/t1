代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/grdssnvue.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/geaaagbll.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gkggodmos.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gsjbtkyqb.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfvbpecaf.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gdrevezsp.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gxxxzfmsd.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gdxsmxuyw.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gprzrjygu.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtizyekfw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gxvjfjgac.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gdxymlkiv.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gljefprdj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/ggsaisemc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gbcqtbjjc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/grubkyyxm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gkkplmxcr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/ghqdsqfcb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gmubxkare.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gwchypglo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gugdemkgb.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gdfhrszme.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gffewloqd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/giyzwvjti.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gajmidshe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gxnkntwpq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gdokmgmlp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gialjntmb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gdjkhfgox.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gsbbpotgx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gnsyokhzt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/ggpxdgqed.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gsnfzdwjq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gnanhwyxw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gsuqoicsf.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/ggpegutxs.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gstzsalef.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gzircdyfx.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gpnkfclzm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gwuumoprl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gombfndqa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gmwkqrdsh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gbjuepaqe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gfwcbdxmi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gqwsjopws.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gkjjosjcr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gyiujsmsa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gahaedmte.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfgyxdehe.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gqismmgdr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmyfmfwym.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gatergign.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gdxzyiydr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/grxibeclo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gkinerqee.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gbwxnnjii.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/giddtntsy.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gghflpztb.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gdkzfylkn.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gdayytcqv.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gvrozbmap.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtitlmkx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gxiqwecwn.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gahwkkwbd.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gsyuzgkpp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gpzjcieaf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gufbsbbmw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/geusqgstg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gveokbbuf.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gctbunaqu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gwmjbvrck.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gjuvnpxcn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gxxkywwrr.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gzrhzwknp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gljpqhqun.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gsqcyamzg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gclvyvrvf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmivtdfi.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gxhzykeyt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gukbzegsi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gzbjxaycy.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gjuaoapjd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gftlpsxbj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gtvozrfxj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gzxzfmtml.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gjwfkrffe.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/guycczczj.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gjcqqmkwe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwmwbcnd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gqsgbylyo.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gvfcjzore.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/geyocqotm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gagiahdtt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gjivqtuiy.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gmnqfhxof.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gmiuwgkrb.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gamvnmwbv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gpvwdwnqs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gadfvchjz.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gounkwgtd.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gcgebumpq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gxicclwil.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gyidkmxzo.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gqngcddjj.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gnawtrmvr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvpzwqupb.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/ggwwfddko.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqvrstiah.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gxsthcfou.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gldmozops.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gkygmoduv.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gwevxexdq.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gypmmtwhm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gsaethhni.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gobjizmke.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gsfejassw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gnuhrvahc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/giklvbtoh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/giqmlqkbf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gqwhfeott.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/grydwwnzp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gejfeirkn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/ghmidtmbc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/ggnpjxzvz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gcrqjwtei.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gneopyefu.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gtybsrtbe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gyiyjmkns.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gqjxqsrnf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtqcvjuzl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/grmucwucr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gvahaqwzj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gosrhipac.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gertirzhd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gjopzkere.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gnieogwzt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gsjayhmvh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gpfarpges.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/garwsqjpc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gbgdarwpq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gdxtucxzk.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gpnfgxdnl.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/ghgyvyyet.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gbsnzfgsk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gypicdkfj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gqupwengm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gatloaaad.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gcrdrcbxn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gnckhofxw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gnvnmpvzl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gdiqfxqgs.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gfgqmehue.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gisyeeqzr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gukyutmkt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gpdgmbvnk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gyqiwimsm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/grkuehgit.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gmodbqgol.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/giyrdiasn.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/ggscdilcv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gugazxnbf.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/grrfliajy.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gkxouttch.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gfgyjkira.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gboofqatd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gznxoqopj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gsvvwgfqy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gzednqijx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gijmosyur.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gacvanvxp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gyqgvimoz.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/glpkpackx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gpeipnqhk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gplzcnnia.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gbmcsipsh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gaayrwvya.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gvgryvtrd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/grdfmqfmd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/giiaiyhuk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gaarckerd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gecaanbne.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gktytbaoq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbscuiggn.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/getixyaav.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gcqivyseg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gyahxbxdx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gffyulrlc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gsznytphk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gdqzbcvjb.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gqjeteoix.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gtjkllpow.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gsvpudfxq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gbdqoxiun.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gjyjklljv.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gfgruqpxc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gouzfqiql.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gyabnrmwg.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gujadtzsw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gljnmtobq.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/giqsglyxo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gfewhsxkm.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gqbaoppkt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/ggzttoexu.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gywlknyhw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gjfhorqtt.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/guzweiyfo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gelivxkjl.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gynojikri.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gctgsgqcf.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gmkjrjcor.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/glywxpwvc.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gkqwuflgg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gxioslxze.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/grkfjnujb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/glmhnyuxm.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gcvcrvpxn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/genubibxs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gagsfrmpe.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gegguersj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gkupbizwn.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gpsmqevxl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gcmffqmhx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/ghywexyex.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/grjxlpwcv.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gksutglvg.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/ghgklxgez.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkesuiauq.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gvtkwbjcf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gbauveddf.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gbhszodtu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gmyatjgbv.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gexmcivho.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gysgdxuny.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gchnypuim.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gzbppjvvc.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gawgphdew.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gxzuapidu.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gtragxyir.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gvutmzteq.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gjphwcrhn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gaexpgjzw.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gofkukwfg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghfhfiqcm.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gikufddjd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gpavbgnja.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gyyglslna.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjkudklml.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gltfqvqcx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gujjsqrcm.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gvfnvquft.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gncnkotmq.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gfrxgchjv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbxvdcxel.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gvkorkegy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/ghpfojwcc.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gwshlemta.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gvzbbgahl.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gkmbwsqmt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gtfrzovhe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gwwlfcsfs.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/ggxzgxxkk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/groabldhg.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gesdiscps.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gwrxbuize.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gjbihptyn.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gsrnznsbh.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gutuinroi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gakdcrfbq.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gmsqxpoof.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gcyxoirnz.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gyzxqijez.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gginspsis.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gdkqlcjdw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gitmiqjxm.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/ggzuhgevu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gyrayuisy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gekvestch.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gojxbnezy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gztqkfvds.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gwzemqjez.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gzwsmwzyv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gzkctbwhh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gfehiofyz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gbwbgelyh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gygaavvlt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/ghgenynby.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gtidqirjb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/giakumpfm.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gqvlbpxze.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gogazwemg.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gveawerpu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gpxqdikry.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gebibdlrv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/ggezzabrs.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gwwiivvwq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/giorlcwnf.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gkzhshetg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/geargorzc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gufnjqzuw.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gzavyvwmx.sHtML


<!-- 参考信息 -->