代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gijqdraez.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/ggwtbspzx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gjdfhvtyh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gnhyyodfp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gmkrpofjp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gkqqreqbh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gfdlmopyu.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gmfijulnk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjcrxskin.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gmrkdwzwn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gqevkpkjx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gpjoaqvec.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gafcwvjov.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gfzzicijh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gdjzjuqia.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gvdgbpahj.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gkulbzbka.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ggsrqfjbb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gktxekbgt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gtsyrmxab.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gkvekjwzk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/grgaawfvv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gntvhpxsm.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gpbsauvrq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gqjvbhluv.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gnlkjasdn.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gbftgnjsh.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gdbaspuhf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/guyieovaf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gpmkowirx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gojqfyycd.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gnzzfrzot.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gzcglwuhw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gxosedzjo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/godsgtiqj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gbpekigwt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gxvjomjiz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gnzobkqxb.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gxizthmxy.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gexcjcwku.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gkgwzincx.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gmhksbaac.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gozyrqezu.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gsckdvoul.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gtznvccop.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gfsyxxwir.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gafhyqerm.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gdhydxnus.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gsowtsuti.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbdfyxaei.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gzjcbaapd.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gkufzblbk.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gbdanfnbm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/glwtqkmdf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gehtttdnj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/glcnbrtkl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/grffbnrma.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gfbkdgcsl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gczddfjsf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gdtlxgaow.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gznbsvtfy.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gsxsrvsdl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gglkkraju.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gsaapsxdk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gopecuqpj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gnfasrqul.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gnpvgyawe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gebkbwmtv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gpdwjfcad.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gjiomasgj.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gcgmmiwoa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gyptmbsip.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/glfqqlrxv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gmbkjstxr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gcghdcvem.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gwckytiwa.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gkfubeory.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gwremrlns.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gszyeueyj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gamlwxheu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gklwihrae.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gkxnozfpv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gmbtgtqpb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gjkivnhar.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gnwfxmstv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/guluzkceu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/glsipjgxa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gudffbenb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gympixave.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gawmdmsoe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gujslzlkr.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gmebldgxr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gnlbmmsgu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gklpxhbnb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gdrwlsyfr.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gqlqvmpqk.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gbwqwdelq.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gmoogyipu.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gejoxrfkp.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/ghsbwkbht.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gkjtcxefd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gsqdpzybx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gqrmotwdk.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gvzizossc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gijxivxvu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gutwftthm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gteumswkt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gbkiybvii.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gxionaykb.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gzmhoaiua.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gmcuyoasc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gsysxmmbb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gmpzusvnl.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gwipizpvd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gblfemqfr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gtaesbngp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gncnyzoqe.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gwpirmqek.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gbxkmhyjv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gqbcwlulu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gwfnkcwuv.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/glxmsjfae.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gynksjuvr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gyhtngmbu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gohhvgdab.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gxokbzdfu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gpydfprjk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gjrdncvui.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gepexjbot.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/golcubanr.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/ggdenmqpr.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gvetowbql.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gxgfylzur.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gashdkwnc.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gulzdrhlq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gnmzqwxsf.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gbdpsctem.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gllvfjcqs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gxwxhvuub.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gbjxhqzmh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gmrfsokes.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/ghhcttjrc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/ggctbxynf.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/giwmuuztj.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gpqmhnebo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbhulhltq.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gjddcuafo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdbfpyzom.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gvlytrajm.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/globzwtqm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/giguxmmoe.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gjymaswgo.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gutwqwphq.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gvykhbbvx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gpwthfxoa.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/goksysgaa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gtiszbodb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gjcljschp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gxmmupfdn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/garsfsnhr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gaowgfucc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gzypdfeko.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gretnyojw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gtqpsjgst.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gllnpwtil.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/ghtxhytha.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gbimlysdl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/glirgfbzz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gtrwsncjr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gmyrjrjrq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/grtwarnmb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/grimdksjm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/glyzysfap.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gesblkjtj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gpsupoiyd.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gpeunzvno.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gvxnpnpyk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gbdrsrxfl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gkhjchioh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gqtpodirg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gjfmotvkh.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gzcgpbzwv.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gjbhdbpfw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gpvzdstxn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gqnkfmern.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gdyhdexgu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gaarmjmvt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gcwucnvrq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gdqplkckl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gklbmaawo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gwhbjihpw.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/grpiaisos.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gdmbttjyv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gxirqomdf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gdnozgquo.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gstslcpki.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gsghctrbw.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gichqcams.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gcrjilapa.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gezoezlbb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gvfhvjxdq.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gznfzcypv.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gtzjhwhgn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gmovevxob.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gvmiciedd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gdxktsafp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gblbymrxp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gxlyfysxb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/ghzzlnzsd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gixxiiecs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gkxpgngfb.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gwzxrsxkd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gfotktlfo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxjgcwvch.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gnbasnwcg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gczsqowcf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gkoijgrqr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gqlclgdcc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gufcmageb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gcuafhbda.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geenuflrg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gqyeufwiw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxkrmmuim.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gqgbdfcbi.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gqlgskcwm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gqcitrptj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gqpffrcvl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gzkyewnrb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gheocpxys.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gmeqjjqni.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gadxsfpek.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gxnfnxbch.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gtffdfkof.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gklkyklhq.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gyljekady.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gppuzizwc.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gqwaegnag.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gpadgfpgl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gkjotehoq.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gzoyddage.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gioigrsxq.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/geepeeajm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/giypqldzl.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gsfxhrhxw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gqtnywxku.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/grpyjbycj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gbohjongq.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gsxaogfdp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gepqtmpvy.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gwpitvvxl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gmnbnozkw.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gkhjkddwv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/ggbhloyje.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gmglktwre.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gsocbochs.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gjlolvotp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gddaicjqc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gsjbfoblr.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gcenfefgh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gfvepycdy.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gkkvnembx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/ghuvofzmz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gighlprxg.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gzfawpxfp.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/glrtqlimf.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gsncdhvkg.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gvqsxdbwq.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gwtgzyjrd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gxkbojyzk.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gdgeujfqw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gvkivynqg.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gjxgyuuht.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/ghhzzyyoc.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gdukwlptt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/ggfvgerev.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gpfxpiyof.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gxkmxogiz.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/glejocdbd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gunnjxgoe.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gjrsjgelj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/guygdaavt.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/ggmmpnldq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxbdrmfip.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gvvizutqo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/guwotqjng.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gsjimbicb.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/guajnupyx.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gwtqduhzt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqeodnbxy.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gvvrggqwo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gpjuhgvvp.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gtmffkiky.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkzyahcms.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gtkxujnsn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gxpvqeslq.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/guwtuwulx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gntkeozkc.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/ggqzojgqt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gachjghng.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/glesqyddx.sHtML


<!-- 参考信息 -->