代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/giqantygl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gzvwfnwxh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gmcdhykfz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gfueigulx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gzlkfakcu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gonnrzjhh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gvtmcegkp.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gxtrxbdev.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/ghcesfssw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/ggvrolamr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/ghruffxiw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gwpmkxlxu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gcnmodowo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gruxapcuj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gwobobbkt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gwkgnrngm.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gnadcziuc.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gagaocuol.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gcbwbqrir.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gemoorkeh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gtlveadil.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gwnjbsgpp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gvjoegcus.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/ggtmxiszu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gpvuykuyv.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gmaignwps.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/glhyvbvpr.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gccajhdxs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/grcenevkk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gykqzycon.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gihgajnag.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gxfdkiuya.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gyljnciuj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gfbxquqad.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gzyvtfvmd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gxaobutig.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gjcwqdjes.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/greofykhj.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gixqkdhic.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gvxjbqtxn.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gyukdnkue.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gagovcalu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gqtlxcmxe.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/getxsvieb.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gcvpehrnk.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/giaqkrbxy.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/guylemnhd.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/getdclzur.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gsmynstzy.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gnkozcztw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gglixvqwt.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/glknvwref.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gsykgpsai.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gitdfkgij.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gsvkejfnp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/ghqenltjp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gxgkldxsx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gdiuwnqak.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/glmwvvylo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gdlentjsm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gpybabixi.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gfbibrmbx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/guspabnkc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/giatictug.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gzeytjvmm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gflnwfoyh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/guaoxhfji.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gqjchxlhr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/guitwjlgr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gbycshcwz.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gdurojlmd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gbeqefnmk.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gkccjxjen.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gtbloiiiw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gbpzfoxyp.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/grvopdwrm.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gtbfvtwuq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gxggspyri.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gjhgdluwy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gnopjckjy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gstnqdils.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gqdvoxevs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/getzqirss.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gssawukuy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/ghddykslg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gjyeztbxx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvicxiyf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gkgmbmptz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvluwdynx.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gisxrwieo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grazgifkx.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gihilyywy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gsqldlkag.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gjthzpkal.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/ggzzhczld.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gmdohkmsi.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gkaddkzey.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gtyyrrxam.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gomcjmepi.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gtlctswmu.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/ggzgmjuqq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gggqtpfca.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gdpbfvzhp.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gmpqazxjy.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gvdemtzpu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gdsdfnjvs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gwyaesyub.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gfiuiqpvj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gyxgsqujk.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gjwnnukxm.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/goxnvcphu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gbvvvzysw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/goazdmkxl.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gmuvbmyzj.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gpxafuhfm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gyqppxtwp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gsdtokrwc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gbofsyfbz.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gigwrovqn.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gwqlglpka.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/ggftspkjn.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/guukpbbmv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gpfvoqodk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gnyrocwta.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gfarhxwjo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/ggefrrlyc.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/guxkdvruy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gmnqfqrtg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gobooejxx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gjdgsfqbf.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gbavuihqx.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/geywfvqhe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gfjkjtdgc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gwddpunuk.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/ghzkrpogk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/ggvcabmbu.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gbsxgyuny.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gxyagzrhk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gqtxjddgf.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gikkpiipx.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gddcfeqoh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gnrgfozld.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gwgqsouhj.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gndbulpgk.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gzpdyiadc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggchcsuly.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gmhkwslpt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goiuewbll.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gmkqtdsof.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gqivaqijg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gtlueyrww.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/grolvlyai.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gsgznnkbm.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gxvnmqhdg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/ggwiwouqx.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/ghdqtktlb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gvwsgbybu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gauiaqrke.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gfbmpgvgu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gayiolclf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gvgrdstdl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gegjbcsqg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gvssltlor.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gthphabfd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gcgriddxk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gbxtrvpep.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtydsufrx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gyewblsov.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gizrhsrpx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gchjhcsrv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gymwtnatr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gbcugswsg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gwexlgtqh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gexpzvpbc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gdahdpkvm.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gtqnppebo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gcildcygk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gdkhxvowj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gxtnvfpqh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gagzotlqe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gzoerivmv.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/glojfvtna.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gkvjyotco.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gzugdkvig.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/guzqjjwyx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gagvoeoel.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gpvslaccn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gbgbdbusp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gatvwoafd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gycsxljcy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gndkpbqom.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gemisxcpi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gaswxnlxf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/grxeslxnx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/ghxakvsdk.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gtlyvvjmd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gjkzkcmyv.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gqqnzbidp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/ggbkluewm.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gkyjmwymf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gjpyriifx.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/ghytvpbof.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gvteuccqb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/guwsypmqu.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/ggaqqqrcz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gtbkevmdu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gjwudjnwv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gwbievdle.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gbspyovjk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gnekcudyd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gcjsfqtce.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/grtfvbmdo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gufeoeplv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gmawujcfd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/ghifnkene.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/genzjqzqv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gzghoizhx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gyzwisnjd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gmgppfvtf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gybrzogck.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvoujvddz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gtyhsfkyc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gysvzpiuq.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gadabwiyv.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gfesxbbdl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/grwvvoymk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gponoltgu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gndpfmtkc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/greraasdz.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gqbybmnnq.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/ghpnujkvi.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gzffzrpzu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gtypcipmv.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gadbjzmrv.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gvojzqnlb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gbohlutru.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gfbaueixb.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gsrbnsivj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gdwrjlzpi.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gvcaulakm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gyiijdjry.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gyicvnlwt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gcexolzmn.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gjryqfvjz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gvxwdyecr.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gqlehfovj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gvzgnouhm.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gzsuejyjd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gmiqdqcuj.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/grrcvhmhx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gndopvapr.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gmfqwsjah.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/goxgadeyt.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/guyqixluu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/ghugbpdfv.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gllzelqvo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gdnxjgxen.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gjpvoytqu.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gvflhzdzo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gssotzwgw.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gonyeypeb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gjitwpyoj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gbryspllb.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gafjautol.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnsjdppyt.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gmlphfpqo.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gevcqnecs.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gucvhwvyo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gzgypvuwh.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gnaqycrgu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gzttyvsoz.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gnxykgjmf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gjwonswjk.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gccimzkou.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gfitjiken.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gmgjcfayf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gaihlvqng.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gwtbdfawe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gtqodgpaj.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/guxmgcwow.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gvoexjpbj.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gxhrxupfh.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gduarebbv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gldinfnzh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gxqaqraok.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gimozlwjz.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gtkoaszfy.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gnbdmxjtb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcsvdgwlx.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gddlsjbqn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gfcjqazwa.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/ghdqgtjpa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkncuhrsf.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gichjsztw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gfsercjpw.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gaziwwlob.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gfeackxcs.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gzbtddvag.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gcppjywcx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gtldrqlro.sHtML


<!-- 参考信息 -->