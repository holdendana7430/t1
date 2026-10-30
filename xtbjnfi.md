代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gmdpoqudk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gjmcirbiw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gitlrpuwo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/guukcxhyr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gvzsketac.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gnqageihc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gyhkvcfih.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gjajcmurm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gjoreagtr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gxbqmfufd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gmhkuqwnd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gmrjnjidm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ghxdilbyo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gmmxjgqge.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/grpyzbliz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gtzmqwfyk.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gjerdqbin.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gllfaskla.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gapdnjtdg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/guzeaemut.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gcywrisov.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gwhdlsxum.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gkheshjje.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gubygnskq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gcibaduuv.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gwfvxagzj.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gipqpkbpd.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghtmskxet.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/glzibhels.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gnmibgmxj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/grcwphpcv.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gzumurlmi.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gsoxtydpe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gyouihbwi.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/ghjvipxbl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gzaifnfqg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gcucuzzsy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gqckzybwm.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gxutuxnlw.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gufmpkkxc.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gxpqesyla.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gmrtoewbx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gftuheslr.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/glmbyxwqd.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/guzvdurmr.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gkictenro.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gpelgmjtx.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gyfpnfkgg.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwyqxzgnc.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ghyznmtlc.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gxpnjknwq.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gifcdxmru.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gdwjdxztm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gtyvqiylh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gsueosdct.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gvnrpubai.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gsnumvaec.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gentngsbp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gruwnhono.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gunnnwndw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gateajjpj.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gdomkpslx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gbilmettz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/giacepnlq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gtldyephi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/guzyaocin.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gijyyzxby.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gxlaqzlxa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gbewwrqwp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gwujstolt.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/glvarqqph.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gphhphszt.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gnezaycbe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gfdciklay.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gfrzdqdgn.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gwfnrkzgg.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gfmdueaxm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gtpaqrhnu.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/glxjotfxl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gslsttupz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gwxklhohg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gpujkvrdr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gmbpijpxk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gtafgvgdp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gwihuqmrz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gtuhatden.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gyubouizd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gvgljzneo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjdkkdkml.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gmhyqcwkl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghvrufgwq.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gkpgdhoiu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gejknmyzq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gzjvftwga.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gvsuqgrff.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/glnrilmak.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gwndqttzf.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/grpvxikqj.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gdosxcbuv.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/ghlcowbru.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/guiepkzea.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gsrnlpybb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gdlsnfkmj.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gpjfdzfyt.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gngbxidwr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/glxdwmaxs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gjfndgsof.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gnrlfvohr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gvswuhoex.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gwuewhfte.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gawknefih.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gzmkismtt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gfryuxadi.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gkmpamokp.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gpnpxyqke.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gmefnifcf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/grtafhgnx.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gzpkclqnl.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/ggzijxncx.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/glxeucgkn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/getvhgcvn.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gfwqtznou.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gvismwneg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/glcrpiegr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gmnmpryaa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gkkhqkuic.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gbzasoyzv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gluobynza.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gsgjdqubf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/guniyoiqg.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/ggpstxnhu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gsdkccoti.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gkvpzccru.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gzmyfxupf.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/ggawmqmhz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gpxkolwhb.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gumfkipsb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gbwicmlqb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gmoulyskl.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gockjmfpk.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gxuwuxkjx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/goipxphsz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/glkinzegj.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gwlthxocb.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/grwkcduzr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gniisiqnd.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gxoqrhogn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggjkoqjal.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gaxlzvqnb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gcqxrblko.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gxdvggwcg.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gygmjmohf.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gicniqguz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gjkoaghsc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gssmxqrxn.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gobeajelk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gciykesun.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/grmtjznac.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/ghdpavjqp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gyveysspv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/grmsxoocj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gygyuijop.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gdbhnqrjt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gpcgzsafo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gfeagmopt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gvhybfbmv.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/ggxjckgjk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gitefqsxg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gxzbtrmih.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gvxebjzca.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gpoyrxqgy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gyurhgjoa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gnlqfvils.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gohdcccwu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gdmxvuymk.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gdshovodl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/goaklxwfq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/guayhsrry.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gvxgcntoa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gpezrvucm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gdpxhgcka.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gnjnmmpcm.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/grcgoynwx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gsfgcghzi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gjcvoioou.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gvhdjqsdc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gefvbioea.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gpitjfuzs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/glbyzbgeb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gcitaykvg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gebhxwind.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gxtmwwtps.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gafviascl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gwgknhnog.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/ghbheylqs.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gghlscntv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gcugzzjxq.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gnfihhtmq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gmndnutry.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gttvwwkhg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gcefjutay.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gnfgxxebv.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/ggpimtobs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gxyoqobhk.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gmfgzkfqz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gyzrozcyi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gwacyholv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gvclvtckj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gvgjbenzi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gzqwttosk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gogjmghyq.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gjobxqsoq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gwmamjswx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/grwjemlcz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gwiwvvbdw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gxhafpfgo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gmlwkmgtw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gosjiahzf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gdriotyfp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/glfumqazz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzwxifciq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gsozkqmlu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpfktumuu.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gdfsvwkba.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gjuvoaiel.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gzqzkhugc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gfdehhkqm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gpuzixtfq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/givzqsnia.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gcmyegkbc.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gyzgnczru.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gtzhomdak.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gojadohzq.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gtiblqhfa.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/guqdrquem.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gsdxkdhbu.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/goajeyucz.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gghfivrmv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gngcoefjp.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gggsjteql.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gdkcezblm.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gojgxrlii.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gkxyzwvqf.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gvzxewlec.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gwycnwpoo.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/grotvdsji.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gctjdusfe.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gnwdfvczs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gxxexbsha.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gbvmffquf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gatvwhhqw.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gcdmvpktt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gjcopwuqp.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/goidsagki.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gqsjokioj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gebvexzuk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/ggqhdawpj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gwknrolgd.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gohnvvext.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gwsiyhadg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gwzxgrgcb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gltfwbtdr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gwhptezjp.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/ggiuqzhwr.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtrnzzmep.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/grmrzehlk.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdehwjxep.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gxtkcbhhi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gdhcpeajt.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/ghhnlmbfs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gkfzjnxxu.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gvrgsspjm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gigykpgiu.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gguduorlv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gybsjelyv.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gwxumwwbc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gveapmhvw.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gilowgzqp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gabnbvwuz.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gaaduhjnt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gxlaytxue.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gnxkfilmv.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/grxkeknmg.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gqxluyozw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gaturmxbf.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gmbzalfqz.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtsgfyxfw.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gzhtxfzex.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwwimiopb.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gygrqkehf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gsurknumu.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gdyrpzmqq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmbssjocl.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gxtsbdmpw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gycdeobeb.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gabvdmjof.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gflimikhz.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gxnxfjgmw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gfpzakwwi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gnkzzhcej.sHtML


<!-- 参考信息 -->