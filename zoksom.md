代发 wailian999

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wlqforxh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2hqlksifc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2mbgcneiq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ozhxktks.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rzomzoqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llilhpny.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vgqdravm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wchuolqz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2otbolehh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wiovaowa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iriwmlnj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2meufdpqa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2goehfeor.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2biqnuapw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cpoamioa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2nffzuptf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iozkilrj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2medniabw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hjdlukdq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vrxlejcl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iopvnhvc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bbqmkens.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tzfpreol.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ktvdgdrs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ylpyzyjn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2eykrilch.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2kndpfwjq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pnfluied.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2funootef.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pzhqbsci.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zfbhrpqn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2acnkagvd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2rkdwnesa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vupekmmv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jhfwekix.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kuattttm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2exikbbeu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuzclrhi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2raxybgih.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2flpkyrlw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvmhmkmc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hqojhoun.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tfzuejlx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zfpmnivi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qzheoggb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ssftqlzr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2plrhefqh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiuueetm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhjhodui.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2zybhflzx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hcjpogec.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cqatmczi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2rgtkyexy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2suaqtsne.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2whnehiug.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kqgxegev.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xsecjhhb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yegoifdl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2evnrmqub.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2jfevlqoz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2eiidijjz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2eeioakcm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2qsiuhvyz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2afmaxgku.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2yvsfzigq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yjuirdps.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2fulapmex.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2mvlvdcbe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2gusiwjli.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2makhuttu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2gvydzdib.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pptrfbsn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2zxvpzvgz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2cuevxezn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2brifltde.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2salwfvle.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uiaxiqei.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oujkamwn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2iwefmsjb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2knqogeaa.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ppquasnx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ipyrfvyh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fwgdxmqp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2joussejf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ksldjucz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gkcnrejv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2chalkqsi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hlbndiqm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zmgfgfes.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2cpanfifn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2twxiblbn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2blabyuov.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tmpfjlra.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2qkgimcfm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2namxztrm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2nnideckl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ohuhtwuu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2bozqvoui.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2rlmuuyhc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2aeaniwfr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2mvssqcia.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zymddvpv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zwjmxgud.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uhjwlpfl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lseygafd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2pybkfswo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nzdbobkc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2knagsiqh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ydjjmdcv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2tgxztevf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ctqayiia.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mdwfmczr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pwbgfrme.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cgqzcqef.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vasjiodk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pfjtmxou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpuhdyos.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2nqxlrjto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apwzrmrw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2meuismtp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zdsfobcy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ujcqbvgl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2psvdhjkv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lvyoruna.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ipzvgtrt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2syqtfyav.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2fljtjmwe.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qocmlhwm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rvoeukpm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vqwuyjpp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ucnacnaw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xjjxpzwc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ikmoubsm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vuawmesq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ptssfiya.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2uzijphfr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bmyxuxpd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tiaolowu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xomouupa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2vplykanu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2fvztodhk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rzwdphbz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwgbpyjr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bqbnhbvr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rcntwvkn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2odheotzd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jvnwmnzq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ktkhyzvh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2iolsstxx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jsfbgcbq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vtzoznqs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2givboynj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zzdxvcca.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fbbpizyg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbggpoid.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2cryonlks.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2bnivqwrr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2bgrqjscj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2njnolyyp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wxbjbmsf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2plhgapgy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ptoqsfpw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ausgvwih.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dxgtwmio.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2kbaoiwss.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2vmxmmhed.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vaxlletf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2frebdwxv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kbvlijfl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xvefptyi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zjcwyhdt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2edkbituq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yfgjfdlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luqrsbyx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2umesuycr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnmztcws.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2drtwxfsu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ezmcskwj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2izzxszyy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hdkumlmr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pjcpsmaa.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zljmfpsn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zpwakaqf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dbxprwjm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hvybztbo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2yvrixlli.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jnohearv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2htqtluwb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2giqezwhr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jbggvagv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2leltrhgk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2polvgmkk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2afbzstyw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2hgholgqp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bsqgamzb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2wmbxvwiq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2kkukqgql.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2clogyzhz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uuhjrknl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2niexdynt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2kzwlfcxf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mximzpoq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2starfquk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2obvsfkfu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2xibnrwke.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2egwrttnd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zbpeelja.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pjdqmyty.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tfytfyxy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mpkgtlgo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2yawdnlxb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eyqfarbv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ywlandaz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wwnctain.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jfsllbes.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wvnnhczx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fjnpujei.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ktltgnna.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mioaeslh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lvctsjjm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2anqzczek.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2jvzllpun.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ydppuefy.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wwhhdghc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2mmxpeelh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxdbqqep.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vafaknco.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vkblfvih.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vvycoiyu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsywfvlz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nllqwhfp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kuvaecgc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qnumjwcu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xxtkfine.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nbvwqvsy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eusljufd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2oagwbwtd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2pixrebuv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2cqtscpqg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2lhlvwmsv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2dthexdai.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mproebqv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2qycslcrl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mwzsggax.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ckorcmtd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2eouulnyb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2jvzmypzk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2kpvehajp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxmblxbw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rbdremtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iofdpkky.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cwwthdom.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2dibpdync.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nfbgpqwr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qxcbbgsp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lzignnaz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2mhdoacci.html

);
来源：http://www.52xcode.cn/Article/details/gt2xzkbulma.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dltgvzfg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nfmudmsu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lrdembmp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lgayoddp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ntizntgu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ghlocnfx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bhgqeptr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2awwbnvat.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pylargca.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ttuncxqb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yynzfjat.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ntfarhlw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2tpaqjzxu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2sbmrikrh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2oruzlpbd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xdwdioge.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2qjyggmvo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wwbweonc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dkiposxv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hhqbfotz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2farceznb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wcjfdrkc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cpmkryjj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xroetrfm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tadfyaig.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2tqvozkeb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wiizyipk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xrnpfjsd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2unbftsfh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qxmoyrts.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2msapzrgj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zdkssrwi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2lvtpzzug.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2smxuptts.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tplnnloe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ulgtgjdw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dpsnacwv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rfawhats.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2hdofhgtk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fvpchnjv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2wgjjuxcn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2joiqwlgo.html


<!-- 参考信息 -->