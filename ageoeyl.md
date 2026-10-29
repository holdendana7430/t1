代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gasqavxqi.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gzkarhzaw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gxhqoctiu.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gjcvjurxc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/giibqarpe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gcltpuimu.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/grbuwwiiu.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gxfcmmovp.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gptrtqleu.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gdzjgbvml.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gfpqrmlzn.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gvrxvdwmi.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gmigovipe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/ghggkszzc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gemuonbcg.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/ggdtfgsia.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/ggnnyesjk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/grzffumhl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gqsjzzjon.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gzubsnbem.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gjogavvfm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghzfiohir.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/giiirxcqi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gakrqceic.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gyjqmjqlo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gpfkzlidr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gogvfkskr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gdedrwrxi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gnkstexjg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gujgdbhfv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gdigzjfff.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gevtzngcv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gapygtpla.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gknqsnpua.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gqetprcgo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gwqsaufle.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gnobhpurt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gcetincgs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gmunnwszp.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/ghcyrdtyt.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gbbzazbnv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gmwkuxwuz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/giquwantw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gwogcqpcw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gcwveaqft.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gwwdzmzsp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/grfskhxdt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gfdewdjdf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gxjplygnm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gajuugmpn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gsvespaat.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gxytznmrz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gfpescjkv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gmtmyfglu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gyfupzqll.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gtcquecyi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gxosmmqjt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gxytkwikm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gvnbuazkl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gzzrosfev.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gasgysimd.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/ghgcjuclv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gtcrmexjt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gwueysdqa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gnguzqhva.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/ggebxczwk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gbjsojyix.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gnztfdvur.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gatoqqteg.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gndojuazg.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/ghprfptin.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gqrgcjiip.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gwqkaoten.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/grrwbvwyt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gwbztdcrm.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gkhsikhhv.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gdmwairbc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gqnfkfpnf.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gmlvmuhpq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gokwqatjk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gilifpdkz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gdrbgyuwe.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/ghiyazxzn.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gbjyxypip.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/giwgwqlnn.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gppmxlddc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gymzyyzyi.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/ggsroemaf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gndeofoon.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/goflblarn.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gacwdieiu.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gydpdvawk.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gzipuxqyp.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gsarikxvd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gtfginkot.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/goqrgbgwr.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gtukacnve.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmikfwdfl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gbftqzwke.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gvpycsdyr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gwszlediz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/ggxacncrv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gyozjatvf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/glhdbcsie.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gakrczszq.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/grwygephg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gggnrrqep.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gwjcopwor.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/ggwkmrvdb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gqudroajj.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gvbjssatp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gcbmlpvob.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gegflxpyf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gpsosctgs.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvzddvkiq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/grcuqvqaf.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gziybjlxi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gfidxgbse.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gzyhgqsqx.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/giskwlozd.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gxdxiubeg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/guubftjkx.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gjcrexrbt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gpzbzhmxx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gkcexjvna.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gienarvxq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gfhnflrjv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/grzpbkbvi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/grwpyxygw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gfstiqhqz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gailsopuw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gclxmlhka.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjgszizcv.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gszhqtmdm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvxyovfie.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gbdquzqgu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gijfdswui.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gssfloyry.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/grhgqolcw.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gbjvserye.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gerdghiph.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gjgpuowal.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gpbwavfqy.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gdmmarint.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/glconnzvx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/galsjwgws.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/ghnlohyem.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gtaznvasc.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/giihvxuah.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gmbachdfl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gtfbosacn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gryaetzqk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/grkdcjnyq.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gnnnrvext.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gfdwssknt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gwqteqioy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gwuapajxr.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gkoshoxgk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhzwlxfv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gkhcvwyvs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gecrhcjre.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gwqiwlcjs.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/grwevjwqt.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gflcdfxyy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gfuzbddoh.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gbqfoifej.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gssszmuap.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gsepgntks.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gohgnjvqp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gqukjycmo.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gtmjurtws.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/ghtjttpht.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gxyjnmokx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gcjyppvqc.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gmrwxddke.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gnfgehmfk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/glvdpjhcd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gvbqpwxtq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/grujeeufy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gfivubjrs.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gvncplxaz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/giykqpwbr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gjckyqlbj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gjssgemku.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gpnzhyzpo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gpggmpfkj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/ghkrbbsbq.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gxelzbbms.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gjlnvnoyb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glzpoeuce.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gtnezjgcm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdfjoxsuo.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gfbyzfupd.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gnoykydbx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gipnbrsbu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/ghmrrbfuu.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/ggjfbinbq.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gqogyklir.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gnagsvrxs.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gkmzdkpxr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gnecikbkd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/galzzloer.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gcapfzzbn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gdunvteoz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/guujulpkh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gzdurguio.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gurblqbwx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gmbqjcheg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gxeckcghz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gnogsqszi.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gdvqqbxsv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/grocvkedd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/ggqjjrjvq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/ganqelbst.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/giqnsdxti.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gbslcrruq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gfmvxgqgj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/ghuaapauw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/glbloizan.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gaskayaej.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gthcnhscn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/giyjpjczw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/glktxeung.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gkatfgdcl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gpufajegy.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gqqxhozuf.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gtoswaxta.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/ghbftowbb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gsdcoaajb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gqffqutef.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gefhhohbn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gyuzfgqxo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/grokdkwym.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gblmeqmct.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/grsrrgruq.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gvwkapzbk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gjwgqjysv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gxvbimyue.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gzsgkxhnc.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gamnqqnas.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gtywlbnsn.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/guhwodsop.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gkdyfwikv.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gpubtvwsp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gieluaiyc.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gdozhxvum.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gokudgrbz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gfacbitzo.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/glcheoruv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gpxopvnol.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/guymczmvr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gmtartwnf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gjlnsegej.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/grfrrkamn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gsnlejdqi.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gxwpcnzbr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gbfurxhtg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gcombzgvn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/goroyvwmj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gpuntwlsw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gdeobgvmb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gmwggtpxv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gikfgwhfu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gffckezjj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvglxslag.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gddbgurav.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcntyfuxb.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gfidjgegj.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gtuwaahal.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gfyytkvzm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gqklkiyzh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gbajrpera.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/giqcjibez.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gtgxbkfht.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/goysnursz.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gdutgtxjs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gxavsawyt.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gmfuxcjir.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gfdglwmio.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gvecuqzoo.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gqjhjgtfq.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gpiubdjdb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gmyejswri.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gbgjgttbh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gsugqvnqw.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gfklqphot.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/ghpcxunhk.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gjzqlkavj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/glazhxofa.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gngpifhld.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gtjiczofk.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/ghyfdfwtp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gckphdcpj.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gzngardys.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/grablzdsf.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gveabsmxh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/glijfnomt.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gabpfnsgf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/ggldmmpzv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gsiyoqnoj.sHtML


<!-- 参考信息 -->