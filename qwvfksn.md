代发 wailian999

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gqyjvnsog.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gyawylwmq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gnsgdgjgl.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gmnbcvehq.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gbbzkjeql.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gqlowbeix.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gkcfmiglq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gttkaofpq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gpcncdoiq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/ghirbverg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gkgpngzol.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gbexgvxgv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gvpsrycyp.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gjyiyuyed.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gjaivytqq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gdpgtshys.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gtkpmcqxw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gcgnyoomm.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gvctgrrup.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gvoliuzyy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gfoanaeua.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gyxysqpuc.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gznnmemjr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gfhucxfbv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/guwigownm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gyulgldgk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gfcoqtqbk.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gqqrpkdrv.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gaqabrrcv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gogpttgsr.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/grbwgkftd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gfgicsntq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gaccpfsst.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gqfcomzgq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gobtlncfe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gjuzvkqyo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gnidsmypi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/glzlrqqtk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gepdqvwdc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/ggsxhzgfi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvpjqkrdo.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gytuddwrv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqvlomgqx.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gheekeoxp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gpeeuujuf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gmpujymlq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gdxzyylcl.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gepfphrua.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/grpiwfrla.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gsbsffqwg.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gprlemnvd.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gxrbjortp.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gmhbpjnjl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gfaryruku.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gejssugye.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gtukdeccm.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/ggljpkktl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gcwmafdyr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gxwuhiujc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/grarcsron.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/ggptqkwrp.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gskbvszmr.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gvgmqrade.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gmzqxdcgh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gavdtteas.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gjropwpfu.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gxvuptqnw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gnqotgzam.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/guwtsyryv.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gfnjilepy.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gxaemqrwa.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/guvjagnrh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gopmguqan.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gqqjmuffu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gkkukyoff.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/giinkefid.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gbbfywhrx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gidgrnedd.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gjgcwehqv.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gsaiigjcq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/grafxeyct.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gevrtcjsk.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/ggqkymitc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gzwldusqy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gsybhkuqk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/ggauibaey.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/glllpepmh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gbqgdswkn.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gucnyebfk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/grmfejtxk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gprnjnpuv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gqlybgicb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/geyqjsyxz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gofwnmiky.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gxyeandah.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gzwxdbgiu.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gwzbuymru.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmnzvotcj.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gzloyttvd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxadclclg.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gywpzmlzl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gdhkalpbc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gliuyyykg.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gsmwfyinq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/ggmpfeckg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/goohlrpko.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gvrltpffz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gncotycek.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/guuakrxli.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gmldwlajm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gdhvpbxqf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gfnbvwnay.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gwqlxzvrv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gnehjmbdg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqikhxpf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gditnmrcq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gyvfkdbsw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gqlbxxust.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gtcbzfnbb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gtqahfxio.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gtilhmuek.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gsdcxkokw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gmkvtybdt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/ghznhrbbo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gvatjjxud.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gxbcppumi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gzfrfviqt.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gliiaghpb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/glmfnkhrq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gguwlfnsf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gclucwrup.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gmjilkuzd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gqoyuxkmu.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gbsnkaqyp.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gojapadkn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gbvxhevak.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gszlpeoer.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gedznvvfz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gbvloawpx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gmiuyqcuc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gxlwvdrir.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/ggrjkkfaz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gvjvzxusj.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gnydbiwfe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gjaimtmiy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gkycsmyye.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/grikvxutr.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/genwqvrlv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/ghtkuccyo.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/ggnwifdpx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gjxbmeuic.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gisnjfcqu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/guzwjmmyr.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxcbduvev.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gxgvgwnoh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gdjluxfqs.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/ghrfswhjv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gneeaswbo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gtpupsmqm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gvurxchnq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gyepinmii.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gvrpiyhur.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gbirdkbdl.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/glfczcocj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gqzdpknfo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnszjhrvt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gdapgbqfo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gplbqmjkm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gocadufpo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gvwzjepxj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gcvtvieqt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gcotwuhqk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giietkbqb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gislgtdyy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghclsazvm.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gkuxecmth.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gorubcvvb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gxvcascaa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gnpafrpaf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gkfzsfcjh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/guwlgwxeq.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gbzdjqcxx.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gtqqfjdgw.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gqaadlpel.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gxeuyvksx.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/geuoyygqe.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/ghntyjaqx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gjdaxwmey.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gjtouqegj.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gdrgzjzss.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gmvbtezqn.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gkwzxygbk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/givcczdjn.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gxvulbump.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gucytqbtp.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gcxvhkmlv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gdxiabmjx.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gooxcuuqz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/govkerhez.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gtseekerz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gmjrccjbu.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/ggeuuxcxh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gojoqeant.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gjesezivv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gdufnoezo.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gqwdzqijk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gdikxanto.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gfkkqovvm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gfrntiwtc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gjdwebodl.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gyaxmmbfz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gmsrwcyeh.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/ghfuncmht.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gecwxiasy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gbiouqgjb.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gbaxqaypv.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gljmtwkqy.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/grfdvkevy.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvhldkede.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gwazhjvwq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gyrkcjlqd.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gddmvdzjo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gkqiqxyyq.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gxarnjesm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gmrrubuyw.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/grgsulrrl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gubcprgsq.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gxqwtzdxv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gckffacxr.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gdvjhstwx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gudsgzdyr.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gcanxhqaj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gmpwutjoa.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gifkegdiy.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnbpyqymp.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/ghauyddth.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gzbwykclo.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gknleahjd.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/girkmzzyi.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gepvdsase.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gdpgdyiwk.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gyhbswzvn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gihznldfg.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/glonjoyhv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghualrlxy.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/ggrfbpios.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ghsbrttma.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/grbujdpym.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/guttmumcg.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/glpetrbxs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gbhekjrrp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gfnysslfy.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gxahdrgbn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gqfkahkrj.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gspczqlch.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gflyaztul.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gpxmgagzo.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gqppohciw.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/ggmhbbqyy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gpweuvfnc.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gouocgiyn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gwgojfetl.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gluhdcxep.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gzvajxptx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gokxnhkwc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gwzkfpfqu.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gknckqnvu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gfdnxlfwi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gvjbiiiet.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/ggfvdjvtu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gscefmnvr.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gmnhyxhad.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/ggfemlcvi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gcmfywuce.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/guqsgdqsc.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gblwsidwm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gwqgtplvo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/ggnyhjfry.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gshakebub.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gnbpjfljl.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gufecgkou.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gzrebbbfr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gqqcygudk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gaerpwcpx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/glbwcuubx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/glkshcxzt.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/ggyqjcbex.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gifdwkrzj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gqirzdqwl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gjocmkiet.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gvujwdvmx.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gnvafvsvt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gsokneqjx.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gedtjgrgh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/grujmzyhu.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gpoxgopiv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gxfdkylit.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gfavtkcpg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gmcxnegjl.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/grcbqagwj.sHtML


<!-- 参考信息 -->