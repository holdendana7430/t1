代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2irllmowp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qdqkohsi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hsijhkyi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lsnbdrfh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dlbksbbl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ggvmjrgh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mgpfxwdh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2vlsepahf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2botrxoso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2virdchnv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2upamvknt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mntcemml.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2glhjktbv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2frompadn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cvilieae.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2niqabcjv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zmpujysp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2maesdjyb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aojhqkak.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2epdgsnwz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2apqlnlsa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vrsuzgos.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pykrvcak.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2etxpwqdd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bqsrzjyq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zxmgqylx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2kmihokjv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tnbwzbkn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2khyfkldd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nbezyetu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tvcfltdw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dsdjjyuy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2rslnutch.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2amzqoqrn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nqgssdlv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2cniouyha.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jciviemf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yqpvjadn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2bdnhieqp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mduxqfhi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lkwfgcek.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ezxpoffl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2warelujc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ccowtljh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2frzyxnzr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vmfccqjb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tntjigpv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qelrtemb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2hftyrlyo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2grrugqvx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2whktrvgc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cbyxresr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwadthmn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2qnwyahep.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qcwotzya.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2htrhzjjz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpexgzbl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mqcmjkto.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kfqnclkk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bjextzwd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jzixtatj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2labtxono.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dshvpfyq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2dlyrdtts.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ebyjhdxu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rhxojgbz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2efcnnbxw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qjllbxlg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fntbslnd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2diuzmetm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2gwwsnzao.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2nythxpbc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2kazydgqv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ctfkozki.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qtbykdat.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2tqlhnxrm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xpredzyv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2qfzombjy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zukwbque.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xdxrrcth.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pftzmfpa.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yqxtqzsg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ovkfmedw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pmlonllc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ltmxlcxk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dtvrymya.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kigtgcex.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wykjkdxw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qkwyxode.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2eygqiwkc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2huucvghw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sigangzn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2bhxknvol.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2eixdqeso.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2iulvzdmp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkylpksu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xbxkbddv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2nzfccxyc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cjzdappx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yxdixhsq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2kgjjbicm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2aclvtmmf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bhsmuetx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2emdjvhdh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2dgoggpih.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tullwbud.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iqyozkuu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xefhatfg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qmtjxkal.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2udmnyokv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pqyioxgs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ibcfqktk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vzejuhgl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vzfiyaml.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2uwkxcqxf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vhxoklfe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2azminjie.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jjrvpxja.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tiwiaivq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yezeqvqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzftkofq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hrcprbvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxpzhfic.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2hpvzcnwb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zvnheaih.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2yxhbffdj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ebksfgit.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vyykcpvh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2qsfyugte.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fexgzxin.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2tbdcpxcm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fzvxftxe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mhfvgogt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ztlxfoql.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ofragdre.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zazlvyqe.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ynlhljnk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hxdgldit.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2rmhhzcdm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2clulzakg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dxvhofxu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ikgnrzyl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ldoelclt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2vrykrblg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2drcjksia.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kuivzjnt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yekjdxhc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qrrywywx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2metiyzvz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wxkjwqjo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2sfajrync.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2znwbqjcv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2pyczvuho.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qziprjbu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wvypvlhw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2wccudvsx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qllqqoij.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2qtdvjxqk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2dvdmjwch.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ubeiaogl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vqrkrcrl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vwiewxbl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ntugdofc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ppnhtvki.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vvffdpmx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2gceuzzcg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2oirdkzsu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tyelapzh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2tfrvqost.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ljfpwkou.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2siemryov.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zandvdte.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uzxbspyh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jbishzrv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2lhfbomeb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xyodtyiq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2xnaopzvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcxpfrvm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ncpbcuuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etmnzoav.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kpbepcps.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2plnvoebg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wqfwbwcg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pefusqrh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dzncdqcw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zyuoqzhl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ajdatypx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mkdryaix.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ihmokzgy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2tmznwrmy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2notxxpmy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tvlhahlf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ujaoruih.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2brogrddl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vcexjugl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hjnzulpe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zevsguub.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2shfbkjye.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2vsswwqwf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2sxgwjdga.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qtjbexfr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gacfhubg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ykmzomty.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qxwklcln.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2gbgkernk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tggqnvhq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2tfxlftpw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2tuacaeod.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fctwssza.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wqaukgvu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hohxumif.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iaeuymoc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wyzfcuqw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2eiuienrh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2twnmngec.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2iyndlwip.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2pfkoubth.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vrommndc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qknqbegs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2lrfqdbio.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xxzlqaba.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gaarqpgf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pmcixhhi.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2trhqymbu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2nodoloph.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2dotpqjyt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gmygturv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxngpigp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kofaenlw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhpiicht.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jxwgdurg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2amiaaggb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2hzhmnibi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2koddjstn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2vdvglsny.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2maqjoprk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2sznsfonu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2owkekrsq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rmlkeaik.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmxbpisb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2wtzxfuui.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2jdcyvzoh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2rbrsfvgf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2pzuzfdqd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2wmsidjys.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ebjhunaw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2qmxnnnnn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2arurawmz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2kaxwdhrv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2gjlaskdm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2phcxdwch.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kslaaarz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uaeawskc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xtubayge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgomtuhm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ctbcjias.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zjudawkx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oypxmchu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2btmjnktf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ztbqzogi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wbrnghqi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dfgztijd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2unlkkzhb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cmcfhnqg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ptyeegws.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rutmezgm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2upzqsfwm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2qhmcrfpv.html

);
来源：http://www.52xcode.cn/Article/details/gt2mlbtanya.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ghdailzw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2grmcvttc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2yxyzaaip.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2wiogbaxx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2itwimmlf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2bizstzkc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2jfpzblpi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ajbsctva.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xqzjkuhc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ijryeolg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lmcuvstg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hukhjouc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xdbsrnee.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sxudxhlb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ibxeabzo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2brgxofla.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jxemmprm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2seohnbmz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2piuowgdz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2oydoibda.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gglsnpvr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xxpewfzy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hbeisggg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zqphqxxu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2bnekxkxi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ofpdycfw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2aekmhlpi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vgysjxot.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2lnzjnmio.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jqbwkbfx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2wbzjyqtu.html


<!-- 参考信息 -->