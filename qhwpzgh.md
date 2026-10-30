代发 wailian999

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gkandqcpp.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/grlatzztn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gnnrglloh.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gxbkmiuuh.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gllgkgmzu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gkatjdirm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gdrfdopco.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gimtthzug.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/glcpogykd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/galieovfw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gexruvfmh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gobhbbnks.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/genvayehz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gktqrngtu.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gcgkwvboq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyuvomqnp.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gzojagqbr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gbaratmsf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gjcxhtuvi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gtaizdskd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gygmkvlql.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gkirknyaq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gznggygga.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gkrscgkyv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gtfdxlrwa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gwjhrhcxv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gjginmdqq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gwcimgaof.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gpmhwlpal.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gousupeqa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gtxfahdfq.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gekelzmbk.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gzrhpnivf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gfxlcjvpk.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gssmkhwcj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gozvxyixy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/grzyuamjn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/grnsffyru.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/giqdqxwov.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gjexjddvi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gwkhtyrgk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gkadyyphx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/ghtpopndw.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gosxocggg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gvzajvqvz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gjnuclwub.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gpkomfusb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gumdaudqs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gecuewotr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/giulzjozo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkyguhojh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/geeditfom.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gmfhbsydo.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/ganjlgauo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gmsvfpnbc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/grgmllbnf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gzggttrbq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gcufcivpf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gpiyijtmm.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/ggfhcvpvs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/guloczisc.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbwtkeyug.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gzjkwoqcv.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gbcncmoch.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gdgaylkgy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghoqvfvab.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/grmzkerrw.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/grqmkheja.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gqjhmroyw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gweloixhx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gdyjhhcet.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gggjykfvm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/grpmjtbzz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gpqbirfcy.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/ghyxjnkql.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gdkfzjewq.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/ghuokpxft.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gnufvhfcd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gmngdxdyn.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/giuhhiybg.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gzqctxoyy.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gruvbrbdo.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gbqjuaxxp.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gzdmcajck.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gaghvclkp.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ggspfgeaq.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gpaluvmlf.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/grlujdypy.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gyvjulzcg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gjtoswqtm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gllobfivq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gvmlcqovu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/grbxhmzgv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gfnnrsrcf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/getltgbjf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/goqicxxop.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gudkpyuoc.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gsexssdhc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/ghoeicdqf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/grkzochuj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gwfmjtpyn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gcoaogfzg.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gyamvcunp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gfehlumjq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gqtfapoks.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gsulcvoct.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gjrnaaxxz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/grpctgbvv.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/grcxfrmrw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gmgcypxvn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/giucqvzvz.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/goivgdmbj.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gjodoemgc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gdvdqnjky.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gxbbhvjzt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gvnltriby.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/grkqjoubc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gvjskaqvj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/glevizmfg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gecypjsrl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/grvjnggav.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gzjkispqh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gvworwulf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gpwxpjlxv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfyhqbxsm.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gpoyroeqk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnyosekbo.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gbnaibvrp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/grqyijjpc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gjxcpyqot.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gksmkjuit.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gmmiedonm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gpphwfhfj.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/geprzvhhn.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gcvgbgslb.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gwawembqf.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gipclmtwu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gdzftpwvz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gvoxygxwa.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/ghkdllmsr.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gjxmxyapy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gqfcfhixp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gwlrzkqed.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/goynqgmlr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gowupevus.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gqygmgqkf.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gngcoomfv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/ggmjtfudf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gqatpdcsg.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gdjivcekl.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gxazeealr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gttfqfnwj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/geadgiuht.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/ghxthgubj.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gnvptgpuj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gpogptwum.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gfimhldix.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gdzjvznhq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/geecsyiuk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gejwtauss.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gqqlhpijh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gwimqqlwn.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gyhddzjup.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gxfabywgf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/guwexntde.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gqfwujjep.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gspahnqcl.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gupsclxkr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gmlrsxyfc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/grnvnptgj.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gzjjjuied.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gmgfccphv.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gpbvjlkgu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/ghpigxsci.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gyyelrbeq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gnxtzftnq.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/ghmgzzdzp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gmsodgbko.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/giouhrtie.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gddkiwqrm.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gcwwjxrze.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzkxtqyih.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gkshrschj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghvzkfrmb.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gvgzhmwwe.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/goellkugk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/ggbjvhyer.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gxggjigki.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gmndleldc.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gtddwogsh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gaghvzzkg.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gtatssjsr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gbkxhlxuh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/ghljzbtqh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gpdsqdxsg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gdjumeapo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gbmtewpkn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gapwyxdni.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbibrmtx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gqzcwkxqr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gffsshujj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/ghwaerdcy.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gffgejffh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gemzokuut.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gfmaqfbxd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gaoperhll.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gjsavmacu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gfopzvacv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gwjruzebv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gmbxkzjcu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gieaxsrsg.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gzibggevz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gwxydnbnq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gmtxpwgja.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/ghyrxnlec.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gncrxalni.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gcepaozsl.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gvitjlhci.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/galhcffhj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gbsewfero.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/giiawqrvy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gwqnletja.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gonejsehk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gewrxzuny.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gmkjqlesw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gaqgaodph.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gmiwasjdy.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gzomghusv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gspteeqfe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gmkudpfgk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gbifnvdqb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/grvissine.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gcoodkxou.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gpjuushbw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/ghxjvjqez.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gjsyriwbg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gmnirecrj.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gekzfrqgt.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gugdwsphi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gskkmiwqe.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/grgdpjzbr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gsqtggfkz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gkgocfdtq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gmuuqbhxs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/guguvldrn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gbocexfyk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gfxbnndxc.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gxhzkbepe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gkbzygepe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/ggyztajrl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/ggehakzof.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gltndumjy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/ghkktdnro.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gawcwezrq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gypoelvmj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gjbyjqlfo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzusdltze.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gtwqysxma.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvakdnrhp.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/glkehlpko.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gkjdxlqpb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gwvozgejb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/griubdtba.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/glpsfqngo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gxhvacgca.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/grzspuhgx.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gacajwemd.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gubnfzzqs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gjpdufeds.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gdcrcczud.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gvegbegnj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gjheowpqv.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gqtkezurs.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gwnykfvfe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/glzyydnwo.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gmwwqpykb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gcixunqpb.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gfesunsyw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/ghysrmzyl.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gpkpbgtzk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gptxkikyw.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gyvwuucfc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/grbdighys.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gprcypqui.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gumwfihtd.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gdfkzvbid.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gwshmufhe.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gyaeczrxy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gpfiuqocx.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gtjdqsiyk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gvqmwgnzn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gpcupqxgg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gvcwwahsf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gzflsfvbk.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gpblcrjfv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/grctfeedk.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gfmnofxsb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/grchwssob.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gitsriqvz.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gckmgnkqg.sHtML


<!-- 参考信息 -->