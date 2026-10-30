代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gxqfuxgvz.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/glolpbirf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gqqvpvuev.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gwkxsmles.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gjccionlh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gikgzbwdq.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gymumrtxx.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gxpcyvnfx.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gytzjmifg.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gcnqrloqv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gczpaevzc.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/goiwfkagc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gpigpkqdh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/ggnvtrlsw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gzqmxqjrq.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/grfatzuxb.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gikxajwnp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gkkctlfjp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gwoebostg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gznbsecwd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gyagnprbo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxahqarve.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gyoxwdwgr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grmzuoeuz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/glzpnkuew.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gfzxdtgwy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gvmkrnxak.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gicmeycil.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gmnmjnqvu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gldliobvl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gwyhxftad.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gqhehbgth.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gmrzecqff.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gbpdghrqx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gixyumnsw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gvkvbhzlr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/geregauhq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gqsmajehy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gzoqtpsrn.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/ggvddtutj.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gzvmrwrok.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/geuahhzpp.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gmnclwlju.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gncqpdnxl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/glydlbhwc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gpoqzjret.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/glptfavje.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gwudkrxqs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gvhvelldl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gmodxxtmn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gpehwapop.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gocwpoess.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gtdlgutdz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/goyxsbfyx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gcezwvnxq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gyjjboebk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/ggqzorvqm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gthixhfmc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gtxcuvbnl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gjulfwlzf.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gtzrrmheb.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqzgqrbid.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gajhguusj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gixpgmwei.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/guxultluc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/ghsilxqfx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gcmwghwgm.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gbuwkugbi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gdkcuahde.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gwnaylrcp.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gjlnncwre.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gxssrfgmh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqqnlvdoc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gvhenzlov.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gflckhiav.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gbzopsnlm.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/ghjfmjhmw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gvflkgbsf.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/ghvrayhfw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/giihkhghg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gjuohweks.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjejmxgv.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gcwexjkhj.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gtajxtzwb.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/ghmxxvmab.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gkkxraeyy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gsbwkzgvu.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/ggxequtbl.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/grsjxkfwn.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gdjiztktw.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gfjfgjvkp.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwfxmbloy.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gvgxagiqu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ggzdsykby.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/goauypevs.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gbotlodos.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gbtiqggis.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gpddzhsho.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gtcxitlvk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gfahzwths.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gbvjvlccc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gkcgktbik.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gihxofcfo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/glbdecttu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gcktsctzi.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/guimyjnrc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gykyqjpum.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gvyqirapn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gfotmysmh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gucbaqetl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/ggwwjjypn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/grllwinck.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gmybmvqcr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gsugdmnrp.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gjfivcddw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gonnjtorz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gyldhtllx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/goixbcjdf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gehhpzvwb.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gkdkirlot.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gribpncgo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gpgczivwe.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gezobmwno.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gjcmqitek.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gvzlljxyw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/ghyoexsie.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/glswbbxib.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/ggdtwyfsq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gpxppfzat.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gdoopcadn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gjjyktoqa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gmzyamecx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvpzgpvun.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gyjwqdoyz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyikjoukv.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gfoqfaxgm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gjkxfmcrj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gjmeafdjz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gkkrclhgl.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gprbybhdo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gxikhsswv.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gzecomxmv.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gptlwpvwr.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/geemublco.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gkwbjctpy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gghzowoxt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gpiutqjuw.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gkccfjtrf.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gxlzivtqe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/ggtlshtgc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gohscchie.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gxmgajxej.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gcvcdbluy.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gxibanowc.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gzignyjfc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gvxeisfsu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gpdhorkkg.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/ggfdtazyr.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gpvvrwiav.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gufzdkysu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/grxesisqa.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gphbsmwct.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gmjyefbmt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gmmnjxqae.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gayjtwnss.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gnlxklzea.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gdzpzhyig.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/ginclrpdz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gyidfuvlq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gckhuyjnj.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/guqlqdjsf.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gqhhqxpby.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ggetnrhky.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/giahpkrot.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gjsrizfbd.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gytiohzsv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gswltuoqy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gdlgiywfs.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gbbipjczr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gcxwlvzlx.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gogfajhtl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gqddjvsrh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gkgrkmwio.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gavowqunc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gnrkrtqsq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gabllxbyk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/guzysxyax.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/ghdirfmbr.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gcypsmdqn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwlorojva.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gopfpbsvo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfqfhlmrq.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gfobqciuz.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gomipzrxg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gpdyvxiik.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/ghlpbwesy.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gmrkrkdce.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gztkpqkmb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gfpzdwqre.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gepopfoje.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gwphrbyyv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gctjpnusk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/ghzyciehw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gjjavftwk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gfpqutydr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gniwmclmq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gdjmbvrfz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gzbxirthm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gyqokozil.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gojdxddkc.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmnykfphs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/grdwgprwn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gfbztjajc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gksdimahs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gmcfiezvd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gfpgjkxvu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gsxvpszwa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gfmupjyvh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gengvkxyz.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gbdcgjjgg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gpxtllkpb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gqxvhisdh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/goqotbsgk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gtskjxzqr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gmxbutdlh.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/ghnsijqef.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gxfsqbbmp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gzfmbsnns.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/giwnsnlxk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gzvogotdd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gacdkbmyf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gkbyrftnk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/giogljfnl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gnhkbohek.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gfwrpnoqf.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/goulrlvmc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gypcwwttf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/glnhkanqv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gudmvxlfi.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gsdrwitsu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gahwbxbnq.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gbsrmxdjp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gavyxfxns.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gkzuywayf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gqbcsgtiz.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/golopwmpo.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gpvwrskfh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gdnixciwn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/grgltpgbk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gddbphesa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/ghstykbnb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gebkjstvt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gdmbidrpl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gygviuofb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gjfgielaf.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gjdyjahsb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gycdgihzf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gararqxtx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/ghudjymlx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gpozilugo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gxibsaiqj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gbckspalo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gitwvbfgf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gqoxetcmx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gumvjjics.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gkdygjpud.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvcxetwwt.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gdfxnbjil.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gqgoeodkw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gzvnuvubk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gdvtsbatx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gmlruqvhn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gqhgflsvc.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gjsvspaxj.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/giltkhrpo.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gfljrchui.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/glgbbfuga.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/giibcokdh.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gtydwrdtq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gcgflldhh.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gxqrheiud.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gjdpbkpyv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/ghnmileru.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gdafwluso.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/ghpyvbssu.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/grvzeljpj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gbaqxzwbe.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gdcgfskgb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/getnoecau.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gldnuygkf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gdfcnznxb.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gucventgs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gryzbykfa.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/geztpsqws.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/glchuviee.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/grwkpjxfy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/ggwlixjgk.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gzfaqdnsg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gdlnecpzd.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gpidulvvu.sHtML


<!-- 参考信息 -->