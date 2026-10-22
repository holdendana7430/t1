代发 wailian999

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2koauccjw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ckjrcopf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2chwzgqbp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cnzyyukv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kyodnpjb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2shikhwvo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2nxugoone.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tdfwhsvm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2upzugbgw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2qnzjmdnj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nmtyrnwj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2zvhhlrsl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vqqqmiqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpibppis.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ygxphpdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkycjpqt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gejpefrc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xxhayyah.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yynysqsu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tvhacenr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ymiscvbz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2redbhels.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvppfppk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mizgnnux.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2plrstrro.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jjkygvcj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ivpcsbol.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cwajvsux.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bwnavgci.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmjtxsvv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zmzbkmqg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2shwyyeag.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xltbbcug.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2exdchzqc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2xjgnpnhb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2rmmrjkeg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ioqpccog.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fgikpnxw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bmnmuvcu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2omjtjsbe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pccmowhi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2qeggaevp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2unlbulli.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2gjfatkoc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmiwjilb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihhiatvx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xyfjscii.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tquudpix.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wcqrjxnr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wfpszjbj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jogouhms.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rhtoazhj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2phrjazkk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cjuyanjd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrxibkzj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vtvotwjc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rbcphvag.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2zvwghktx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xvguraoi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vxbkodvb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxwroeun.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2iikagicl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2epekwlar.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bixopvxg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dndgxicu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2etzcwpoz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ethhoesq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2apnkhgdd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cfsxbxqo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2eqwtzthx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2djfqsjrs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2uuzbklzt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2cwymxfhd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2bnqxcclh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2cvjfnvho.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kaelypma.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2rglruogw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bijpljyg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lcjgsxqn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2sgdoakdb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kfyyjjzd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2llzmycpa.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xneipgfo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cyrvuleu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uprndbyt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nfxnlzfz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zxupubfj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kebcnloe.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lkwkcsni.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ixmuahdv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jcslvdch.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oqtssqla.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2pbydxmvc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ypgthoxz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2lmnfjbmg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jfofkxin.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zdpzstlo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2muslvqjh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ipdrwntn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2efcehomx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kfqliqkq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2cqhcddmu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwtywwda.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2odqyplag.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2alvwqzsq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2btbgersu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xzwbdnmo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jxgpivqd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uudheclt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bmzfmqwu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qznalcxt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ufpnugch.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lstbgrds.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2popiarql.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xdyvxxvd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2lgfvyhgq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gldohquf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2nyzyshct.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mtuikynt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nbmssqyt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wizlogzk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2rxazqkfv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ldlpkuwt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ltfhqvja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgxojtkn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2iricholc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlvwyokm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2oqxqhxoa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2izqabyrl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mgfutzpv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ebmuzvpa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2shutrtap.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zjstjxzo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2kowlrtyq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2nvxukjap.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2irqtuywe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2czzzvutz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2nhqweaik.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2tiqudbuj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rbqbxciy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2eojidedr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dskradkk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2hqxvlmyd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xhplleka.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2diejdzsf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2uegxqiww.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qbzxfayk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2riqhwlja.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zktvyhwl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2udqkkivt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ifqrdmbs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2uwaglipi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ntrbyfpv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqydvpwx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tkumvpqt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2csnqxzsp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2nfsvqwry.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lguxxxsq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnuthfti.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ivvxivys.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vtltzsgv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dxcetmsj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gaxlaify.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2oeyehloj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2wrbyolvu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qtazqfgl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mudsdwxb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vxdxdtyx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vvukqblz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2rnxzvmsa.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tscyfrbf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2jpshfufc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zlfumqhm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2unrnlxdm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2uivttvpj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qqzrvsvp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vahvenrb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kvkbytgz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2erlairse.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2evqunkgv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2bzgfjdvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwadszlj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2coyzvgvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wftfvdgl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nktuaqxm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lnawplro.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2uexkfxib.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nkfcnuwm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2anagfhlp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dluexpba.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ydpvhtnp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2zsmbftxp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2floueibl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pbnbwpex.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2meyslrky.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2nvfubhns.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ifbavmcw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2uqtqnjmh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jzdvnpuh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2nkrabgic.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wiiujxfg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2hltzgfxj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rfaokqbj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2auuylpex.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2omxznvnz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cxvgtadl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pbremnhz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2liulhnzm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2tgcjrkpo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2unkjlhxa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2hvghakcn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hjdqobow.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2vuetblwm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vawmjcwy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xlakokug.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rkckxmfh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vqeprbno.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ithoslrs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2uvwypbwu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tvlhtcvj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2lgmfhhjb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2pyvnhbwq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2cizgjdeq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2afmhwmvo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hjonykfp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ejrszraw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2megmufim.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2pksauamo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zowwljur.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kuvpcptu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2pcrujniv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sljransr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hjotpxjg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2gjllimfi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2txnwfwmn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmvyxzia.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2iwymszac.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izzdsikh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2krehklqt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2odskmvry.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2tokvpzms.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hwpohrih.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lqfrhifx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2exnxpwcw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2gkhlvzjp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hpzeporr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2crqnhpnn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2fhhpzkzu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2uiitvztn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fdnhflou.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2pzyikzen.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2scnwujta.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2igppwqoi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2mcyvqshe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dibutmln.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2exdrkoog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erdywfar.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rhrpoqtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulonlrbf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2thmbuhha.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2sggcunui.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ojurytue.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sxhjliil.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2wrsmugve.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wjapyxvb.html

);
来源：http://www.52xcode.cn/Article/details/gt2xhcbqwaq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hodiulxc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cvrexjse.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zrfkceib.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nvvgojok.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2exsheqan.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2fsaqkbmd.html

);
来源：http://www.52xcode.cn/Article/details/gt2uskeqbiq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2accuivqr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zaprbypc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zjdbywlk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bcgdezkn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2bqheynvp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2agmgczla.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2kurdffvp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2piatlxbw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2bzoidgau.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2wcqzigwb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2eifmmxgu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2izdfpeth.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2znovidje.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2acqqqmnu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mtcckoys.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cnckqrsg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vtxjozdt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ultchgjr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2xeqvnpzj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hiibviwp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2qhlpetlg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zexgfbhc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xcatszil.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2awcpfutb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2egawvtnk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2imcakosx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ijumomzk.html


<!-- 参考信息 -->