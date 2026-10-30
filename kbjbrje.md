代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gqhkxxewz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gwmgtwuzv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ggzmfchru.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gumoxlppr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gpdwvkreq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gogcobnlw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gcldlwvla.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gmuibmtfx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/ghelckwuy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gjdtypyzg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gszvkvnhi.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkmrateij.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gfkasloci.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gmucnuthe.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gzchvowbm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gecvqafrk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gmhfkndom.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gnnvwacna.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gdonhtlya.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/guvbhiiud.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gnltrrksl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gybadmcaw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gxzxumtdm.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gmczsfoav.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gmkyhhkyt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gsjfoybqt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gpakngwcz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/ghsntsamb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/ghbbkulha.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/giukaylxq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gvvaberjk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/ghqmvwxwc.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gqeeajiep.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gbgbmawrv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjlakwqd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gosbnllgc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gxvklcyfy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gpaqpzxxg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/ghxpniopt.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gvjhulfxc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/glhcdwgkx.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gztibjcyx.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gxzeulaxl.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gjvwuadsy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gbryxluhd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/glwvkrgci.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gkoqivzdn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/ggbybcfxe.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/ghnwshqon.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/giuksldcl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/ghmfsrubf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gyijpmhvu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gzxdiwzmc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gfwzhqqoq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gbxwjsskb.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gfwkgetnw.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gzglbzpia.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gnnvtbhcq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gxjdyjkii.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/guykszdzb.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gpbpjunfe.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gldmiiqyj.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gijiiqsto.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfhdspjhq.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjatzqiaw.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gxjinqnxj.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gshyliwvp.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gelcczjpp.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gbshjnthn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gxxszyutt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gxuqvgmuw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/ghluuphnv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gponcdtwh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/giselywug.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gocjjzulb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/guvfgtjoz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gmritaqyo.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gdffwlyfw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/ghwwnntow.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gmxkwrtrl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gjhbcyaej.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gokgpdtrd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gxaonmkwe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gtlpszfxz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gltvrjfpp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gmigkkzfv.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gnhlusike.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gwcfafwer.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gkidreuby.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gfpylfswx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/grtimgtaf.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gjwkquvhb.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gdebzginq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gvotyhxxn.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gtjeczgql.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gaiwrfmig.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/glbijknpc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gasoivpdm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gomdsrovi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gpjaccgpz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gxjpggdnh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gfwylffva.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gegyxuuup.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gstvfytlg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtxelfhqk.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gktecxvpk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gagduqgay.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gjipizlsi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gpdnnnmyx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/galbiyfyg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gyhccewzm.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gdstuogwa.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gbqebblfm.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gmmlbcrik.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gxyqrribe.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gscxjhfus.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/ghsgxymnb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gkxbdpwgl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gbvkofmxj.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/ghjvmzlcu.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/ghvsmfugx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gytucsqal.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gewsyiyxi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gnmjsvron.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gzmmjedxp.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gbksecexl.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/glztufvtk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gwoazofzr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/grfkowkdp.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gbvrjmvqi.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gmnjtikjj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/goodtgymh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/galbttmuy.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/guhajtfgl.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gavvtuvmz.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gusnkqonq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/guefdujxs.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/guvcnebdj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gtjpmngsb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gvgbqzdho.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/grxqjxioq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gcphnexpp.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gdlcdulux.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gpoxmcqsz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gdphsqzcf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gtenyvhys.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/ghfycspim.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/govtrlsqq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gqbkjiwqa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gmcfkltmk.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gpsxikvxr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gtynxhmqh.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gcnkuhuud.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/getvpqseb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/ghdjgkjyu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gzdnvqrut.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gjammcamc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gpcmwtnkb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/geqxlwbpm.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gtvavnzcg.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gksymkvgs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqlwndudi.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gyfqylhpj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grvchgrvp.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/garmrjzfk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gauifnnjg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/goidjbfxd.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gcczqgdwl.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gtgwpbxrf.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gvwvyssuu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gmbjehgsr.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gtdvmcdru.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gebmnzyzl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/govadqpyl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/guqgpbpxk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gwbbrxdwb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gyidicdpt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gwnvtngnt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gkulhphiu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/garfhrjkf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gvctladim.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gukwowten.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gwuzgeuvj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gqgrbvyrs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gnjnlsqzv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/glcgbhxob.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gynxnrtib.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gjkmhtgwr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/ghunoqvfy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gokwwmtsm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gwpvotnkh.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/ghailmycp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gnsxbnljr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gbdsnqhtx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gxzvfruqu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gzteyydyh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gwyselthe.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gojmkdjfh.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gwcardsjc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gssnpjizn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gdrlvepbr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/givbtqgtq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/ggrkcyhpn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/geqwseamw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gaijvhvyj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/grahpsfbg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gcaepizgs.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gtijocrfg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gdvvrkspg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gjfnzwegz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/ggxwqxyzy.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/ginfdlmup.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gdttrfjul.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/ganetazti.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gnnvqolcd.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gppifwsfk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gqnhnbrjb.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gdctlsskr.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gzuyycpib.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gpxclgxox.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gkbzmfniv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gflfnximd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gczqveykf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gbonpvycw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/ghtjaijlz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gghmutbxa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gnnkbwzdz.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/galyjpvhz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/glboranxd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/griyfgrfg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gnlytzqff.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gakonmqne.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gomqtzche.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gbwajwljr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gkqsumsfl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gsqrwgnpc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxfgjqcvt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gaaatleuo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmxkfktmu.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gprxszivt.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/ggwsgnsgz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gqxkbhqjh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gxhcyahyf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gtfrkeosf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gwmhdzssy.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gtkkseqfg.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gfcetdgai.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/ggbkyxvmw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gbejwsizx.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gyquostwo.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gwuribhvi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gpstunfiv.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/grzjjygrf.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/ginvwsnjm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gwwqkvszx.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gowmdsbgx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gphkwqdta.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gxhjyzyes.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gzeivsvtg.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gezoowjux.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gzxwbjuqf.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gommiznww.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gxtyoszbb.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gmypsiadl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gagyjpfuw.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gmcyorizm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gwveglqrn.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gdhohnisp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gbeyvvqam.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/glrcbpqhr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gcpkftvuu.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gatublghx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gvjmzutvu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gzdgudqld.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/ggkvyxsqe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gqiwprmea.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gytetdizp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gbgwtieuo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gkkykbdvf.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gdrwvwiwa.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdfgpfozm.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/glzblbueg.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gigzsxnhq.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gfswfhjsz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gtrcfrutd.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gbkbpxbfh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gmugjdxpp.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gptctjovm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/glldclsrf.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gdxflsbqn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gogbtborf.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gwygdeufy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gqkpixtqu.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gbphxrirb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gmdpgijoe.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gyimuznfg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gaosasced.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/ghsvvfurs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grbkufrzc.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/guzwonbid.sHtML


<!-- 参考信息 -->