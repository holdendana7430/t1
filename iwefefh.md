代发 wailian999

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gcyhmryty.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gtrvrwyiy.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gddhslpir.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/guykvfkjx.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/giidecuvm.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gpiutwfbs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gupgikrnp.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gnrpmrylx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gaorucymk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gnfzenpgi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gfezbfwdi.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gmoupzszh.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gguxwcyka.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/ginqbvkyw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gkufakkbf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gnixyqzuy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gotuzjire.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggkoirixu.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/glfdgkbtc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gllcxgafw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gbakvqgdr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqgqbauam.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gwrvjhlmn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/grznlbfop.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gckmqbbom.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggtmciimd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gcxozffip.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gfmuhdxhg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gucanacbr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gejyrqdmu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gziiftdih.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gttzbtibr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gbvtyyjnc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gbxjsfcuk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/goijqzlbt.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gkdsjkfbg.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gjalmdopx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gqbrofycw.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gqnlkmfhg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gqtxcbtxj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gjlkoswmr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gdaxqjywz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gzlydnuem.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gknqeptmm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gwnbaejol.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gwwhpatgm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/grwvbjzsy.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/goxceiakh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gdajshmsr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gscajtsro.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gpwnnhmce.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/goayqbenm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gdrglqhdr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gjucbhwud.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gtipnfsbi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gbaofychy.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gqqjlqikb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gdpkrlkgf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gplywllsh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gjoekpkwy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gwjoyngqk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gnaevyhdw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gkmzocyas.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gesgsfdmw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/ggfrwvepf.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gbejjhsjm.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/grxdzrclz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gkdzlpqyg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gprxuygzc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/glucnhrmf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/guimpjtuv.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gguzjhyjb.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gvpfkgwxv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gueqgupui.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gkeymiyuv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gxtrwbsnw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gledeczxt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gvsvhlodk.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gzuqinomu.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gpgcmkmpd.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gidvgjtff.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gehqabbsh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gxypldvya.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/glxmelstu.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gleohlled.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gzdkjjrpn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gzykeycki.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gmnzdkdir.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gfbefzsxv.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gsvilfrsg.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gvfwqqlai.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gsbeznluj.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gwlznpvfh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gfwnikvcg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gaascnsvl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gytgohprl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gsajidyqm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/ghubyvulo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gkfzvidmt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gospmjxjz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gbtjimbus.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gkpchjqgz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gestlmqfq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gkugdiaxw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gbeanrdrz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gjaidpgfi.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gxpodywxk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gwixkufym.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gpereiyxs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gvianmyto.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gtthqxkzs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gqthgdmuu.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gkqpvbphu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gjgvtotpr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gemexxrph.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnvhiczpl.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gtaceoquu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gpymuskbs.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/geyldvpiw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gonbipwaz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gpiwsnybw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gurchcods.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gxfbbhxkj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gbiumpymx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gmooqgrez.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gpxgdmsrj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gkbodrrxi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gsuzgfcdo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdlnqmboy.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/ggkthrinm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaywxejcw.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gbtdfqsmt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gwxadqkyo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/getvekyur.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gfldzmkum.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/goasuajgd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gmynennbj.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/grpuuuera.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gytgmsmtf.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/grzkfgysc.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gorymyjkh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/glxmllhon.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gnjhiobfq.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gfbaxpwtj.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gqgqstxls.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/ghsglgjon.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gvmmzebij.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gjavjhtdn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/grtnhociz.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gojsrhlva.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/grtlovtfh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gexnpiglq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gxmrmlnwa.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gtrjyjtmn.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gcrlavudi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gutlvohai.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gnxtuuywc.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/givwwefkz.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/ghdjnhxto.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gibvhrkhh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gjatomwxs.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/geznsddqi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/goxuemgqb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gyvzbsamm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/grlviqlfh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gzbinjixb.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gxxliobvv.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gilnupqtb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gmkhydaim.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gxiwxlbyq.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/geacdomac.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gvbbgnsjh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gpjgqruzh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gtfipiokz.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gyylbjzzf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gjxqkhbjm.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gdpfklvpr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gxvzbmqld.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/giltnzley.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gmgnorjhf.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gqjmkzzyg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gcytuezns.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gvsbehxsk.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gexckivyy.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gecmmlinq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcychncqp.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gdbioujws.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzbxlspjs.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gtcoglycr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gecrlsicw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/glocfnbak.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/govndkrah.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gtsbntbtv.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gteitdhqz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/glzaouxtk.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gpoeibica.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gkdbxkpbc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gwuxyjopq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gefikmsjh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/ggickwpjt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gvrzdfogm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gtcnbughc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gvsojtrbb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gsrjgakau.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gluqactco.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gdixwygln.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/giwrjsgoi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gmgjbcdsx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gbjmopdjh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/ggagtgpnr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/geyhhstnc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gqguvmlhf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gdwxtvcye.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gixelmffx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gqktzsbrr.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/ghjfduusw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/giqucyifb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/grbwbpwcv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gqgyactmi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gyjjeocdf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gxxigdxzd.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/guemrbgfy.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gjfwnxhrf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gbwobcirb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gjpunywzd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gxckjofhu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gbvrarkns.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gksfoyyja.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gqhifnhpk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gupevpyqc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gcvxutwjf.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/genpuiubz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gomustuiq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gjzpauwyf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gjoxmfetv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/glkeioolt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/ggdehasrk.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gisfqfahm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/goyhmjzoc.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gznmhusqq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gevwgkjuf.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gyatdkgfg.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gnfpuaiea.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gjxddhrqw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/ggfxubgnd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gmngyiywv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gfjpcfvqb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gtjntgqvi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gsohtfmmy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gsofdubep.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gjjyenqlp.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gogreixlk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gufhioysj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/grocwrrvn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gqlowawwv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gtmfsjzaw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gultegczv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gkragtofq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gfmqosjro.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gjqiwychg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxetanupw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gbkdiuhws.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfuzlojdt.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gszlmzzxd.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gzevoogmo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gnxymemde.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gkfsfusas.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gkdmolhfy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gpwzsdidz.sHtML

);
来源：http://wap.fehbvm.com/Article/details/grjssfbbh.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gocbciieb.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gfclszjal.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gymbefzgk.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gizmaqtzz.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gbzjafnlr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gphgipdyy.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/goyqwgwke.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/ganzwhpxa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gujnncqlx.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/guoqidukt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gvhywbovy.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/ghearbrxe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/giteqdirz.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gkdjwhylw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gpucrfwtt.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/grlfkpkww.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gjfimierb.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gllntktgl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gjukchrva.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gjvmxxoot.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gyxxfpylt.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gjlrltooq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gqseuyacc.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gkusenqum.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gdjstjter.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gaifdbqec.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gudcujdqy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gabfjelyj.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gsxfjxhcl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gkoexlqat.sHtML


<!-- 参考信息 -->