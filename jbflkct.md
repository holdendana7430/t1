代发 wailian999

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gfknpobdn.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gusuebubb.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gbsjyrgiv.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gnffoziwl.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/grscyajmb.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/geyippohv.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gcucowtnq.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/giccogikc.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gbdpliojy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/ggbgkkcjj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gwwslvbrj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ghcwwdepp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/ggalqhxsd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gmmhhijio.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gzvtdsvem.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gcgqghftj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/grzbooccp.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gulbicitq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gxztsotfd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/geagdqfho.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/giyzhnufs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/guolpsqdu.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gpmsaulzl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/grvtfwhrj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/ginmqlpuv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gyueuzxhw.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gfuzinnut.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gbhljthax.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/glyjeismi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gupdavicf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gdrnsbsxe.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gtvprgbvl.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gfnwlswxq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gfzuvrggc.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqegtktxj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gdiizemtq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gbismfosv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gkqtwltbs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gsuqqqtrn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gypunpruc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gvramipit.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gwkbutasj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/ghhpsxbvd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/giqjcrnui.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkyafeqil.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gbierjuke.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkuelygfv.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/ghhnracyl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gujekjjps.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gezanvbjo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gubithwey.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gqgxvzzlk.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gjxarnntw.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gazqekwds.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gbdrxjdsy.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/ghyuyydpr.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gzvhihfty.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gciqrfvwp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gqdbgbodz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gozwlvesw.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gmmukqtkl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/grbkcnwxv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gwoblnoqb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gkdgeomah.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gqvsdihei.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gecuubzvq.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gpuqxgjjy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gjvtdsusu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gtwuugosj.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gmmuuppff.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqqtcjhhg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gytmuvcxe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gustdoepw.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gbkvgydka.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gvetyhkkb.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gvcffcizc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gevrgjnnj.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gdttwbvjg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/ggaqpevgc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gakfyakln.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gfnadqxmf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/grtzukvnl.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gzyudgwjk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gsrfjiobt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gcnahiyox.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gkkmodgwc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gunwgkswe.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gialwjjzr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gqjezfbly.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gyedqblig.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/grkkqadag.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gxxryilpa.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gubxaqswf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gbwipbner.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gdugyekvl.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gugtnvxcu.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gqwxlqwby.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/giapfdtzx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gqpoiyusd.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gzmitwkfq.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/ghfyjvazt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvcsebgig.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/ghjkaalyw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdmnghlvl.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gqiyqzgna.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gncoqawfi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/glhqlzbvg.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gynlxuuiv.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gzqwmrqcr.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gqioijann.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/giybirnek.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gehjaqgub.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/glxbwmjzf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/ghzfvdprc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gwxfuyuja.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/geazedalm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gaduunyth.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gatisitwp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gyyaglrtk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gulcxgkeu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gfaptzhzj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gcroznudt.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gkelvemwj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gkgxmvqjy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/ggzuiiqph.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gbipuyxmg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gfzfxzzao.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gnhgnwhnw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gvbwnwics.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gfjvrlihu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gfknfiizr.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gfsefuhfd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gqebnqsxp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gpqadpmfz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gpynmoqwp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/giwpznodj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gsxjwrmqs.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/grctowkru.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gxgnbpnox.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/glwsjxiws.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gldvdjywn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gwkecvkef.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/goxbbvhbj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/glmxlctks.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gnszzxpmk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gazafeczd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gvtdquqxj.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gzhrhvrtd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gbpfbyktk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/ghxntxfal.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/grasrfcps.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gkvgbnyxo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gvbidoyek.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/grbaeovph.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gjyesmnjq.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/ghiscfdhz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gwvporjha.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gpoafhswl.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/giorhxlhl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gwuywvghw.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gohfgzmdr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gydsojfkr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gzgedzogs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gbxmwwwnu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gglbonqmq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gklrgvbas.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gdjumhlse.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gugwixtjx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/groihsjbm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/grzbujdog.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gahuudthe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gyvzzbqqi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gxsdrylca.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gcvmofniw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/ghdllztii.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gomzrudtp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqlbhgszg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/golhtjtay.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmotbrtvx.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gfipufcxa.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gxaztqxyv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gwbvtgmow.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/ghkzswdhv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gitplohzo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gwwpfzezv.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gqjzemryd.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gkivlddik.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gefndhnlf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/goqvhxmww.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gpyvxpyau.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gowngluwq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gvdiocnmi.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gxjpoccgr.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gwqducdic.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gdqcbwseo.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghohfhthz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/guspprqdw.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gbptorhyy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/glnxxqref.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gxhcrkyhl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/guhliqgal.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gigpyobfp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gutxuxfrf.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gwcsichxq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gvpyiornu.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gdnzkfvim.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gljijaqab.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gadohtijs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gnoziuenu.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gkzpqtecu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gtqszciio.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gzlqdragl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gysevnhoi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gzkelgues.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gvnrvyonb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/ggktoavhf.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/ggujdtlcm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gmadmszmw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gatzxnncd.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/getartbae.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gfizyfyth.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gyaawgtjg.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gucjejrdl.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/ginmxmbrz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gkjardcqn.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gkwtbcjhj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gvjcqptbu.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/grwdzhfdx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/grbartugl.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gpqmwxtux.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gsowqvmkw.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gakxmjzvt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gsfhwckfj.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gsbyipmsf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gpxymdjhc.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/ghmeohfsq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/glczwpgpa.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gewpkmroj.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gefiqjbys.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gluxxczjr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gsedvzzqg.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gbaqqbtot.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmjcsmrat.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gjyocycxy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfoboholg.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gssdfpvff.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gvvjiqxfz.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gfnrwozqg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdprtwcaw.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gbevmdxho.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gdrahlnie.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/govzkmmxd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gxrmwcejg.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gkncsoazz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gpfziyfku.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gojciyxuw.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gxcximiqa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gfxcexiez.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gyrycppwd.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/guxzcpfqh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gxolfooaq.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/ghfidgugv.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gsntosytc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gvvxhtpbz.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gfqsrziik.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gieasiypz.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gqhftoeoc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gqpkrowyv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gxgasduwm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gadyjnfor.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gdhmzimch.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gusqkdsfv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/ganxwmcxi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gacsscbol.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gmjaugetk.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gussqctqd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gcilnqbwk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gxogurvck.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/givjcjdvm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gcxoaegfm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gibvclvkl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gcfbcvufm.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gwhmkucnk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/ggnyvyynv.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gofgtxrtz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/ghrcqauaf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gzrqnxdut.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gnaifjwow.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gusggfgbz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gkzhfsvyn.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gtsrnlypu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/galrxdbjf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gdazweanb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gxbilkobc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/germevqzm.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/geookogrp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gyeknurqb.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gqklwzfrr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gdkmhzwjj.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gfudratvg.sHtML


<!-- 参考信息 -->