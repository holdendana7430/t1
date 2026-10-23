代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rouurpjs.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ldddimtl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fgdhtpbs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xbrfscch.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gdbqhlby.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zxigzxcs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ccpnpxgy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3tbptpzok.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fwxmglon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zamxkgbj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3efjwhtio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvnbchhk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ygcfksby.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3njysxhzf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gmgmsvkw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vhsyylxu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ksnvjecl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lxqzlkto.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bmbnijdp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ysgnfgat.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vrsuvtep.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3drutbsnj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vneepsuj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3voavhony.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3aulkcbvz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kjvixrej.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fdhdautn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cvfvavwu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wznnxxfv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3opiikyht.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3mrmkflyh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3jykzgeuw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dosqiprs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lqrcuckn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zcgxjcoo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3drjkvvxc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3syysvgyq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3puxsxayo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tnvpsstl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3duaqqjun.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dbrteglc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofhjdrjr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tvqlimll.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dpkbyhlm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fjlkirlr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3rxbqrvih.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ynchajzo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pumsfrbj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3mesmsblu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vinjcjwu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kqtzmqvz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ueclimyb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kvdyegvz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3razyolym.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3cpbhohqq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mfocwafh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjjiwbgc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pmfctmnh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qatqulnz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3opvbmvdj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ntnleinm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mtsspzit.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qynevjlu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3momrihdq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jqeuajei.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ohzibnsy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tklznshq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cqpyulxb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jqdfnuxm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3uqoyfeib.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3pscwopcv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cyliwoyl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tpjxsnlu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3rzevpivz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3kgssuoxb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3uulsprmx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xddwnapv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3erqbivnd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zpousivc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aaimrnhm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eivzltko.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dqzttluj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3eketnxno.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sneqlehd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xifcrdzm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fzitiokh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rsvlycfz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ggykbrmx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vgbdvqyf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xhezddnd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3jxhhrmho.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kefcozoy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3eijkcrue.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3pbnqqsbk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3uemztlpk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3iqffadzl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ypzcwcik.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3olardeac.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddbtuxsw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3dsnkqtau.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3abraokgd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jfsjlgwm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uhluzcyp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ulzidecr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hfgzyxfr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bfwwjryz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fxmzftpi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3omubicgj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3aohubbgo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3oanhqkcy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gphkbzev.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jedfqtqp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3unobfgjn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dxfbepur.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tymxwpen.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ldaulzcy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3yqmfeimo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3aqzaxiis.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gyjqxeld.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cxbrazir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhcvxqcx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3czwdxlbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwatlwym.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3raxfaclb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mocwmarb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3udxkyuqa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3yplgabes.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ipecyiry.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xnycaxei.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3kezezqdo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rnbrocki.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qxdyhmkx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3akcrgenc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3nykddqrn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ayvordjp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3nmiuggir.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rpxmtzxb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3mqndzxmi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lxelbxgf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3exvqyiag.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ozafcerf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3kqivgrqz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rohqrgev.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vusotuhf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qsexfpnj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bjccfqmy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hupwaysq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3newuyjcp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fkcetmkd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmfgpmaj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3oosbjxhu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3svhnxzbl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qqxhpsng.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hoihuhhh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ghgwktnb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wkyazyls.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3znrtxikx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vvlkjrap.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zarxaxwg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mijbrhef.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bodcznyz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hotekkkq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nlkkrvqc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mpfxeipa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lsunwpqx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3aagocnxe.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3duriqdyw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tlwywgly.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hkrwvdjy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fvbjosmo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3fvzejalg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tnyxpapu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3iljhejyq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qxysxldm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rrihfbkb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ztjeedmf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3wxnlupvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htykwfku.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3wvrkcmeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybsyzrkl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3uvfhtvwd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3kcxjsbqy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hidajrtu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mbihakmv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ixfvuwnr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zqpvpcep.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pjovxiar.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jftcnmkn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ijvsllhq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3hdcndhas.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3hsnmljmn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rbfjhefy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3rxqayptf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3awaqjufi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hojrqlnv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3efhrecuv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3diiqutnh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3govcqprk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vsaevllb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3wgucymay.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3kiryjvcn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3avnlbnvv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3frmpwadl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wrpuzcez.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3infihlsh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3acbmjewq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mylyttmt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3drkjbmbe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3houmylhd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oeqdwurv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jsnzjrvg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3weljfoqd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xpdxjkxy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3tnmntdoy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3yahukrbx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3npvbwtig.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xmohhtlj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3uuigqnap.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3yalzrnwu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3slhiaggo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uydzdduk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bceygklt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jxtscrxd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3oerwdxvg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3odloxjmj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wltyoqyd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3lekshzys.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3velpekzi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3uodmxydv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3yraafuag.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3essbrhgw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjvljzrs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tiuzwujp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdnbnezc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3yuxvchqe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3rssqghaz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qmbuqjou.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mvbmjcwf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dnomgwsb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3grggefrq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3awgykjfx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3zqdvdglr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3irrmpvwu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3omqejzyz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pyyslfrr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ttzpaxso.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wloaxhcf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qvcfjyok.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3yhmuivjf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ojttpxsl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3iffwyiyo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3qqacjqyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3klpsrijp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3mhgkldhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkdxctsa.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3oaihxkzm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fjnrueyv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jssnmvgz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fexvxisw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3catjqtfj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3rprvjxrz.html

);
来源：http://www.52xcode.cn/Article/details/gt3vwvdiqod.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3rpvagsks.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3kofdhkks.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cnpmkalw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dgpoggxe.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3wplmnarg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ymirjbso.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vxlkscfe.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3yzkmtwws.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cntfsbdd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3dutobibq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pzghmvxj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3poejylwm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bfkdfbak.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3upnzlnmx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3dswgqcqp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gvnewisc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wtthuveo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xmmsvvdh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lidkczgd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3xjxkmkob.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3usdeiawu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xmosunio.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3whgqhdgy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kulodawm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ecqeyfyu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3trccgcoj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3pjgrcedb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3etdlroug.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kezaylea.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ssqeujgn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3svadymto.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3uqajitbh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3uqdhybro.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3krzfqwzb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qqbqucon.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3dsvrtjib.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aaidlcwb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cyfgegmh.html


<!-- 参考信息 -->