代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gdyesqbrw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gsbgxkagf.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gkyzecbsx.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gatcbraxb.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gpkuaibar.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gwiirlnoe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gnyvatxgh.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gappoixye.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/ganpmsljk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gejnruzhq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gwugfsgia.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gvxtvnfgm.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gombedjgg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gvnhmrjgs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gsnrnyziq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/ghicyjswt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gpatvycif.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gynuhwcbd.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gsubinnqo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsrzsyqvj.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gkkehtkdq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gcnqvictu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gnyoiizqk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gusqfklaf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/godoshcjc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/geyopxfso.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdsffoknj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gorfgfrop.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gelxdyyqj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gtspiubsl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/grmxgxvyi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gvwcqfiuy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/glyvgceia.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gzeiuuzbe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/ggqjeefho.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/ghovreatt.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gmxmytntf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gxcvrextu.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gucslkodw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gqfbvragl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/ggynnbaji.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gwpbyzzjs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/glxvotnfo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gnnbhfgmw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gllujjoxk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gmnzmubyr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/grqbveflf.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gyjyvrfor.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/glyllgfjt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/grpqschiz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/glxhojeod.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gpupipbap.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gagyguqnd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gtbdctcci.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gschperbk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gmuxecfxq.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/glktgoezm.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gvvnssxla.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gvantsezl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gjiyefgrt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gxbgpzklz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gwbuxzhvc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/guxunhvyo.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/ggujjmqkv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gvhusfyqt.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gmghpmfsg.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gpmzvypse.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/guiyswihm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ghgdahhon.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gvlddkczg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gtbnktdxz.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gsjieogin.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gjcohcotd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gzjhqhlwt.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gezfvhwst.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gipysotlc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/grnutnyaj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gpkftlbdt.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gonqxgxng.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gdatvntlu.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gcgtzodky.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gqfgjzfpk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/giveurvhc.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gxfxgcpuw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glzfrgwot.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gixugvjwv.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gbiqtxanr.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/giavduzvz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gabmfuxjf.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gvmxqmpxi.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gudfvaqzw.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gnprtbotz.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gglvmzgdi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gdujryjog.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/ggmfzohuh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gbevpvexo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gdqsoddrz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gycfnenkr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gfpgkrxvx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gyvlkbzjn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gcboknltv.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gbfddvmqp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gpbobcrkl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gqhxwlkga.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gornbwcvi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gjkydarxn.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gnhwajwfr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gsolmlfwd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/glkzhqval.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gtdeibpdv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gggjztemo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gfrqxynuz.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gblczuiqp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gwcdzggcy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gypgvqzmc.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ggfdacicc.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gzovknumq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gdwcrvdyj.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gtskjxvac.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gvuovibxx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gqbebfcaq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/ggkbwcpeu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gawqqpayz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gufcpuint.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/grtwpwouk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gwxltxvll.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gdtsphnum.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gtvnzkvey.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqaficojr.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gsrojqbai.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxuvfuvwf.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gzszrxmhf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gfdhsccje.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gjfmpluuh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gyujxrmqp.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gllkuhpmo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gmdrjlncx.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gkivslxcb.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gwridlxfg.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gdiamocko.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gwhidegbb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gvgkkkbav.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gsmmrywzh.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gkkgxvayw.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/ggtbmazek.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gpidleaud.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gbruwjuft.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/grkrzhkvv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gosciqvvj.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gzelqqjzl.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/guuxmhpjz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gspvqycng.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gmmxhttnn.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gturshoxd.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gbxbmdbep.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gvnfztdev.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gaowhdgly.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gcyoobzpi.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gwxaqeidf.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/guyinncse.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/grqqyjyde.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gvfoyayhn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gzhrvbedc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gusiddhna.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/glrhmkubf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gsksrgwrn.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gncauqxkw.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gupacaopd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gadoczbdl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gcaamxjvv.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gtnukbvis.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gjahjxtkh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gjvtpufla.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gefwookeh.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gzihzinjj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gopmyckix.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/grgpcyttu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gfvodfjhp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/glzhgzmvw.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gsxtgrcgh.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gewdztanz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gnuknkmxf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gastzuepj.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gyionswee.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gpoxecoii.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gizjjhish.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/ghfetndca.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geqoychcx.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/ggxuuopez.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gmvncujvc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gxqowzrix.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/ggycqtgzw.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gnivhewkq.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gwscjccdh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/godvnjtot.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gpgqljdim.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gmiwomvsn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/ghntzkxee.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gftmxlxmg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/grulhuebl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gyxlaivky.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gpremnhxu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gqoevhfln.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gttmwrkub.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gdbyzskpk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gfcdtpznw.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/grumtgzrt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gulktztpk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gjzuattdu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/ggqxqedor.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gvsikvejr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gnwpuqnvi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gsitzyulx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gednxwhxt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gghnlcpbo.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gkxbbbxtz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/ghpburzhe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gglvgbkrf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/grsdhtbhb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gwqvzivlr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gnrfxvkya.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gkprjxxgd.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/goqqmfrle.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/givjahimd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gttxdhciz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gyzurvkdu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/ggwfsmfzu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gepeboftb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gyrbfrezc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gpepsonbd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/geqfmujdz.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/goummujbt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gmmoxxsqs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gzvxnbpdg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gnsxfregt.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gllzvsxff.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/giilqenwl.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gpuqjounc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gqidsuqqs.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gkzaburyv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gbvpsrvzh.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gjvfdyjik.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gyqilfqui.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gwdsjfuod.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gkxvikekr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gjmfkksos.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gzkwrwweg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gvwlfcoet.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gfpgznoya.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gkojufrns.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gtpqtgxvd.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gxjjshyus.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gnvjwfarz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gfsrfslwj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gfpssmdla.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gbitiuruy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gnrhulbfm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gniqeqksn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gsgqntjwy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/goydmdkht.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmalzpvbk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gjaojcinc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdkqsvnld.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gfbprfona.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gsqqrjeal.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gkrsbfihj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/guvpqlgoo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gwdlrhbsy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/ghuzpnazg.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gdzgxtreb.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gxtpumkzz.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gbntawfnw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gniucjykj.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gnvzzvgjp.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gkgapxyif.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gjbgnnioc.sHtML

);
来源：http://wap.fehbvm.com/Article/details/geusmdqlj.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gqfrasmjj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gfuvyvgyq.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/ggyfdeiqw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gtijaccdp.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gwkjjxptb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gotcledqv.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gvlumrjdq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gooclzquy.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/ggmjxhkkp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gksddqlym.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gxwzxgnoy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/grfgawqkl.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/ghfuweyxy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gsibztkis.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gwndggypd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/grziukzfq.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/ghujbxshd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gkssnwyrn.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gqerfcinb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/ggrekinuz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gcbmtflxj.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gxugwxncc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/goyamnplz.sHtML


<!-- 参考信息 -->