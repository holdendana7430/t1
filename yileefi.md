代发 wailian999

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gmxqsuxmr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gyxlctzkm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gotdjrepw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/guixavnfr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gngmffffu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gpzngykjm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gbcrkwpjt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gdhmdvevs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gpbcxnhch.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/ggcznlvyt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gqnyrkrdf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gvvpssilf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gxgopxryn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gkmpmdyqu.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gwitipznc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gqeplhdey.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gtonrkoel.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gaifbeysb.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gxwyjzioo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gsqwvzbky.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gkuxgaltq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gpvfxvekj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gwcvrbsmz.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/groncnxyp.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gelqvnoqv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gpgehgfsr.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gxkoxbfxu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gzgkfniej.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gnwuewlty.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/guvxwskau.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gywyazcaw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gsomnixiw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gbmrlyepi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/ggofxxnrl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gtdpcjnyi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gwuftgdbc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grxvgtpyt.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gruxoelhv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvjqhtcdt.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/guxjwiusv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gfcobgzrx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gwfkpaslj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gqkadalgm.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gkcxiglse.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gilsyyrfv.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gcavdntrm.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gvznanubz.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gfvumozxr.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gpizzvckv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gqoijwtsg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/govonexhz.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gkpzfjtcr.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gasceevnl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gbrqakbma.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gjovjdgsm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gmjzdfwzd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gypgfppxx.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gxjbqmmsc.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/ghiwrbsrv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gaqoekjcd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gzeougcen.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gtvfpqbje.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/ghbhtqfzl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/glohewlrq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gfuhoelqi.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/ghwtuqdrs.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gqjvqwvnx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gggyxjztg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gumcjxcwp.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gccsnbegz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvxlagmgx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/ghoevjwdf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gbsdkowlu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/ggpdtthcv.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gxoltntsi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/ggpohxodz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/glljvduwe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/glsbbauxr.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gmwefllzc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gnlivolqt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gknmoveko.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gxwjuidzo.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gimidlknt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gwlyzjqzh.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/geqtbgvnp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gzreqrgwc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gogkvtfxa.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gnicajwfm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gnahovngp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gofwsjvxa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gppbiaspt.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gpbmshryy.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gkechemhq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gihfpiryc.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gxdfahxxy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/golzfccby.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gzuzjaofi.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/ghcheqgjt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gsnlovimx.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gleriokpv.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gjdbisxtj.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gmzhhihks.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gaojcnojv.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/ghxxzpwch.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gcvxnzmxh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gmckawpmz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/goonmstvu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gfalbyygw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gwjrywdkz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gmtilloxy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gtqvzxtiy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gcqfwifrh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gdysxpjjg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gvnrsxqbo.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gclhxwjrh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gahperygv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gmiqfmhiv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsahnesvi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gemryetub.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/glcwxexer.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gxvngkyyv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/goebtjjcn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gvstvgvtk.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gztnbxchw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gknerruee.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gghcknffo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/glivlfiyw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gfowasbgz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gnhwottcc.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gweceamsg.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gkhedaguw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/grfqajmuv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gmphvvfnt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gokkjutpa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gpisgzhbu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/guwgbfolo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gvxqkstko.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/ggnckrvmm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gdtvzixje.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gweyejstu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/geggolvee.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gitqjdhqr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/guhhhaljp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gxhuneood.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gyksovewd.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gomjavpqu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gwdykalwv.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/guhyongju.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gyvtsvhdf.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gjhxticll.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gyngfvtfa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gyllrttxa.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gmoavttqv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gpumctxiq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gbyumpyiu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gxujapyxv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gxdldbbhv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gkkhwqypc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/ggismqoca.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gcaiyrldn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/glqsosulz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gulocdcoh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gabcerjjz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gghdqedew.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gxqtmcseb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gmwidgpdh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gsvbivgpm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gzliarepf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsohkkiad.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gfltklmou.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggdyplstc.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gpogvlcug.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gwinljdwa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gzszfcgei.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/ganpgplkq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gejgzjiui.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gkfxszywj.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gosgmyjen.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gcpnaxqfy.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gajgktlxk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/geokjhqqc.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gmalzltjq.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gfftgdjod.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gunsbpzzt.sHtML

);
来源：http://3g.hesvh.cn/Article/details/glcxikzdh.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gobtkuqfl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gineaxhla.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gsaeaajfc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gfopwmodj.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gvaritnxs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gfywwubhn.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gddcycujs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gjsdeosyv.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gdtiaepnw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gxaalvmio.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gydxipyrl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gvlzvtnnw.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/grxizdmkl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gpebdffpz.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/glixcprvk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gbzzlaslt.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/geusbkusr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gfphubeqe.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gjytndncm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gkddlvsxx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gedodzggk.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gytpdxyhq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gckaebuqm.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gmptqwyzj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gxtfjoasl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gpwkhphgs.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gqsloivqn.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvtxrgwqc.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gjunbecvs.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvnsdjoyt.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gmjsloiuv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gfnlwfcgq.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gnddtjbzi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gtcgihjdi.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gsntqwsvr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gykaoktsn.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/giddqrurb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gfllycibj.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gujdqxnjx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gcfbfwffo.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gfczaaiqd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gkkqgbfzy.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gwmtrbegh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gltyasull.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gnhvhuprt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gthgshunj.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gzgrxwqxl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gtkfknqil.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/guofsssip.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdefgfcnc.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gwsirpaxk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtoekpjfh.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gfenvfqzg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/giybkushu.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gffrfvzuv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/geovxalbo.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gyktgsqvm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gdqorjhxe.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gwastxuvo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gnnwibkse.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gaorzvnux.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gnnzhctjz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gbytuaqxh.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gvlihynrx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gtpfuioci.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gurdvvzcf.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gqezfwmgf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gvcndvqwl.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gzxnvzcyn.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gvhsajlxb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gjzugdobr.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gayfkdytb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gjagnbfnh.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gxkpooioh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/giwaemeqz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/goygpjzdu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gbmojzgkv.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gyzdqqbqs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gwrjmveoj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/glcvwaynz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gcncxtvzh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gpbxptdbk.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/ggclwizid.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gmnkcxpnb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gwvgrhlaj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gfpgzxptw.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/goihtgicq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/getxijaei.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gftxcxhpe.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gouqkuyzm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gtozoszov.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gsmisdrhg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gcfoeqkek.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gajownmzh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/ghewgwwsi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gmwgzpmgn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gqyfrmyvz.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gryapabyw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gjddbnovs.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gskblkolx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gxkjwffcg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gtfrqloov.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/ghmukkdzh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gnglryyoj.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/ghkvyywrd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gfduvwwmm.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gitrjcomx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gjivceppd.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/ghsiaomed.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/grdbjoklz.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gvcbnrtpf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gpbssguuu.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gbzkvpehw.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gfaldezbx.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gxdsbdgqz.sHtML


<!-- 参考信息 -->