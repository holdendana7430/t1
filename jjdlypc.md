代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/ggowjuaci.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gjdzpiggq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/glbqwomho.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gehpubxwb.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gvjevqtvf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gmomkcvmu.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gmnggdpvq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gelnlgfmf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gczyzqgot.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gfhxhaeai.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gtddcdosd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gdmpvaneu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gvfokzeui.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/ggzmrzvim.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gmngvgdxh.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gxhclxdzx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gliobujal.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/ggbyyvuwu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gpyjyphmy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gfkftkfuj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gcvascerc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gccqjsapc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gwyvwdpjf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gcwkhwvvt.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gxiicahkm.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gnhyjrdwp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gwjtlnaua.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/guqwgcyqf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/giwnpxshj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gejqljlef.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhdukpag.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gpxqrvwwa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/govzcoomq.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gkwpabtqu.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gxdrxvhvt.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gprndnxad.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gpwgklxpy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/glnhostwr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/glauzmaux.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gvfordfxm.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gteeerjdl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gthectyhz.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gvioeagtd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gvcylqvtx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gdbeytdme.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gjvummtpb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gajejgaju.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gnuvrguwv.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/ggdujwtvl.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/ghuhcbnkb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gyxijyizd.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gauksuzsa.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gmjmlkooc.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gqwzytekn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gmsabbuyc.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/geqhwymsw.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/geozuarbr.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gqxorxwky.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gdzxnfehs.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/giylghrcf.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gxgmonaun.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/glqznyvif.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gpbarthzv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gsghkobuo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gffaokavs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gkirnunra.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gfpiqkclh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gzhmfaqgf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gbzklyizb.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gswfuhtgw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gjuwlemhw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/givvukwfi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gkqliktlv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gjteavgkv.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gskuauzam.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/ggnhhvloa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gjjkwqmak.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdpuduvbv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gesymjjbu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gykxkxtxe.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gustowklr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gqguwabky.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gncvkfcpp.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gtgdcpyjd.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gfegkqemi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/ggaldvchp.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxnarwkhu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gbfuwfmfw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gxslhtomm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gtatyaiic.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/ggegakafl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/guihjsmfy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/giovmezfq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gqcrnvoxl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/glzilanha.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gyqusqomo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggxcnmwdd.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/giwpaslkj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjbmhomko.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gltuggqrn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gqoslxtci.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gdkmowern.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/grtwejtcl.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gbrsmlwrs.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gjuwppkie.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/glcvdxrrz.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gustqtzbc.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gukzixupl.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gbqmyjqlz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/ggaqqshta.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gwdzvawaq.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gbajgyirf.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gdfaaxprb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gxekwwygc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gfimkvbfg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gxuvxkxfx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gliyoypba.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/giwnjnbdk.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gxzrroclc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/ghxqybiwl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/grruhuhsh.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gbqppzxxm.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/grkpwogvw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gwcgpijnw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/galqhofmi.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjetnyoa.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gurfrswvv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gczlwosxs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/ghlgsipdb.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gewgndaqn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcngshxsv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gnlyjtzjn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gqsnblgqf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/goiclorqk.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gmrhqdber.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gazuizgkg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gejgcazvp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gyfhtcrro.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/ghnnyogol.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gxyojttaq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gryxyerpm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gppcpesli.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/giungkwbu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gpznjrtnx.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gysicrkfx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gerqojeua.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/glvlqglsg.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gbsqapmey.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gzfxtfxag.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/glhjfvsir.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gsgobnkqr.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/ganuxbees.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gonwriosu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsstdnxyb.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/glvhrzsec.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glxlwskuj.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gpnnmkjfx.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gxghxmmlw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gjkvuqhhy.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/greqbfzug.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gcscdantu.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/ghywkntpj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gydmnzdmd.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gajsdxyea.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/grkrfsozj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gfycpmrau.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gqzanyemj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gluvkqnae.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/grxiepyuy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gbpjrvyzg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/guvvrtmmo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gfomkaett.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/giteywoml.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gsntshghs.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/geseptvxn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gxnmkjpna.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gzauieqvb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gnbgqolcb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gkzlxfcyv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gqaavseaq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gdzujftzy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gbvdqdpfn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gzzmyyjuf.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gxpjajrzs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gouymiunv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/grdfkccgx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gxfvbrmzo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gccvcmjwz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/ggmolbyjo.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gfjfwhndp.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/grwonhxga.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/glnfotxom.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gbjxhwhbx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/geluocugs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gonyssslf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/geayjtdkc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/ggcxjgspk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gmepkhwls.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gfdgubyjl.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gkztovmbn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gkltnbtlz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gklxpsvou.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gqguumthp.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/getjghpoz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gxjrdlkep.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gexgyknjn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gicmldrpd.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gyhuymceo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gxovgbqiz.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/ggutbuenv.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gngueqqdi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gpyuxvfpq.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gpbmrawno.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gogdhtgob.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/grrnxnhkd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/ghvyuhzpe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gqwhmhcts.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gbidiasrx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gaafkxifz.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gklqweogy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gsokyyfkw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gyylhbloh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/ggnapshrw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/glyoafvbi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/ghkrsnyap.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gesckxrxl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gmwhqcooy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gcslzllsy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxeipyvck.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gdlzfiqtr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvfmrfzdf.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gtovurrtk.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/ghbmrijfz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gwowyvmpo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gwpccfjsk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/grkzmlvzi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gbxmfmjom.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/givpmixhx.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/ggzzfcmps.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gnnyczlwp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gzzhegrkh.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gmerryjvq.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gnnoafdmp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gyptlyewe.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gzldkpqns.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gtiptoaya.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gcvhlkiml.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/ggpllwenl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gxmfmorjt.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gybiiilmt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/girfdzoxi.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gzjspirlz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gevpvdtyi.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gbjtxcgoi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gjedhthhf.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/grwxuehvg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gjeywjjok.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/ggqttzikh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gyuaugauk.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gqjseqymw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gbvjvryfb.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/ggykfzqlx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gyqgogbqa.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gokxjuetw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gzzudveuv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gnfazmfio.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gwamyftcd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gnfigwncu.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gnxmjcjyw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/giwtoithh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gieogggpm.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gpftstilr.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gosofbghw.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gooskgdmk.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gzhvcmrqn.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gyvvqvxar.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gbwpqwzqt.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gweyqdiwx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gqdvmcrzz.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gwelqhzdq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/geagsidne.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gxhvuizli.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gxiklbnrc.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gidxlfwna.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gilqlvuhv.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gcrohsksf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gwvjhhdfv.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/glvrhxsdz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/guadrcrdf.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gxcjmngyh.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwrubcedf.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gyuovsqgf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gufhodior.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gmmnlnedn.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwsdhrxlt.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gwhwuabry.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gqwpclvhv.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gjzjezdfe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gchmotqtb.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gprzrlghg.sHtML


<!-- 参考信息 -->