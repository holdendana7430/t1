代发 wailian999

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3obuxoupm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tdxfiyus.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wcwrwypl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3shjppehu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bhyzjmdr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3llwfwjxz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ogynfihc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nluylwgo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3syprwzuz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nazntmmk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ptlainxb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cdgbywdv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wwwnoawx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3tnikokjj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jgcferth.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3elbhdati.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3suuavuyw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dppfaccz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qhvnzcfo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3pmtfqtpn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3tqhrvvyz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dmfsflgw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nmsrmfik.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3jiyaxvaa.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hggusmvj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hwhfrgdz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3linlzukb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rknzyhnm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lrjmgqfa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3yuujqqmi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wgnciwgz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fbnlduff.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nbrepplh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ynoojwzb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mpiqiszg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vkmnfnwi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3akvlrflw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3urmslruw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3syxeemva.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fvetypad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqoxkwjx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ugyjvpzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwnwqmha.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ovsyxlbp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fbvratts.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xhximtry.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lwqcwbvq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tdhpcjgs.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gzdmvegd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mozjobrr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3pbngsqlx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ybjqcdlf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zgkisled.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ibjggpoe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ubtigeeg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dgtibuuo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uvcubvdb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rggbjara.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kktctoue.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ckekppwn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3csnsgylb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3bhtlyudw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3wdbyzjzr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nwiridvs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vbimykhc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3npztijfg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3idffkvxt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ocbaztor.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wnviwdam.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bprqlgah.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xnrnqbdp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rkhwasyz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wgwossij.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmwsxkkm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwwgvwus.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3cabjaqhn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3zdppalht.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3omvkbckt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3emfrddhr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3xukdxvfo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3oelmheda.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3naxetegl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kauhmbxq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nkhrnwha.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3cxpagyvd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zovuwerr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xwcjfjen.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3zohedfqk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3cgdfberg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3tbynggwi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jmrhljaa.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ihwvyljb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jvrefdcj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ztdtlxii.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3behcbzgb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mcfzctgc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3athpzxsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idfdhwgn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ogogljkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xerfhgtq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xddncxhm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wkdgdiwc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3whwvlchl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rqlcscxx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hgvtnmst.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zcuiptbs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3etpepjie.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kufoemwt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3yspjdpuy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ipvkpzrf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ocxjzczb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qysxevou.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3qmyazptw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3pqtjqpar.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hazcyijk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3gbrpovbu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3btugrtej.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cgfiamip.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3yhdxbnev.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3cqykhzzx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3svjrzdsm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yxxoqclm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3invjmjuh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3nlqiiqha.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3slwvtrca.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gagemlqw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qbhyntlf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3wqybpypg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3vvvngkgt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3skuxivmm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wadguvga.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3scxwlltr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3iiungnnn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3njkgcykh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3lzldyhtt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qsnxjbba.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hwvbjnyq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3bayaenpk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ibzpqger.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3dtrmqdoi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qdktntfj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3pmtlxhfd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3awfamyss.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3vegbkpox.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3szcfcisg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3hkwglbfe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nymzqhdx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mwhwoasa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gdpafldw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3brdjhawm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dmuynegr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3bivtpufx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3flkoeobu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkyjsbrx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3elcbkmvr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3naxpzqgx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wmyjdxga.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3harexiis.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mozyktdt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3mnlwvuhu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ulhyfwqo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3exrdlqpi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dcutfhtd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3wcakzdlo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ruxwqqoc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wkqermvg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3xavtpwix.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ayanpwcj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dprsvmzz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3lqhrgabh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3uveytfoq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3kcueodwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hokarjbs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3aauslrir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opscygve.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zvilrlrt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3xguglnut.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nuncwtun.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xyoxdrfj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3stchdhnm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3uijgjfnb.html

);
来源：http://www.52xcode.cn/Article/details/gt3qolmwkbp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vtbwfjww.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3zftkorqa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gsdvmwmw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lvgoitmp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3vdtxbxba.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gmwxepjb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ubtdbngr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3crarinfq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3sttpeorb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bvjyryqa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cvczeisr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3emhimegf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lvqijpvi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3blxfmvjz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3dwwrgdpd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3eerneosc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3llegoocp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3xgjvvopl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3frwoccmn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ohagcptc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yhmbkdah.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qhlbncon.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jwbwmncc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3gulnsqxo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mlxgzlvt.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wurokppu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3tmbjcddt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3jrilfclp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xuasxfbw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3izpjjjqm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3bgxtjhpb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3utfwpfon.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zjzxcstv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3fpqxgsjn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jzuqtybn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jrhgclvz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dbllqubn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cxazctkc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ayzeapij.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3cbehybxc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3wupafmuh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3arifxkjt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xdynzhgv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3qpfquhva.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3rulqoysc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3oarvdaov.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kykxriyd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qprwcuvp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3uublslci.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ikaaevxe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3chxhmpfj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xpdioffo.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3japkxbmr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3chjamqdw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3tabgkapp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vartfgze.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pabmroar.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3bxqjpvcc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gvdtudyz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zqbxbeuw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hzhiokcq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3expnqdnx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xheikvlx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ftsyfbfn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uwajorpv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3trzabuca.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ynsxwygs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pkzsokiq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xsncnqhe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3dopkmegr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3gkgakcla.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ujvdxjau.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3tpniopnv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3iipqrqpt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3pmhofyzo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ebtdmlfg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3zxtcjwle.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ckeqgvnf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3cyvcrfre.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cnflsrdg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zvjaivbk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fodixhwk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3awrepfvt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3tqepyhzd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3gdmqowyl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3owcdpqqx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3walexioi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hztwfumi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3prhiwgoi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3njbukola.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3fydiwcoh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xsewhjzg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3tnwfehkj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bpvmpqkx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3boacyxam.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lpkvxpio.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fknleqgv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xyvnpuqq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3yxlbkdma.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3oqvakmos.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3xfmjecqp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3szeftdbr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3frxsmdrw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ozsmxwsj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3paxncehf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3iarynuga.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ftpfpwel.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3nxhuewcd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3rpqcvtts.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3huspplva.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dqoclexz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zbnysnee.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gkgroiof.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3vepfhfzj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3efokpuwz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3zelsjmse.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iayiilfp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3hhostckj.html


<!-- 参考信息 -->