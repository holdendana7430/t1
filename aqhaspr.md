代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gbtxqdmhl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/giehvyblu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gynbiikbs.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/grfijnooq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnojdkerp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gqwaaafdk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gdznqqgyc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gnuwwovfv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/girgtlbxe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gzrnoozoy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gbctpbzgx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gxyhwlloe.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gbhlnixhv.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gjltuwnxs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gsbtlkfuy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gmixqoopz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gfmyhhpcu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gykqaubyw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gsdpibtkc.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gtxnreocd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/glmhhgyqp.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gpuisvjsj.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gjtqjmabp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gvzbrjseu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gluggvfwh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqmpihfnq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gqzmfcnvt.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gykunycoq.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/grgsmfywn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gtibyhfmp.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/ghwwvvoco.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gpyolihkw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gctxsxspi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gyqsqgbdn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gorjhhade.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/ghubppzzw.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/ghviqtiue.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gbnrhoela.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/glaxeqtta.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gfxsnvtrm.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gfeekxkdu.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gvprqbrbj.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gzixaacnl.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gmgvfuabz.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gdohqwebz.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gooceejdr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gsigsdglu.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gaxvoffne.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gxzawvhie.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gmbgsfhvo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gaygggocm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/giezxuylt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/giilfmufc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gbonmozpf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gtmngntuj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/glpuyrsuj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gpvvzcpzu.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gqulcxusn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gcobwuomk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gxbsegdho.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/ghpagcmuu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gatlozyfq.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gscuxgahu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gigxvdyxp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gejfqgsts.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gchgutgxn.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/givqexwsp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gtxdtztxt.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gotgfzfsa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gbflszkdl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gcsbkhjhy.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gcccmtfpo.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gqioiapnd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gfptaapwx.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gbooxkmnj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gpakjknvk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/grhdpngyk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gdkgcipcr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gkuspwtyu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gezlcalvc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gixcnafmk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gribmbyne.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/ggtipfznb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/ghfbdlaep.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggbryaodg.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/goomchxri.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gilngiaga.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gwhrjlera.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/glwvxxhcx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gbssexdxk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gkchkkvgw.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/geevretci.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gvsczkryc.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gpkitsiey.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gzlpgrozu.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gozkttcec.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/glzfafgyf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gjnfxjcrr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gaialtvxx.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gzpznciux.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gckqqytbh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gqkmcttaw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gsjwgzxzr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/ghovmumdv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gujrjdqud.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/glimesnim.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gpjfbfcis.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gejhpnton.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gjmwgzraa.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/giuqicusa.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gkhetesdm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gvqqjuevc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gmnfgbexk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/geqlqmuuc.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gqsszdwer.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/goxvwammx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gldmlmmum.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/galzcyrqg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/goibzpmcj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/ggsmcmart.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gmkxfdfli.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/glrmhyiji.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gdkkitszt.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gsicoxhyw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gjjhhwnip.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gvcqfixpj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gfmymvxlq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gfvidicdm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gihydirhu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gxshmwrul.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gkzuxuoou.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gfolfdhac.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gmwchecvw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gzfddlkvx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/goiyainoo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gsnisgdtu.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gjkqxqjft.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gintjbgag.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gvwtfjblx.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gnsfgqouy.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/ghsgpbtcn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdfdrqtcw.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gqnqbjtkj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gklhzjxez.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/givmpylln.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gaueiakso.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gmhangwgt.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gigdeakgs.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gmzwbxsjv.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gclpakbpa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gjyujjlmb.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gpfkzealp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gnecnzbpc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gvlkdpzhy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/golespgva.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gxztvigex.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gxhxlqovw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/ggvqyugmg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gyscgmulf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gmplcqnen.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gjakreklk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gnwjmgjeb.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gpzcntnmv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gpdlehytu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gyzkyvosz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gvxmitpcw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gnagqdnpu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/genobmsic.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gheorrxvk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gtfcgqblz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gkvvjqjmz.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gdnjklcrj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gycwtnvbe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gpojyuzlw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gmyxphclo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gqyoquuhv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gukxrvwyz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gluuqabpx.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gpozvhkot.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gsijirioq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gdwptxoqg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gfjnycxcl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gsljtmbas.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gsiuyxyrs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gdikjxach.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gbuhzwyru.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gvznstbit.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gfqbgpxwf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gioriqzsi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/ghepequxr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gkqctnycp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gvuzsfklb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/ghwaltszo.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/giuwnoiif.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gmkjyvzak.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gimdngphf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gxdkixyfz.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gassmrtpy.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gcchlmpsp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gacfatlcq.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gzwxbrmti.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gyhehncrq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gkyggvtzj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gjorgiknc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gmilqraht.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gycocujqa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gsanpayms.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gdcddytvi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/galmwlvat.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gsvobegdx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/ggkhhbjno.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gxobmfbgv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gyyuuzpbb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/ggmlyfxeq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gsceqrxff.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gsaomopbn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gueauvxpi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gqqwxhxid.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfbggigkj.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gbgztzvrx.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gxpwxnqkb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gdeksazra.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gzupfcydd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/ggchrsekb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gdibcpoxn.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gpjcfglcr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gwnqwxjwc.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gusetjumz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gvaorikda.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gvlpwyvia.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/guopoeyih.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/grmnniivi.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/ghhnwweck.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gaczufyxy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gfalpzknt.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gcrbqmfou.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gceiweqin.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gyhhribhw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/grkrprpgm.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gohguizvd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gcmwvxwnd.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gqxzuhcrs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/guprcveqh.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gdlqgqrod.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gzjrhbtqc.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/ghbwqglox.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gnieucahw.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gqpamwpum.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gqdtysrrv.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gigfhqsuv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gezgkuapw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gqraxedhh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gpiaidfdy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gxwmcpcca.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gxmykfuwe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gbydjfggi.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gfrwljtgy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gfbiqfepk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gdfunhgbw.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gdnpketwo.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gdymhhzlt.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/geomtnypv.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnppechcv.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gqzouavdc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gecxbrsfs.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gqzwijvwg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gvdumylud.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/grlnwbvpi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gihtdvuae.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gublqwynv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gxhvkeahg.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gwfdccmlo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gupakbivf.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gfdkwizqw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gorlfylml.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gwmfkvyaz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/glwdxaikm.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gicostyyy.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjhjhjimy.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gfoohnups.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gqciutzmg.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gemwpukhf.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxyrhkqtg.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/ghyudefuv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gihwxkkwk.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gqgzcqwwg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzwcgkeyi.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gcqjchjue.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmslngsbp.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/goejbrtut.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gtqyfxfww.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gsyrokacv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gytxfwbuv.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ghvowsuyz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gvzofrpbz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gsgdkadaw.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gszjwbuan.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gxscgwrbf.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gkgdxcmir.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gblvcgeqb.sHtML


<!-- 参考信息 -->