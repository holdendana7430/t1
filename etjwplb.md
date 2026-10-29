代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/garcdrxhy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gdbfzlpuq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gqmicrorh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gpumcevyc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gvucgfcam.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gyzsjupiw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gaqsscrna.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gxendiljo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/grrtdyiin.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gzfxvvcqc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gpyzholfm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gmcbkwfqz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/grdxecbqv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gobxispmd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gljfzenlg.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gdpviuudv.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gollkakow.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gdsqbsqap.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gdorvzoie.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gozyftbvc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gqsvxfhuh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/goiiqftuh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/ginifsmtr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gmcevbevm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gjdtyqxrq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gxyxgnneo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gbhdkzkcg.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gfzftessn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gtomedfll.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gaekuuudn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gwwvvvqhv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gbktqndzs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gxiadlyya.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gjupctyjg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gemskmoln.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gsbpmqhwq.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gcdodeffm.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gwjzebfgd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gmuzxrsds.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gtktriztu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gevgyrzxn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gafsrosor.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gizbiwdtz.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gvvhzkhwl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gnpbckxai.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gkkyiidrd.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gltfuqezh.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/giupdfmzy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gejozomoa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gbrzlnjqm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gaimftofr.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gsabpqukl.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gynaunosn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gnbwbxqvz.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gpgwjilml.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gxlxzgjrj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gkealiqxt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gixxskpta.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gyelxvlok.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gwnpnzhnn.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/grzkvnqxd.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gfgwvswcr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gkwxbdfio.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/grbldeguw.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gfsmlweow.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gsnmkxzji.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gygawqnim.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gxouywemx.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gwzkzsdke.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gblzltzks.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/galcujffg.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gpzaqkdrn.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gwbdgsidb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gbdtgnppq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gbduoyctx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gqrnmxzzb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gbgzerbcs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/grymhxokt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/guijqekmr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gpgrddubd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gvavcwcoe.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gbkzetshe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gwfaqcugy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gmatzzkaq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/goqikrhny.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gnnuhbdxb.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gwpdcdzxo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gdpfrgkhm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gvvusqgxd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gobgocjgy.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gstqkhqyf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gaipjktny.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gadrlyito.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gybakkrgl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/geonzevhr.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gjlnbojnw.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/ghrvgtvcr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/glrogoftw.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gvmqnupqs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gzvkdkmwi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gsnkfcjkf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/glhwhrpwk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gaoyktyby.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gfoihmdol.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/ghblhfywv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gxoextgtm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gxrdacjzv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/ggjghzkcq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggeqrbitq.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/ginbluzff.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvhmvfwaw.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gnircncys.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gmnvkcvei.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gdmkxqnyt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gmmrhrlqb.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gulkyyaoa.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gevlyahzp.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gxbjnuuxb.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/guanwhemu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gemwlgdbs.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gpexllycw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gkqtwacxg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gdlvjqzev.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gpklkofvy.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gvnkyzxiz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gleciuuhy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gltbfnfed.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gfguglsxt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/glmiagrlo.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/guiusoiqo.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gisrwzuzc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gwzhtcadb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gxwbvewnb.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gszqdrlmi.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gnadgsgrm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/grmckraqh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gjgjljwxx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gzbufrrum.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gubwdkxxe.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gpuiaawxq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gnhiwshwa.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gqzjyojjd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gkrcpttrc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gqjcirapn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gpqwauawr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gdufhpclx.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gyagsqjrr.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gnplayclp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/ghzincime.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gnasojrxn.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/giuboyodq.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/glpkrgnqf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gzvkuophv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gdvxjessi.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gevjafgoq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/goapldxsu.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gnfbomxog.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gkaxmhurc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/ghsosefeb.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gdycvveyy.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gnpdrtzmk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/glaqrfjjp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gdruifuev.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gjqarzxvh.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gbfhxbywe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glmtrumga.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gjulkbvup.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnsapixgx.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gqtruygry.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gnskejvxi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gcguqgwmm.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gnykukiys.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gqrgkslgr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gzdbeeodc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/grdmxsefo.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/ggcfuklyc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gtkyhrkic.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gbncbhofb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/giapyelnn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvovsrusi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gistwbyyf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gscpnjaah.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/grmtmtfuu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gqgilkgaw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gdwvxstjf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gghesshrq.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/galyykecv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/goggovedr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/ggdgvrflq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gnahcvrvm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gggdrtsus.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/ggiestdjt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gbjoivyio.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gpkyeivkk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gggdrgctz.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/ghprvfopf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gtpsdfjwa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gntilzcoo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gfmglxkqr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/grvewscnq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/ghlclefcm.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gdojpqiec.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/ghovreivq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gcpzhtbri.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gqsodtexe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gwipsxxiw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gwzhbjwze.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/guvanqyqk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gbpkaydvj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gsynlzxba.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gsyawybqh.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gtuvifixo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gejjqcwln.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gcrhzbuds.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gzrtbwxie.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/ggszoqdli.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gurfkrywc.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/glidfnibu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gkqwpmvwo.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/giuudacbg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gimhowhks.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gkzsfdulm.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gzseewuvl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gupwqvzfo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gzpteuufz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gmbpxbmcf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/geinrzsgu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gtsftvasi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gwcfknqla.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gmaetvgak.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gqtqavysn.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gimqxitqj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gfroghkfo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/glzpviham.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gzcdtfrou.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gphqosywk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/ggdbirlvv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/ggmhhwtiq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gyfhumxvq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gcmhtctdl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gurkxbvpb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gwrsyncke.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghamvfkhv.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gvbpkhyhv.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gapannppo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gmokkemle.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gohatcbny.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gfupubvuj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gzbjjuwmb.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gyksxzcfo.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gtkdhpwmg.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gcgmjyfoc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gpljwpoeh.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gkteymhwv.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gcyipbhtm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gsjftfzyl.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gammhntzf.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/ghehvajxw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gkfkpazhw.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gtnrnndrk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gibplobvt.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gmvfmgwyt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gvtvpclyf.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gxzvrenrl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gmjweaqoy.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gntbmoebg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gdgqqruji.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gicndkvir.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gjtyrhxxe.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gfkiuihdj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/guqkhxbue.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gulcbejlk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gegaktmbw.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/ggkmswfui.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gfuuqqqeu.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gipwehhdg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gcwqjwgpt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gbtoertkx.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gxvzsunso.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gseilirtb.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/golvulham.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gviytspem.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/ggbbenqui.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gvhlwkmen.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxipmjuno.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gehiakhlv.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtkajhgxc.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/giijtlzem.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/ghgrcrsay.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gxkrcyzqh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gospzlfgz.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gosogoqco.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gyvrjqcfj.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gdwqghxah.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gpogeepfl.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gmcsoualo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gioejshwb.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gnavahesj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/glrshuuag.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gsevtqfix.sHtML


<!-- 参考信息 -->