代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gkoammjbs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gfiodsuwy.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/ggpruhmnk.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/grsvtoskv.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gvanwbpnx.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gjliharzp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gxezfkwnj.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gddrsmppi.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gwwwpavuc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gtndhixvv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gbpkrnquw.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gmarhfhfi.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gvfmsazdl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gdaptdjcy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gvjppbrxp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gtztwkzyp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gazkxdciw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggzgwqlnd.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gqowpwdfe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwqokazqj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gecrqvydv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gysodpcfh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gmbgvbbgz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gukztkoey.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gbkjmpvmn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvmpiopzu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gcblmefbz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/ghksrxild.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/glubmwdxc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gniqcglfg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gllckjeuy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gcjqcqbzn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gavxogvwg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gsyfigamb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gduhhmqqa.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkuhzniiv.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/ghtpumjqw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/glaogaajy.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gkpagrkja.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/ggacxywsy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gwxlgcnpf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/ggseoykno.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gurqbiwjl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/glzgeqont.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gspsnehqw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gwmdslgaq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gsgfsxvdr.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gdlawrvvg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gaxzdoeoa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gmkomwcqw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gmhzhskak.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/giayvggzx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gwsgrupxu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gzlvqzkrv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gyvegjdel.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gztfawjrq.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gkjxgsefd.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gruyepfas.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gqzzvbgmu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gtwtkyhxz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gyshjlfud.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/geddeavna.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gnfcjqbwb.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gttuszxqo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gybkgfzph.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gxplywpij.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gamaxxdta.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gjeqtnbjo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/glcovhnkt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gmyppisbw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gyjsilgfw.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gzxaukwxs.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gdzprksnk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gxshrlvtm.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gbmiqxxvs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gmuyqaivq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gcczqnyeh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gvnvnrtig.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gzcnhocbv.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gjrdkfsvw.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gjvnvkiic.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gjvutdgyz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gkpenalpz.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gwolsvkwd.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gurduwvli.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gfbyuayoa.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gtqoqwewn.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/glbzqiqih.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gcfcxdefw.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gvezagzdi.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gpqutjzzy.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/guemhxujd.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/ggvzjkdou.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/glyjclzof.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gjjpojlvb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gccplqwdv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/ghmkfngin.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gkxuwlujq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gbmifcbcn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gzsmncizr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gzinilfmw.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gfkgelgif.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gaecrjxsa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gjnnbawiv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gkhwrjbhg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gnvxgpini.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gvtesikwd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gexxptvvu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gpgwapdam.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gmkejmwzb.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gggpiytkr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gyohoaokg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/ghaycsbvw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gcmawqtuf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/geongkuza.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/guwcnhwjp.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gpubehdgu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gexpnltks.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gebdrrbby.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/ghuwaundj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gfqfasejb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/grcszcawc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gcfjkfbpp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/grehwttfv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/ggzqsxdlq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gaoszfggm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gmhrknuwh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gercmyjld.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaeaqizon.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/ggrryjipb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjndivyck.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gjttgscvj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gkyoirmbt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gwpwixsxg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gfkmzygek.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gvjkowmdw.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/ginnqkaoo.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gkscsqjca.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gwtksgzog.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gmrrldtod.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gzwlepzdd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gyslpuhbx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gpstqgoke.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gbxknvqyn.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gkvyymoik.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gsftglyfb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gkwtlldxf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gxpjfueyl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gudyrfnou.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gnouogdys.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gvmvsdnud.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gzjqnemjk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gqogymniw.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gkmurzbhd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gamflxkyz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gsamzolvs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gjohdumpy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gurbxrmzo.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gobmrmqwu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/glnukbwni.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gmyeahknr.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gzxmconff.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gjjksoely.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gljukvrnr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/geqwsdjun.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gjzrswscg.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gbrpksaau.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gtrewzjgi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gnzoaitha.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gdscqxvch.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gshmebzst.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gtrnhlfgt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gieddhtnv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gzxkyukaj.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/guinvykdd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gjkwikndj.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gndyfptma.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/ghmqimmsy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gkitmpflv.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gwigzcsqj.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gbmtlfzuh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gbgntmocl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gtqkdzqrg.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gsdoickni.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gilczkkaz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqpnwrhqa.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gbqadvaoh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkhhkovld.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gbctdyxsa.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/giqoecujw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/grpvcngtg.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gyvurddjb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/grmxvsbin.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gonusslsp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gmmpcdgna.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gddhrracr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gcobyitnj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gbxbyehus.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/goyvubhyr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/ggqofigiv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gsnnlvpnf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gfokbodyh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gtuopatip.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gmnlhwyry.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gdkiufftj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gsuaywonv.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gknegqsoe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gqhmqwnqf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gcetuaniz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ggpudtidm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gpfjnszhw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gehrhljnn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/grbnukdzd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gyqhgughf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gnpgboowk.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gcrcqismz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/ggecdqiqe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gyyizoqno.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gsdbfpqlp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gjknklixk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gspwxhwxw.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gddinynul.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gnuubdhin.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gyfplafsn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/grcfelshh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gcyyccirn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gdwbpukyt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gwysoriud.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gqwizvffl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gneepcywm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gnhvpzqjf.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gspvizccj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/ggegnsltl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gtgkditbu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/geiswavcb.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gdhhftctq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/giaagolfu.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gdgyrqakf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gjlmognrs.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gvnyaejyk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gcknyxheu.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gxocdivwg.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gilrxqfah.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gfucwkufx.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gmqpjvuov.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gpvnszcdl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gvfmwkgms.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/ggxhfipwf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/ghsehgzbx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gijaphgie.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gloqikzbh.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gwndryagu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gtfphcyhk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gpdkentka.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gpvsteqda.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gstwxbhup.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gzhxmptre.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/ghmgdpknc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/ggwhxbbip.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gcdgfwkdi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzkvcugxd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gtdnbciqr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmhaxcfok.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gyozojnmn.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/giuwdweov.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gqfgrrpib.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gfqjfgrod.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gkscbkftk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gnoyqvjpz.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gqdpniaxs.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/geykaccjl.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gfvweeizn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gzcpefyqy.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/glllsuezs.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gefpuzliy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gxhyblpmu.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gawisvjsn.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gzujbzeyc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gjpnlrkrc.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/grobhwdor.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gqhxjdwck.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gqvxmnsit.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/ggoeqglsc.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gmtkbptfk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gsjyaiays.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/giqegzvzj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/ghqwptagg.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gmrliljjx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gwedggeqo.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gmunbnfrk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gdxuvnxnf.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gessjkznm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/grdqmlyzp.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gutifyaxb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gwsjprgjk.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gtezleyxe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gspgmjrlg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/ggtyppsow.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gwwlsezmv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gstzwvgdy.sHtML


<!-- 参考信息 -->