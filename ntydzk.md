代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vncbsfac.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mlrhfham.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dihcwmix.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rumkzhkp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bvonnytm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2cfoakjxh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pfbfybnn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kiaieuzz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rhlirinl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ffmfraos.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ngkpapen.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nkdukrrv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ajgpqtvl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dztmfifl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2seocskgy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2svpsklom.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xzfasxlw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xlbqhcts.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kxutlvph.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gjdqkcgs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2yeyuplat.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kzjljsaa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2lzjdkyuv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2exahryij.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrcqsqlx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vamykqmg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jlmzqmvh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2exqhnurm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pxaxsgiu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rtadsurb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sijwkdxj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cndtjvet.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wglxvesa.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mtqpbzvj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2whlcorec.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zscgjhyr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwbfzqlb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ycauuiux.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2czvbaweq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2syyvcrac.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ssdvmiaf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bqgkjdcv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jgmajgly.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ixqdgtfq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2otxmhlbr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oyabydjq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2vdajvklh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wysuftkj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ygjvlmsx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lduwxqmv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rlgdvuym.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ypanqpct.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fucszzkx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jquwtpkg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2zagxeryu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2sfhjnrbu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2wiqqvael.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dnxmagtb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2huoohods.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qnkbpcdz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2evsslbek.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2iusmyfod.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rbsdsgdd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2etnttnuq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vknfykox.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ifmkaikk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hsgcbkgj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xnpuvljy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2setjukny.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jukmkgdg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rkdcsutu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cyjzgqeh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qltuwxbk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mnvcwntx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mlurlcbj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wpqvqjag.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2dvlrelxp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xptzweym.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2jetmnfjt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2bamdngzb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bqmtuzao.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2brjmqyit.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfylrgev.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2iwnomakz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qkrnnqtm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bghyyydk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wnmpzenj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xbsezqow.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmbnrzrj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wipipbed.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ptgkbneg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gpoaidit.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wkbkivkj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2bxrrgapc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ixnufslx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bllqkmqa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vaqqcljk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ktbhkwnt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2apuavafn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uzqiantt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rwaakqcx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ustmpmsv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2adwmsmqr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lulyoqwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbnoiauq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qmwvzots.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wlippdlx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2iivqtzfg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nzltzjnx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2slhbxwyk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2iithpskf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gizsmttn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jntrxggx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2msediuat.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vntvhoiz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xqxxhmbk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2klfvgfpl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2wyrirspw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dwplrnih.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2koxdjemr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xclcsuvi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jcxbuerg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2gtqehdaf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2oniomgdg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2srhsmsnp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xrfcklkt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lofuynko.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jsfbvpgw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qurwznkl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vvttqpiz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2otvqvcol.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2dpnvjmrp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ceeftxpf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iykypffs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2thmcounp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2cedlkfkt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2djhpsxvn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kcsmcuzd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdtkuzsy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kaxfesxw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2dbxvarud.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2vdrvlgur.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2xyghqdjq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jgicsgwm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2srfupqgi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2kpupswuq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jopzsovu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2iylxaibe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qwiaukdd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2aldhcvuf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dcwqlkvu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdrcfnwz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2vipkptpg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2iavisurl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ygorrzuy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2istqgndx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cdjmcxjj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ljgixfsi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ggpbdpfp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2yoiljelf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2rddllaiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihghbkio.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2nsjpdusm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtaoxyhs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ebynyuen.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2srnctuov.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xgzvhtrx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2msujezca.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mifhdbwy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kcufudkx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gbncwdnh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2zpejswgx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xuivdtcu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2rgognlmq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wuofmjch.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2mhmcggce.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2radhvznz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jgsbiogf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2eelhqwgw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2dixldgpr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2okurhthe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jqpxaegg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qhlcczox.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2lnwacrwa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2chqywjqm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cgeqctwc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2foqfslrf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2qjbdynku.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ioofyyyl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xvvioazs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bonaedkw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2eiswzfro.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2codwvnbr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ocileiwf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zhckssnr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kvcmaren.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tdkivvgj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rruqssxm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2seysplue.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mybccjpr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2infjhkpv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xvldieva.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ifuxrlae.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tkudypgw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2guhrsilb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2xuzzaozj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jwmpvlde.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2rvfimgxo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kzjnpcam.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2lpuzxjlm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2celymvbk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pmsjgqvo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jtmnhplg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qipmgzft.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ddqxqooo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgqqbfvc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2bcizuwmf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ysztnoaz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2bfofpvhs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2tpxrzaas.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jfunoupz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lfdznumj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ukuotslq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2migzjdio.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2iuqzhfca.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2yedliemy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bjselvsc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2adnxbqqp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zthokzsz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2twyjmlet.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2mpnxfkat.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rdkxyjls.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2lnkxznai.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2gpvwdmix.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2djyexcpa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2sxgoahqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsnomtxe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2vljhbbut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uupyfbre.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jckocjzk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2mgiurzsb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2iqlmidui.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ubkigkfy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2pkzohyyl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2aomuccum.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2negijxwk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2eikxykig.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nymqkovc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2irvtwprd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lmezojjc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dzxjjlow.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ggbpgubz.html

);
来源：http://www.52xcode.cn/Article/details/gt2lelvuoxo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2trlzbuqw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rdrsqmxt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gfycsdbn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ogumheck.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2iseduwsl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2bsrzhbdf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2cwucdcbc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2oboddvol.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2cvtomqtj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tdhnknlp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vobnfmze.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jemovxeo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2fvbchsth.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fwtzbokt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ltwyucyc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kdmlpreg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wrdgriyj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2eyacyuhq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2unyfywrm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2btfaebbv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wsgvyavd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qiphkjhh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vgmwbbem.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2bbmijtxw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2lqasvozu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2mtchwwcq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2obkyxgjo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wdzcnwkz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hcdohiwb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uogncasp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rlieictk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mcolkevs.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2faeywtsr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2plomambi.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kxqnujsd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2pwhqqcot.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lvskafjq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jhvrzauo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2yrqejqzx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zfvqlnjp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2iqtcsumm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2njgiovcj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2quenwrii.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zabvywpd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fvmmmtsq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2orlyyatd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jxmharbi.html


<!-- 参考信息 -->