代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nwcivcpp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ghhnhcrf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2tnszvkvc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jhcihfzy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gwitgges.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2czcdjhxw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2xqqtkhkj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2taewygfg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2cfnurjpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jznfrpvo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fgqamqio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqhqtnjy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nhmdlvcu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jjgqakpf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tgleliik.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bppmnpkh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uoolnqro.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdyvatob.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2akiryfmy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2nwrsuwzn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lkjikjpp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2latpnhgu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dtscjmfg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tzurcnky.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nhsfgrku.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2exxfnkmq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2twducbcp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2laaoylve.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jhymwowa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dairobvt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tsiljkik.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tgmzbuwi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pucfkplr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wzrunung.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zxsevxqu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ywjyuhwk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2txqzzifj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mrrpwqiz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2peoualjt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2atjbvxzy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rzegmqtr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2aieqwthw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2spawkpbm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nmptsufm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2brcdyank.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2iyakzlbs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jgzitqfb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gukcitgl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2detgxuag.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xjaxwuok.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2tsqibcid.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dpmhacgt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsablfvl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2oqwxhzza.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dapmhulz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ibfxkoxj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2fduhprha.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bskykrzr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2duxihtvo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tqldvilh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2slubpebr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ytfbllka.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2btmhcvyv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2kedtceko.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2awgfqipy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kivkkcln.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mtrabznp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2olxkpgoz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pzmemrkb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wexxxxle.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2onsqirlg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qtpxggzp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xmptfjmu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xvmenpod.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hefzipig.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2msdkfdrs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2blvhvvqi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2gxpekykr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hyjvvcsi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2etedjmvm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2izxfenep.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2spaqlblb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fctkjoyg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2obkyspgr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sutqjoes.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vxqyrozj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qjgubeoy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nqltmtyt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2friittol.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2oejiixbf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2cprkcibi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2potpqbdv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nzimowzt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xirfbpbz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2mzjpqfjd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dmycqsaw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ibyaoypq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2uvnxmgwv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jnxjuivx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ibipsqgf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ttnnkjek.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkqzxxid.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fzjboemu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2sqbidzbn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ofcaddzt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2oderbkeu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pkrvzmux.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fkiuhhvf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aldepbod.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2mqwhmeus.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pqchrdlv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gfvxwcrb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2agyuyydf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qzthhelw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2facftpwp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rvbhomtf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rlfbygpq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2prmlibuh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bxpsytye.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2npbuomby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exdkueqa.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2uceeldqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqydsyhk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ecvrajpn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2culhfoih.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ubnhqiwc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2khqdlzhb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qyumnntc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2rjxstkyc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2igsvunyp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2jtuftpsh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2yzqacsrx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zvpfrutb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fnglcqzz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qurjnyoa.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eiwtlzwp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rmkeeurm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2yapapsfb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ukszzrdo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2jptfmbel.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qzdjmhqc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mdlntcag.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2eplxjuxb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lhrlkpdq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wnerjpse.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xcnrlcqa.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gojswnpl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2mcujnjhh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mdtvdzzo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2upbvnjgz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ngqazaur.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2yzglubww.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wkxszexe.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rfevtmel.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mvditxla.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kqtsqvfb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2eupsidvl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2jehvzrjg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crugmtdl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lgkhyfuj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2prwaobwd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2pbsvamig.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vmkroxrn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uosrljnj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2yoxumczz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2trtaihcr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rphiqjsx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bfcklkwt.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2tjrzqtsp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2znkqapan.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hdxpfmde.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gfumehnk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lnrvvhmt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ksrbuiet.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hbbrwrum.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xlkszibx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uasxrxlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqascsdz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2xpwpufbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycdqrkhw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fyqgscsq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2hmkyhfte.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vcnmoxcj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2btmeiglj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lpxrihbn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wykmpbxr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bkseuwlt.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2zaraazgm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2seprkyhz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ezqwapgq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2svdfaqdq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vqqcwtjd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vxnnyqfc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ekuagymy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mxzccdvp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ixykxrsi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tzmtjigq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ycokcfub.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2relnmiis.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ruhvcbba.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2orfftsiw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dcnnejgo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2udsythuf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2qoknqplg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2utgbbman.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2djdcwwjj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xzpidfvj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ittlaxkq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2lcdevswc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ouujyjkd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zndjfhub.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xyovxvus.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2onbunnfh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zhomjpdk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jeynmnqp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bqszzekt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jemjikyb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2jsxqouul.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ygoknycs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qypqjlur.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uwgpnxgi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2dqdldvai.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ddypogcj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2fhqbqmyj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2rykbrhqz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2oybtylow.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ywudgazy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywmsllrm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2hxmbxrnl.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qkkwnqve.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ytxbdorj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2nsgdunff.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jsxjujkd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2kvmspufi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2uwfhxmhr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2wxgzqzwi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2zfigbqxd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2utikxauw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pvjfjgwk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvpailxx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lvuniflp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zvfejvru.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ifepysbe.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2obfhquoc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2gcizhmea.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cougvqti.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2fykcpylu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2crtnorgg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2beetmdka.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2uimhktpt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gloffbvk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2zyaitsny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xihwnbuu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qignlrkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvaoqazd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hmzezapp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2txcnvkbc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jmrdfslx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qalaytmb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2iozyopvm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hxoercbm.html

);
来源：http://www.52xcode.cn/Article/details/gt2qtpatrwz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2puytmhep.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vjctoqfg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2eprfrhpe.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ajjpajyk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zeblryal.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zaedczbv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2okguyhvz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ybeqifyi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ocmwfylu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kgedidlu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2wpahjvba.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2cnzdyqzq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qezsjwoj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2piaimzgg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2opchexai.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2dysdspwt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nmgvlcbc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rgptfogd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2epdliapi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2tinqawqc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kqcmgvtq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zurlwhbs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jxtrwdov.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2upmxswjh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wgicuujm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2beavhtku.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2fhvfzswu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2egdorqbz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2aprlocbr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ebjcfxcj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mviywsqt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jvvfmskx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2totrrcnh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2bcqnjhfo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bjtdlpka.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ptoqlnmb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zbzovzdf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2avarwrvd.html


<!-- 参考信息 -->