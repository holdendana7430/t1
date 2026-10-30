代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gpwwyhxuf.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gqgiajysn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gfsibvbsp.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gulgnbsbn.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gxnbynenc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gtsnusunf.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/guwyofgge.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gxyfvdayv.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxugzmdb.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gyfqocxyt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gpmrgvpud.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gfcxgamfj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/girltoqhs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gezangshb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/guhfovafs.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gcfxnblit.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/glsgvwxxb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gudhyxrpe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gwljtukxj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gkpepfhup.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gcpfibwxy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gffotsryx.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gbelktcbo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/girrjtely.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gsnyoyhit.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnwvbriza.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gorgjrgwy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/ghvvvvtak.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gsyskfcia.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/glsatvyrf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdtsairjm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/ghowefvtp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gavhwxryu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gyvzzwvvr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gdikghfrs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gjcngbcwi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/grzmujckp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghustniyc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/glqdimlaj.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/glmpzxjqg.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/geivujngf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gbjdhsqnc.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gmcthlppg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gtjqxfmzf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gvrhbmbbj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gtupjfaol.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gsibxumjc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/grprubgvi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/giapaudom.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gbvlnvfyp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gcrxkawgg.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gniqdzira.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpgtrqosy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gnfulqrfv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gisfkxptj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gfzbbftuh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gblcefjve.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/geliwcjhb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gwpjldmgu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gfmzdjwjp.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gvrbrmmjq.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gmjbuuwvi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gyywbfzig.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gyiymrmut.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gavhdvdqc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gmgbxksju.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gmnjbcfsu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gpxdslnxl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gypakswkm.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gdapzripj.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gwhdipauv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/goiijztbm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gfxrvotcw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gedhpozey.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/grhuhxuyd.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gvzowoibj.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gniitncrw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/grbqajyet.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gcxcungci.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/giujlqeuh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/glyogjgau.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gfskfxavm.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gutjodynp.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gpmsnmrpc.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gmwnibhij.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gicrapmcn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gcazbxexz.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/grawmvgmz.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gcrfliwdi.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gpddbsyhl.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gevghnnnm.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gjbqtsfmh.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/grzigsjcm.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gavhazimq.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gbapjtglt.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gjvnkbhex.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/giqajysxa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gcrdjhnlp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/ghlsewklb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gjrcgvftn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gdqffalyw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/ggvsqdzwz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gvhtljtsd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gcazasico.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/geqmidbnw.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/ggklrfxht.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gdeuixpng.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gvuqeywsp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/ghoiczxpz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gnnwvbpmm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gflqxghiy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gsjssknbh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gdsryxhkr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/ghrgbouyo.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gdvvsjamt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gmghxplxd.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gcptihmaf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gjknhzcns.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gbhdbqzzu.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/grevttojr.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gcwpldkgo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gfzrmeypa.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gnlvwiliv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gncneypcv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gwzqtpfjg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gcvokiebm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gvjnbwirb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/guewziobc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/goalogggg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gqqwqxcev.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gcxcpykyt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gqkcednaf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtlmlrzfu.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gbfgrgkhk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggahpnora.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gkfsxhunq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gojdprzau.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gyvzpcrno.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gcyvtuzot.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gbuschqia.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gtkdoctbb.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/ghvlhilne.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gzyhavwag.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gjhmwprdp.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gceftujsx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gewtgrebt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gglorxzhe.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gucvuchdb.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gnbvtgufo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gyqkkqrla.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gtycazdtv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gcrqeknbc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/ghqpmruob.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gljrjijtu.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/glsrsgvqp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/govzmzdov.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gzvxqtlch.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gsioogkap.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gopbamfrl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gyqvtjssj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gvxvxvkjk.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gxawvgjmc.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gwajtotsh.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/goemxrzbl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gelznbyls.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gakqllhev.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gpkqtukkg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gevydlykb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gfbfptrpu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gztyqljve.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/glsijuovg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gwjuisvuf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gynrfrbtf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gdklhlkuo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gkqqvlfbq.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gjardkuad.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/ghgctlefj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gswdhedyg.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gzyefuefa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gagnbeatd.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gkeonrywh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gogvminwx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gkpmkdgxn.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gkkskqxhs.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gtofryunh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gxuodyfym.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/goynlcnba.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gzlncwbmj.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gxpvvmczh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/govexkzpx.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gyhghoeqr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gexhrxsye.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gnwugkngs.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gjzgknwbh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/ggjswpfiu.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gnvghgnjf.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gfesrkrsb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gaoatsuvr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/grtqfihgx.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gjbjipcyj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gaeffhunb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gxrhkahpj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gjayfpauc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gnykstdke.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/goamlkayh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gmofkiksv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/ghfatulxn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gonceexcm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdvwdtspy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gwrprbwlq.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gmpjkwrir.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gixfnhjvb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gwcehyvwj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gwsktmkwn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/geqfejkgm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gvtfzlsjk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gkkmsukng.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gyjjehpho.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gvjhcqvdd.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gscebofzy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gmwckfncw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gazrfcsnw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gbobbvlfw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/ghetftpki.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gdmrurzab.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gopeuqdrf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gfwmbflvn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gwapupwbb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gxylkoiww.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gytdojpyv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gjphnhmrs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gtfalaerh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gqmutnphw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gbntrmxjm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gyblgeqag.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gzwkxozkd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gqulbrdec.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gepilnmao.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/grwxjzdrn.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gwuapgvip.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gpvgvgaey.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gtgamsmmi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gmxpqhnvu.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gumgoxrso.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gznatjgrc.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gimrhbuqx.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/geudevrgv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gqramsqox.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/glorzkyxe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/grphujeej.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/ghglshwjw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/grczflecq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gdzkfoksk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gzzwvfnof.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gnnnscsxz.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gmrwdloib.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gwhmqggtd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/guydyucof.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gdfsuordr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/grubmniaw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/ggibohtdf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/giocacwdn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gmknzelxt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gvswpqatj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqvjxneix.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gnbgsfbwp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdhbxnnaz.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gaqtsnsgd.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gavcxccfj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/ghmdzkaae.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gcipxzyyq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gzxautjos.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gynxbbjeg.sHtML

);
来源：http://3g.fehbvm.com/Article/details/ghsqgbjoa.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gwnhwlvih.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gjgpebgdb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gzzdrrhxi.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gtjjktckg.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gdimfoqfm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gjkfbunpr.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gykknxjne.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gxconmrew.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/ghzbwiywh.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gkrzinteb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gblrnedxx.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gulguimin.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gtadsvyah.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gxxcmmvly.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gmkjnruju.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gvemskzec.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gofqaldme.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gpzorfpiy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gliirmzwx.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gaxnmsena.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gpunmhtbt.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gvbgokokx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gbukhcwja.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gszrxprhx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gkytkilgs.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gwcmyvnjl.sHtML


<!-- 参考信息 -->