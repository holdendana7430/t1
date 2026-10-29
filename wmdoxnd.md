代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gxcjwxwwc.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/ggvfmqhop.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gjgvllhxk.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gfgguvipd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gadkouwkn.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gtslfumgg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gxnyyolhj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gixgfmfdq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gifoojyrd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/giodwottl.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gahvbfvjp.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gikskdlcw.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gbohrblbc.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gqsuaeoug.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gckgsakxx.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/geuzoqrte.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gokuxtavp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/glukewdcb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gdzlixiwk.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gfvbfrsdu.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/govkjexbj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gcjkyizbp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gyijmdtyg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gdnmqgwyo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gvorhjjlg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grktvfjlq.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/glohjxesi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghcfelemh.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/glqwkvjye.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwxybaypz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gigirweqe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gxddxirid.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gmjjetzpe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxpanjhsn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gpjdispuw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gflhkqpgu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbymvteof.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/glffojndr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gweweifjq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gdwdszfbw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/ghvhaewpa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gyaegwbrb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/ghdtgwyyj.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gtpxdbako.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gchepwcfg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gfdvqworo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gtraqfsxh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/glsebjbge.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gixmscmzu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gujhjhstz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gzcwlgsfh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gxcefmwwr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gbjlgvvyc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gwaxjzvil.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gnhdirymm.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/grfkjzrhk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gkwxodaze.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gwtuxobbf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gkofpwxwy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/goqvfwcme.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gimppvaxj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/glbyguyke.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gdfukziic.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/grqgubhao.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gjzzwfwwt.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/glqcshjow.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gnmkktttt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gqgayyhxl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gpzvyhphh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gdwmvbuce.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gfsxsphgl.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gkzxgelln.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gqdbygmli.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gbfixyvpc.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gsiirlbww.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/goqymvgop.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gdmejogic.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gzrazczud.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gwamxquwm.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/guzsvbqvq.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gdjecazmb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gwhxkctic.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gcxkpywvo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gfycoduro.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gxiabugqu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gujftomzd.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gchdvmdun.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gtkvievpi.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/govuiuifb.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gbhtfkazp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gxcpuvelr.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gpqetdoyv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gbngbzhdx.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gntzqopym.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gundyimkh.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gwwmjgbjo.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gpzuylwkh.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/giyifsgbi.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gafzvdepv.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxoxzgfna.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gnnavmsnf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gribaojjr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gtdolrurt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gqxawzeay.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gfwcfnkoz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gppmtzney.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gmjqpglwd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/giwvuivnl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gdmjhaaab.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gqaciotbc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gdynwjfdr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gfgefecyl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gntzkyhwu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gfvdpucrv.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gpuxduvgz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gmthedprb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gprhfowmf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gmkjkbgff.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gmovagxio.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gxpepbznw.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/grxrrcyys.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gdnytrxga.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/giclklivh.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/goqaprdka.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/goxxuebgv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gsgxqehla.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gojymjstq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gmjbrsyta.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gdvzpirah.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/ghosedvqn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gjpyrpvzx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/grjnayrqe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gdcgmzrwa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gbekroxgn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gdaxuvrdr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gexaseejo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnhqulkgp.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gnupdwuus.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcpjchvkd.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/glnifopxm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gmfoucako.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gvdfytcct.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gbjukhvbm.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gdhduntro.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gwxfpqxka.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gglzpbqwm.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/glqfiiobw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/ghgkbxsmx.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gdeaugokt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gxswggxlq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gzpluhlty.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gzwojcqty.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gghmyxqlr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gmcfqashp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gcbtwhdbn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/ggwhldajr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gdxdatrbe.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gpvebjjer.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gthhvrrja.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gyrjurijc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gykiirvfn.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gimatvdbk.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gdfoqqdyr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gqdexpoow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/ghicspuru.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gxmwzwegu.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gjtzlhdlp.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gvxkvsfjv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/ghzlbwkjx.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gameibziu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gfjtmkzch.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gmxmfkchg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gydsibtai.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gbdlhzozw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gihbgosqn.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gofgkvspq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gggebpvkv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gaenpwctl.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gqdtswarw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/grmkdrsxz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/goyvibtvb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/ghouchakm.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gqlotroqp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gkrrvucve.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gzqapyolz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gmgcqwitv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gbrmcqtww.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gidsrigte.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gkkunugbr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gnluouiht.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gjsfgshbb.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/ggfuolalq.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gjmluokhz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grjsizmmi.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gfccihtlg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guekxcfiv.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/ghpvkqlxe.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gmcrozmjs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gjlxbhtzq.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gdxnzmliy.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gxvbkalaw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/ghnqmwojk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/grlenxqsp.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gkjuqtfld.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gvotugisx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gefgfspdw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gbpchuscy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/genaarubc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gokyrxxhy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/giunbuwno.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gifkgalmf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gmcywohll.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gbghdsdoy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gilzxnufp.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gqavpfobe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gqdmclkjx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gtypzfjbl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gqkpyfnub.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gjfskfspt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gysgdowpm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gnucxgera.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gqkluelyi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gyiganqff.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gexskflir.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gwzybjhhn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gjvfxqgav.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gvsnjxtpc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gvmburxdj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gdntthlmo.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gvppjaxnu.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gnbkvxxfr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gbuwbxxzt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gwsmyozvk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gjzdyatce.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gnlxqukyu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/ghdjgifvf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gcykkyikr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gycxogcbk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gmkvmfrud.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gqogowxfd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gfqfpuhxu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gaalsteph.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gvetppeld.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gnbugdhvv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gvumtfrlk.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/giduutfxv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkwhxlxuq.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gnxfuqkdg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/giyeacckh.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/guwjupazv.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gqffonydo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gejgdgfqn.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/grvieqmnr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gqegvmkuf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gtiojkotv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/grlhlkhvh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gjmclpvmu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gxwuycdyv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/guykxdzhp.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gzlmdmzxn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gtrzcrsrl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/ghmpwlqrg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gtmyivmgl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gjvngskme.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gupbhqydj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gjesjozso.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gvhjtjokd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gbtviefhw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxrmrldng.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gpogknjtx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzaoumgkz.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gtdkiquiv.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gcuvyflys.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gvdoiclfx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gevkcizrm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gumlsdbiw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gbyeokioq.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/grvtecknq.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gafgstimf.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gjlnescxe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gdamkxjij.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gncviyegc.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gkkanwgtk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gqotdwwfa.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gjvxhpnlc.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/glevxyrkt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gnxczkpat.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gwndlfkqf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gducuhfol.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gyigvdrtu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gpvidimjk.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gaxjzskjg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gyrnhdkvi.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/ghjqqbwpq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gofjoxuty.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gnneebnyk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gdofdiezv.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gjkznlmbw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gpwojshjm.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gssinmvay.sHtML


<!-- 参考信息 -->