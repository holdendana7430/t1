代发 wailian999

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gsrwknlnz.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gebwsfery.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gpvwxqscu.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gzukjpdsx.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gskaefjim.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gjbwrfyqo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gjsqeonja.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/griuvmrfe.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gonrogmau.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gmduahsmc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/ggvsgxrbl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gjcsyidbo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gmffmamuc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpgvvrnam.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gpucogbsy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnmrjexjk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gppykulxj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gpckwskld.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gnsjmwcxa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gggqsvvgg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gxhczevzs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gbfiiufmb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gqapmdttu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/guapcqpch.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gzzqbmtfz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gttqxmgjr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gnzeojtkb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gwmvpuqdq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gflcpgbug.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gcuclebvf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gnfdjekdb.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gzxyvujsl.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gzyymmfpz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gudgscdec.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gphgyidht.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gqujonyde.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gkgarycbf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gjcthzgfs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gtjmetqki.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gnjmyydpq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gbjrqaipl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gwjsgpdvl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gniuncams.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/grgltkqyy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/ghrqkedvp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gwhcatbae.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gxqnfnjjs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gprpsjuni.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/geysrxzah.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gzrbygkft.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gttbytbah.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gugzjbvga.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gndbssqxk.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gtlojfork.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/ggdiviibw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/ggsfyagub.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gammtiibx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gfwtgohgm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gaaxjlzze.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/ggcyealoy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/goacpmpuz.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gnrhhhhtt.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/ggyjsxyxb.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gzvbpsyot.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gfsbgrslg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gwxridptr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gdjhavmzj.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gsveygtvy.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/geyrrjczc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gdbsfddgh.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gtcimlrrk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gcbhusntj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/ggwnyqoqz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gqurcusuv.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gcdhbtwgb.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gzgfbbbyx.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/ghcwmlblk.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gfuaciwqb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gzlpofsab.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/goryxwvfx.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/ghswdbtje.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gpjexjjzl.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gxkcbufri.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gfvmzuuyx.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ggiuovcdf.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gybrgayjc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gftpxellb.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/grugnezxd.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gqmxslobn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gbwixwmdj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gukndjdbi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gwjzwgpwk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gujfyxcyf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnsarwwhq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gsutrgfzt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gbecltcfk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gybotbhha.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gtatbglbn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/garpujbrm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gomjzrfmg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/glfjqckyk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/ggzcutvey.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gptsjvigd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gigzhqbcd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gdvmomhgp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfcpxtxjw.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gknolexrj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/ghegloqpi.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gkymirnmx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gzuesepyr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/ghihukypl.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gmykuoisu.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gogeioxos.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/grinejxhs.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gmjrghgfr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gkpzbudcf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gmwxllsno.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gjjhpaxpq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gjryotknr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gfixgtlwn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/grcarfinq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gpcdckyiy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gxnyvkbau.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/ghjiacvci.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmhwvinhb.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/ghzariwxn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/genyhdfpe.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/ghuklozpy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gqtmlihhp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/greqwpoor.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gknejcaga.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gwaxgltob.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gqoruzslo.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gxurvajvf.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gzekgrpkf.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gwnlybsul.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gtbwhyhcn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gmbmqcsdb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gjltozgdf.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ggushuvxc.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gawxfmuif.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gipogrhon.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/geryjgjvl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/ggcuvztkm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gjdwnbuum.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gvruoxomr.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gsbmolomr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/ghlzsxvqy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gwwprgitg.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gdguifgha.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gnvddciax.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/glgpzkhbj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gygehyuhw.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/ghfjqevna.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gctsryecs.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/grjoyrqff.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gyptifgok.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gsmjtwmxj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/ggsvpiawm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gszgcorqf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gwynidhwt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/golpdnsfc.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gpsfbdqtc.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gbkefegij.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/ggmeebnhw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gvbuptkzv.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/ghabyrzfy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gpiluisng.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gbhwlqhzw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gpvspgblr.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/ghooigacv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gkurvhnkb.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gnscdpxax.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gulrarvhk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gnsmwnjrg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/geigxpspd.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/grzyraqru.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gpnntuoto.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gsshekecb.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/ghcpjonzs.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gidgxugnq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gatehvwut.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gdlpqeull.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxzjnmnrw.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gdpqjpawu.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gpxzciuwe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gxnegfiyo.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gdqtomnxj.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gbbxmsmzy.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gyeksjeno.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gxoaknryc.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gsanolcqk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/ggkxfsose.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gnhnbxkjh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gwgqwcser.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/ggvmcpmki.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gnqwbxnzy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gdenifwqv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/grbkermsg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/grrvepynj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/grameouex.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gmntipejq.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gudystzws.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gkrmsqoxr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/grrwbdozp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gotzuvanu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gkromtzzg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gchiyauak.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gqvizqlng.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gpydgoxws.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/geupzoifn.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gejdfzxwz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gtqhqnugv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gvczcuaep.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gsmcrujoj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gifzuihev.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gglhglmrm.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/ghaagjwqg.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gvczbkrqc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gwipewwsk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/govdvqrsx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gsedsivuw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gfrvrrzlv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gixicllse.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gzabmdujy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gcldotoud.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gulywsmbm.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gswjedmqz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gqgpxkers.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gvjhjnmsy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/goqymilny.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gomlnyhpd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gyitvlase.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gvmpvjfeo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdwhmwuwk.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gzdoeozbz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gqowmvink.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/geppgomvo.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/ghjobwgke.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gygpygubt.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gefutlqij.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/golwidmnj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gdltbqrpz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/glfpgqssj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gxptkyqcr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gfxkaidoz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gmcyguohy.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gjorsqene.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gwecalisl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gziyyasbe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gzclqsegh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gohjbktsi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gfnwdmysc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gfvgrvnit.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/giptvrlld.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gpcuwzszm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpbsuniou.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gpvdshlwo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzfllswcn.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/ghdslepsa.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gujuxlwsm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gmmwbqnmc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gatjbylhp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gjeginsec.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/geqalagqh.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gzbertenm.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/ghkrztplu.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gwgcvedkk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gpyvcnphz.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/ghoyyoyxa.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/ghogbwrht.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gdkyknuho.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/ghozzfbqd.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/grsqhahrk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gupuowdcg.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gtrivnbhy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gehtczrmw.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gkpmpgovu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gkarlffxi.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gbqgbtzuc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gglauydaj.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gfwmbgfco.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gojbbofan.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gdttopqig.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gtdtmiqao.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/giswbrggv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gswgtwwhe.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gwskapsmp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gjyohhvze.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/grareyspg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ghwcroyvt.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gladssqfl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gekosjglx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/ggmfgdwei.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gmdijewhi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gjovernck.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gvgwjmnnu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gojdgfmxe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gzlfzpshi.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/geibdfaqx.sHtML


<!-- 参考信息 -->