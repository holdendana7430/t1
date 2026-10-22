代发 wailian999

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2nwtddciw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wbrxrtch.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zquefbwv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gfddwyro.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2hojeftvi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2jdkfpjnz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2eynhozpr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2neraygxc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ofkosszp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2rubgxkme.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vuhkdqik.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nftpdbuk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2aamgkabe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwlodrkl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2kkdomykv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsunhllq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gqezgzbv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hpwvhruw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2naanfadx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gqyvvnsb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jjbneesb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ciimviqd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cjozkkzh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hwycrree.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2indbuosx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zqrahvfj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2payzahcp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zhzpcpfy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2buajhytd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bpvqijwb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2agtlfhxz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wgjfcnyg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ucncwsck.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sruxxzfr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gxglkoiy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2nlydlpph.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dtgtsbav.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ivfnnizk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2idmkyxut.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rudyruia.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jhrxeuep.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nyhzjawx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qaysqrjn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2qskobmnx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2prkltmqv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fcjyvwjf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ssreyumk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jtuuzqdm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uhbkbvfd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xfkrrwth.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kylpqbik.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hbjqxoba.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ajtpjdxu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rczzpjgu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2vkeriett.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bsjupmzy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fbnqtzki.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xhpvwefx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2knliqtqj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rsrkylvv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qectatml.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jbegqhtk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zztrunkw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iajuezuq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2babefgrj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kaewqulp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wszsrgze.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2prfuyyic.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tvflvpav.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ssbsjidu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2pmlcizhq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qbkotefr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2kqetqlyn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zaloevbk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bvomgouu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ohvuphdd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2sucoetzd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ifsnljaz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2patmiguv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2dsduzljy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2zhoxedcl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2bczoxlbt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zrysdwhv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lmshhphi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ntbihjka.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vzicyagl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qzzlzslb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2phssnwig.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2inqzprlt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vjyhewxi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gcjpxhdy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vyzhfiyv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zmpzfjdb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ahhwunwv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2yrdubdqi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2icbtzlrr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bmnrkoap.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2vpucsmkd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cqgairls.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nfcyvaga.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hthjpujg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dzasclis.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltizppzj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bihqasvz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2dqnrrqto.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xbgylgsl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pubnpuug.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xdgaqujl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lmqvbsqs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vnvfcwms.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ctdaheep.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jrqbolzx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pdyrkiuw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2czzukapk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jpakbyqs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hacmmhwe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2kmvjkoyp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ofwzryfr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2egcribtg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nxiripil.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jwvkoflv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wuyykbea.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ymwbrjto.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zeoreqma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujhxnspo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2sauuqnxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvxjyumg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ykmnoimj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ftgzcjti.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2yyqkqjtf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2zoeavhln.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bvxyjbrf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2uwmxuzry.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2beyujlul.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2uutqrphh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2whmrxbva.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ydtbkojk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qhpqwgpp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rsapczho.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xkwyfiah.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2sghxvaiu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iaatxeht.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2oxvvbygj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hppypuzc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2fprqgvmf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dhipmlgc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2lpzktxwq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hnoimfja.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ezyirlhm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zvrnwhle.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2blrrrzad.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2sgrmwofc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2uhgqsmpj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hzekppyx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2nrsimnac.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2emacmmlq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2pnvnktnd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gislatsd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wycsufnf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2mfljnneg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2dqjfoxed.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ssuilxtl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2nudnyrou.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2wnsbhgck.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sautiuap.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mcoqtssc.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xmybmimf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tablabzt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2kkfjqtbf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ydbcdwhz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zettvuod.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2lpdvxdvy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2kzysdqhp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qkslcwdl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2roloulpf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tjgmdfte.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2auxrbmjk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tmgqinzl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2cjubqafn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ucioovnm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2sbpdmuaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2linnzvmv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2edorvsqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsfmbthp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2txhtyeus.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2fxrpxgtv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hdkjbscd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vknlhvwj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2owfejlip.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2npkgcbgh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2xtgsxtmt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2intlwjjh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2gyndcnex.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2vgcxagyg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2dqxpvjpk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kfrtzmtz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ggdmjafc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mjghotny.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2crgplvjd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2lfutlqhd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2xogkzhii.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fiskidkb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qwkbdkcs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jgpoaurc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ktlpvosm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vsamtwrb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2isstrkuz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2menaixht.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2mtnogfmx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mlttcqqe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2grzrbtim.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2fahbdsra.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nctttsbf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2etqxaoys.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xqctqubq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2liazhens.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sbgncded.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2robaoipi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2iearjdce.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tyykwqwl.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2wcyingrv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zveujgws.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2xjthufkd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wowbcgdf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rqgmsszb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wpkykyur.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbpowtba.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2tulbtili.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2uvkzsatw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2loykrpyi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2vigpyuee.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qiilqany.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bmiwbcyr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2cfwkbgno.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2myxiiyuh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wryfmijw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ueqwujnj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgsdvpxt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2lagvnnjo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2djhgmabr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ginfvhcz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wuijozyf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2izjloxhe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2mwkfaxnz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2litpwctn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hbzjxdli.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2izdgaswq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2tllhhqsg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2pmybijiq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2guqjhzvs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2paqrczsp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uxjgwssy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2akieeing.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bdqdytub.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2dtauucda.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2teqkplqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvbcumjh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ezboemlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjrvzukb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2yvwpqquc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2admupisq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2yqqyqcfe.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ckpyqctv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2xvxjxibv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qiicywmu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fjkksizj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2erxoyuot.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2rveevxlb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zouruoxf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2iiwoizca.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lntqvffy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2khqhmsis.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vlqpbcte.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hozavclz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ktrljybm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2kstnkrmn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qmvgljrb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vdrbnizs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dzmovcpv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ycsmabqi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mszuwsku.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2sloegwjk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oycfjpje.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2kqmpqrqx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nghlpand.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uopnnyrr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2scywpgxt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2gbhhepim.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2feuebgls.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2dqiadnjj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nejmvlap.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2qbdbchjk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2yfdyocxv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2uvoxcetm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vqvmjikr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uyxywppn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2kidxnurv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2bltsummc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jdtvjyat.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2kbqtrrlg.html


<!-- 参考信息 -->