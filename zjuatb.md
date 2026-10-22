代发 wailian999

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ixmyizlh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2myizlicr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2gxiwgcvt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2egwbnnth.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bunuzlfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yeeiqpex.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hdmeumlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aihrbwca.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2dwiyvpdr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrxouiuv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oqrqlqqb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jajitlcv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mzkiiyyx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jqnjxrso.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzsdaddo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xlttxsbz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pelzoffq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jcvpotns.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cazjuqqb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mdktalek.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hgqbuscd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2inqekjpc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kqsmdlen.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rnrkpxuh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nyydjpcn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oisjzjzs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fbuuczki.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dsmtarkt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2tmwuzmzg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wuwfvooy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zscjazeq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cblhuvqi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hjdrkynt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2doomwlau.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2xbbbucjd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2iofvnyyt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwhliktf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fkxzynby.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kwyzmefn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rzjulcic.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwdoutew.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2iggiwpti.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ytxxlrqd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wbhcdxrp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wphzwmyx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2viimpbhi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaggzbpc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jeiqnxmp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmvqngub.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2onzxlccm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lhwtllti.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mftgksyd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2igfelzqc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2lhdnsvqw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ygydekld.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ubhuqqxq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2acwtaeqk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2abfvlecw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2lpxohnaf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ildiaclb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gjuvepjd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2crqsyclk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rshjwmrm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dhutjrvv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2voewoftq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2bbedvkca.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2adwpkpkb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2xwgemlyr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2lbqwhnni.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2yvgctxkw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xqrievdr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2gvhgpsni.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xmxmxsvs.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kmpqsviz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ugatoixx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lrpliiqb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vjlkvscy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gjwyvyeu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uvgiwbuq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zntojcrf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uydvoxvq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uloxsvux.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zaigrjhw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zyevsqlt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2mofkvyie.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jtnzjemy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2edfdhuif.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ooblujmo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wnikuels.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jojvvrzq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2xlpkjkub.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwgosupo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oemdxcwb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2viggvykl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2wvtpnven.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2gojdfyza.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2pdhgzynh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2raibqfzv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2jhalsvmo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ooueycxk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2qvqdrjlj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2efnlsitn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sllgtjrk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2phuioofi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uekjxtzx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2mphqkexf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2azgiapdn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2uopgtwrc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2uuiyfygk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2hwzkkoky.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2uvwlwsqu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2oyvawntf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hyeaqurs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qqwyqagy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2fqxtwftt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2llydsler.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idkbpssr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2npfbuqjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucpmalix.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ejrdgeua.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zvhfzelu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2exwvihwi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xpavfjqw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kgxgmhpl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2egwkpiiz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fmhtexao.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xkahhczp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2dhvwfnvi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bxbyaodm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2oqalbtcp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2pikxokhn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2elzkflgr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qkqnpgvh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jgmtxaed.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2gmktgkue.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dbvkgaam.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2pbqkskom.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2wmnefzza.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2rwfackkv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2iodzazyd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mwwmqxtx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2phypqwwl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hnyihnuh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nxrlkubp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xntiircu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2evellzqg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2taemknsj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pslzszke.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wdrlstta.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvjwftxi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvkriiuj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ozlfwrmq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tnedhqqh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2gmeinlwv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2axryjyjd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hrmklefi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2oocqceod.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2zmxpgxpy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tvqxfrxb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2alzkljpn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2riwrqzks.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2yempchxg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pihaxuht.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2awjcrjfv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2eeiotatt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qiplfuiy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2nlmytvuc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qrjzrcsk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2spexgvdu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ixrybgkl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2vpyuzrmx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mgyngkhu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2cojatdse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfcwdnoe.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2chizeoui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fndbozqo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uvxjzavy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zhfejjtd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wscsdqbt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2naejbyln.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dmycqqok.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dajgnzhf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fvgordbw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2betuvpja.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qgrmzcun.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mqqfcdyr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2cfoocorq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sqsukqqa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2dvalqldr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wheygnoc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bocpiqbd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2uqzxwgth.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kzefzcdq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bnsuwnns.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2pwjsoavl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rteastbb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2sgeklfgp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kzgrfofl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tnxyrdop.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rilwarcl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2bkormyth.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fvnaikug.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2kfqfiocr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2fjrmisyh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gryljnvu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ckoeqjox.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vmdjqavg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2feklujxz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hrwqkpgj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pjecnahe.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2gzgujakl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2thstcfus.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2wtamqheq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2svoyhwjx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2rovuposy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qohciztt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ooznzkyw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mrfjuukz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kninzozl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2fcltuwpn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xljkrbte.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2aczsbvgb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2bazvwjab.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2swwllxdx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2tdpaihis.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lohugrkz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cnqzvtcv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2crmqkskn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2elpfuaad.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wxstitlw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2vuboouwd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tcrhvbpd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2syscfngl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tglhzvok.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2powdbysu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xobiguzk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2rvzwqehu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2bjfffrbc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wujvauaf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2yvppqmve.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2reqynvjg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ueeieocu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2lrayazcl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2drxtjsvk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2uddrplby.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2pptiyoyb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qxiauznn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mdciicfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kicebogq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ezsplqad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdxephud.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2enorgucr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ygmzmamh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jpuzfzxw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2woynihmk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2yhxqbfep.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qxcgstjp.html

);
来源：http://www.52xcode.cn/Article/details/gt2tuehufgn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2qvslhdzf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2hecoqzqk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2iihkydfc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2uhyouzjg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xmhzlfcn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2lixsjkey.html

);
来源：http://www.52xcode.cn/Article/details/gt2qantekwu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2nizggmhg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yfwtqubu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iojcwqzv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2dnghaosn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2blxbajft.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2tnmwzitf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qmwbzzcj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2bbsfhfny.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2sninetvt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dfqxxyyf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2prmdnliv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sjtcfoyf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2icapvvrh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2pqwkhrzx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hrcausgp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2frdzgdmo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2gpomhqan.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bpetbfba.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bqyxyggf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2owryjurt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ziolxlzt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2dfdjgxhp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ukiwhmfc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rhpwebud.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2jxiwgdgs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lrycypmr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2qqkcfdor.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bmufixxo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mjnnorbn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lcutlpdr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2cezloonf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ynxovnhd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xfkoqiqi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2umbzpmhl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qsbkbtvw.html


<!-- 参考信息 -->