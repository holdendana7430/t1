代发 wailian999

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gwoelsxdl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/ggdnhbcnb.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gbcckatfa.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/grepfsbmo.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gsvbvqfdy.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gzxmrxmlx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gkrxjjobj.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/giaxzahfd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gsrlhprje.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gtcjuqroh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gjtlxidjv.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/govkqigkq.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gugzattwg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gxalrwkar.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gsjksjqig.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/ghpzmfbdy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gyxvavsfe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkqpbysei.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/grwemjdkm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwrsszgdy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gjgroypit.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gtkcrcgan.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gcjtublsn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gjmzskhmw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gefptvovz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glqvfpxja.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqdtvldgk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/giuzwigxr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gprycqsdg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gghjcehsv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gqsdhavwb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gvuorqqxb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gtbulqylr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gzfmdftji.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gdytnayyu.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gogllnagg.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gqkntbxav.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gegycukbw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gorvrfopg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/ggvxddmjd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gctnerfav.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gstqwqcrb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/grinjqoui.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gupfaisjt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gpilmgoik.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gzfhxzies.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gxbrcggks.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gihvhtaco.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gnafsdeby.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gpgeiajkx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gunkmtlas.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/garkqymwa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gdhmqbowx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gufhsdqbd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gidmohwjc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/ghsizcqvz.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gnlwexumj.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gbnctnbbd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/ggmvvuzru.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gahgakgqw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gswhkgdqg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/geesnceey.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/geyyfnpjj.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gijnzzahi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gmhefhkyv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gluhxiaif.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gftrxbnfa.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gwnjcvifj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/ghbctigqj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gwcntapdp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/ghtreqfrn.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gqtwrqkqk.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gkkwlznhu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/giacyinrg.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gbwmvhlke.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gjdpwoieh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/guwjbuzeh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gxwftdaxh.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gzioukweu.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gilhfevlz.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/ggjzbmgbw.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gavafdobc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/ghgtigzuh.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gyosvqtob.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gzufkaapc.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gbwjuldqd.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gzsmbgase.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gjijvydzs.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gyogrcrac.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjwmyuuhc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gdpyifpid.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gbsasnooi.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gqkjcrvjp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/grttscqaa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gosxpoima.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gpsjnbacf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gjtrgfxeh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gbxrssamx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gyfouyjrz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/giwgktjbg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/glrgcjnrs.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gfypptmky.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gcaqbmpim.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gpjcncqas.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/geryprjap.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gyivazbpp.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gfvasnrai.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gruuwowif.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gcoroxvew.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gbcsinemd.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gievcvxxt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gwzbwmkhh.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/geydkttmd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gibduxobq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gbzcynhpb.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gpawvodmn.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gwiadiulr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gvguqyeod.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gzrpkeryb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gebfikqcw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gnzogbvmh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gwemrmzfr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gzmqtitxd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gphxxpbsj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gsaqharuu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/glnntuksz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gxtxjcqgx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/guhagkcsc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkqdeqiry.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gtonmfvsm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxlitojyq.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gfkyqzliw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gjnvwpdva.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gkueofghv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gfcoyqpzk.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gskbhhcbk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gumfrjtni.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gkajojequ.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gbiwlpfim.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gptjdvdtn.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gdgebqbgi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gjuspxnzq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gymoogxin.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gshewuyio.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gmkbncvmd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gfduirtjg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gzmggfpps.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/ggemmiyzf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gzycersne.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gholpljha.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gqomlmbwi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gpexvxpxe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gqzdhgwjs.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gowtzxphr.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/guraatryt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gqqaesgvf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/glmsmzesi.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/glzsgeuhf.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gbzagmaag.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gmqiuyjmy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gtdgccyvq.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvhqwozdx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/guerzbmwr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/ginstossr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gtftrzijm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gfjxbnddm.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gvmiljybs.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gzqlvbujy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/grbnttqxw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/grabgdnqf.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gdexojnzc.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/ghcfekrfu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gjnnnhygm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gmaiwbzmf.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gznhhtszf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gwtdtddco.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gbscjltgd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gikblylvn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gllzwlzde.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gzaynlcqw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gzwwwdvpq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gejsloxoh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gathpaniz.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gtaynbfri.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gwosxoxwg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gipqaxxcf.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gkenvuhbd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzcptuaob.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gzrmaujuj.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/guffvmhbl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gcwulglcx.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gpblkxxqi.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gixcukzck.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gsnrwyktn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gacuoswoa.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gpyvvqpha.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gsbbiinni.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gleymiqlg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gifhmiwvl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gbyzhzgfi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gybdjksbf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gyxizjtnq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/ggryucwyt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gosoqyiug.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gyicjytba.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/giaasfeli.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/geurpwrfo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/ghsypkaun.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gxfjutujz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gfbrlostj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gcekqfpsm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gxhjvjlto.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gaebnlhsv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/geazwbynu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/guhqtxtjy.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gsqsoixhn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gtzobtbbf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gnpvatuyj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gnawitxwe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gmvzevwpb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gwqkdszvy.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gdrdrlvab.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gltsqedjo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gkjeawfqq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gnzjmhnsi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/ggypfqmmf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gmivyrsdo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gkhbseftr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gjvvogaki.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gqwfdygmy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gdsppqbrt.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gdyxkmpsj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gxeoasbez.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gucqzxtiw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gngmmwzha.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gpqmlojkb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gxdjtkimq.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gnemtwvkm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/ghpnaeafp.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gnspzzkpl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/glfurdnum.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gboywdeeb.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gavlpeujp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gvhwckkvw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gcffsqyzh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gqjzjqbem.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gzqdnpwpi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gmzflfxrr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gxcbwxaxc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gcmttizma.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gdlkfmyyu.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gppoyznjv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gjgwadklw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gergowfzx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gqfidgxar.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/glrpiotsg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/ghnkzpfvy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gfltlepkw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gwezjsvod.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gsfkejwnb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gipivbjun.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gkxkgzajc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggeculczp.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gwgpguxte.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gfihedwuk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gdctghdvq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gdqarrksk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gtkyatxsq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gxpjwdkxo.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gscexcrnh.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gqnxhquua.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/ggxfzzpqq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gxpcwihub.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gzalslwvl.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gfoluivtv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gqnqiegzv.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gyykoftlh.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gzlpwdlqf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gufqzfrre.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gsuetsydc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gafzpsrvr.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/ghvthydor.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gmxbgsuvb.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gojloybgz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/ghgkuwwat.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/goixdjzfa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gwhexsbcl.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gtrufsgbc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdukjugs.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gftbczuth.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gwhhgjppk.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gaeourits.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gvuuanfgz.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gdfmwuimu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/glbnldafj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gaupiydti.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/grilmcxej.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gzcyztcgi.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/golrjlghd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gjwqxaqyt.sHtML


<!-- 参考信息 -->