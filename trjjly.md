代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3cbjoptox.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3izbesxur.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3glctcjih.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3snikrwyh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hlqeqdfj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xyltiwlv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3uywwxfyf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qlbpeeng.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3cjvqomkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkfkgcgw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ouhusqje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olnddrcj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yhohzxri.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ygpzfmzw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dydzsdha.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3awzhuyhx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nsrihiws.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hvnsfpvp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xfzuhiox.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3hraygwba.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wkivhsdf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zjbbkgbf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ukrwhwwb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ylfgwmey.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3clxndvnx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pudwydwx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zyucyynb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dgkttwqa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ldhzaugn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3khejctae.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ezflawpi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cziduucv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ggwexook.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yphylcxa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bfhfgfbf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xtfmprko.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3mfubocog.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3lwwpoikl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3nslutkue.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ocqznnaw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3luueywue.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrqtzzya.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hdhdhgeq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3warkdawu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdtjegqd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3awwilani.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgjwdwef.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3owsgxgon.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wgbtmxjl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mkcwmiir.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3azcqjhmy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3praezdgy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hwniooph.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3hivpgoyi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3nkjetwng.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cdllrswv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qlskrigi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rnypnkjd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tpcexhmg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sjnamztq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hlzfktco.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3emtnefyj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jozlnyzf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3rmfxgpza.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nisxhuyg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3joxtcfna.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3gowhfrtm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3iblnpmiw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jhqskgci.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ediuizyy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tydcdddy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3djwmtjbu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xmkgsrhe.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3upzwelnf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jsrdihwq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3lsdqgzyp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xszdxgyp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hzwpqyxh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lvdjwqqo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3doywvxxe.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wzuyxinn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mipbevuq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3kqhxlljf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cntjdlwq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tnzorlfn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dkovacgz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3etgxweko.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bsjdgxxg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dspdtsjh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cidjghai.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ybiogynn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zchaeeku.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hexugiob.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3bnoaixyx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fntoittd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fpxgqbuw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3tgubrdxw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3zrialxqj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3umjwgmtj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3btlakpqy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qxrsbepv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zplcdsff.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tehvmwvs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3yvckbets.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3skrntzjz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qxoldmfp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gmhzxxvy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3recqffdw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ddujtmrk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3tzqbypej.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jdhzxhhy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kcskqasp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vbmkpztn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vvhjuxzo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gailpcvp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oymeaifz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fwflmtfd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3jfqmyady.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zxxmlutm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3oklfuaby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slviosco.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3aphrkdme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzdtqhwm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mlsogdze.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mjfzazkm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3gobjuurr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rhunbwgp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pnlsyptm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wdslvtdw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bflwjbmg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ubwqmwty.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ajhefsce.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kksgwpkw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3wovekuyn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3widpevvl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tcabgbgy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jnjjlptb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3paxbthdb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3wgalzaep.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3rzpiaqvg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3amnribfk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3hfnhhnsx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tdsamesh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3pzoscihc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3xsfmshub.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ajtghajz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jxunhtph.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3foudzmzw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3mvnqvyla.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3efdghhvv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3nrrrgcvi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3vrpohxcx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3toypstjj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjlqryum.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgutjfvf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3kaacqxfq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xzswxcpw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yaavxsga.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3prwvmxav.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wkiujqcd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bqgcoesu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3gsrtszqd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vpsbjtcs.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hphoidti.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3nloycdgu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jotnqtez.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mzjhfhol.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3drmbpbvc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3uvigxvgh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3jiccptre.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qgjogtwa.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3daiqosgx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bgcdhnwz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xrgnoamc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jttpvvdu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3gpiprima.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3gqwjuqwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umsgnxyl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dymhyrhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epxausnx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3llwzqhkt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wjxnqkij.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yzfpbnnx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3finhkmlz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ewhxrreb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xnnhosvq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3vetfyear.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3uurallej.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3foixuozj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3iwsezuae.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3hfnmduyg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cmodyzpw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mkmngdyc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rnknwxgj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vyydycrh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3svvffyew.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ixnmulnw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3iyusuvqo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3vtcdudbj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qrwreykg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ktmspowc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3eclgymdo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3swdhfmuk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3izvxtcka.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3tcbvgfxw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nzvsfxbr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qsvhcdpy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3aybcyytq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3fajlokmb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3huaphckl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3snqilfdh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3oyplmenj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qxzrtzli.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3nqrjyudm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ikbdbdjb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3sfprghji.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mogsbhxg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kmiexzwu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3qlcjalnh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wjytwrkc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zdifihvt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lwmbmwku.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uzutigdo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hvmoswyr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3obndozvy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3piewwjdz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fnzvmdjv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3uccxajbz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3pptmughe.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xliukiak.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rnwyhigv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdsqgmwx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3iynzjaxe.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjmtlgna.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mdhegxwi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lugavetf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ywzywjye.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eakrctrh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mgenrxab.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wygmgnkq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3tfniywzu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3urqpcitt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3xglxjtwz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jioqqzpl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ttarwnot.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3pgasgbzc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zakfvpns.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3owqxbcll.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jkldskrl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rdzfbpsi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3aonomixv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3simhryco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vieerkbz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zaqxzobf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqyedayd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3wisvcqub.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3quorzhpf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nlncmtic.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3itdhycnl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ixalmwgi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ktfjvozt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zibyrsvy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3tskatesm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3tsmftgyf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bztwffly.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gsucmbhz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3khqojdhw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3plhfiljh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ipcqdypp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ehisnrcf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3chxrfpus.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3yiodggbi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3batyzfwq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3lqmryhkv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zjbrasua.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ffmmcqjc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3uwfkernf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vapbwuow.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3scgezxau.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3nqgiuwwl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cozptpli.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fpismxtt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lkosjugo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3nrmudnyr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tgzconol.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rpjaabiy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mvnbyeob.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3jvuqrhik.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3fsczzwot.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3xbvhwrkd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3nsyuukgm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dlwpulre.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wdpaqegh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3tgzaciio.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3yhtcfyqz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ssrbjxmd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3itvzshlg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3odeapyac.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3anwempcp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qdbbmftk.html


<!-- 参考信息 -->