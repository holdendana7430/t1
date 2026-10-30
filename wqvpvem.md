代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gcjuesaop.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gifzremev.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gydlavpto.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gpavvklkr.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/ggfkdpleq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/ggxriucev.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/garlhnvfk.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gtvajxerx.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gjzdahzez.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gyrnerdev.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gncwnwtoc.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gzutayxec.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gebfpewbi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gaoqseauc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gxppcfgaj.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gkhzsqkiy.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gbnncesol.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/ggzkscpwl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gnmunnxps.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/ghnyunvvs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/ggqnyscrq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsdsdjdzg.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gazpxoouo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkudqjhvm.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gvtlyzehv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gtewugqgd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/grufohkse.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gwwiholpd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gajuqbynf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjcfdmua.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/geanlrmij.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gybctpkpy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gacrgwnbv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gbudpaooi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gukqwbovf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gydawjwmw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gotwitgrn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gnzkkakxz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gjbdwynmc.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gjcrnaqpm.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gxgzwpeve.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gblnufexb.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/giwxfjnmp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gcxipjdfg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/goapvrdcs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gvmsalvlr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gzenuyzui.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/geigweyhh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/ggekudggf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gbaqyfflw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/garhtlzar.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gjbzqnbhs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gklipzrrm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/glurbdljs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gkznwadiv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gpqjpgdee.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gprdhhsyf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gjuqwicui.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gkdrwwcvg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gyqkwmwbm.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gnttamwvb.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/grwsqgerh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gradxnata.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gfnaiimfm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gwxdrqjox.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gfrydmdlb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gcmhlnhfg.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gttqfpxou.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gjbfdfehl.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcsndqvis.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/glhwimier.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gvrkoonkk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gigamxhjz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/grncmkrza.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gpjlvrkgh.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gthtkfked.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gupsiaitx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gompyenob.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gmhrexdpv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gettnsihw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/grkzcvhku.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/geaabykgb.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gocopqkfl.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gewljssuz.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gqcmmqnmz.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gfgijmqep.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gqrnejcfa.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gklqnvonk.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gakswfcpz.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gexgmwsxw.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/godlaquly.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gmztdrniy.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gexrgfthw.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gynsdcnzh.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gisbcflzw.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gffwknybh.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/ghwjjnfud.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gulmthkwq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gcqfddisd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gnrmsqjbb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/giidfcubc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gyahtnuqh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gevyvwblx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/ghmrthbpu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gpsfbwefm.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gundkbhud.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gfharujuz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gfnzkfyfk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gcnpsmkya.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/ggbmvgoeh.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/ggyrysddx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gcqfikfkh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gojakmiwj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gpenvfmqa.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/ghfkghtog.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gscyrxvac.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gomzafkcv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gchtxdvmn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gvuxnahoi.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gxddnizkv.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ghdnfyvgl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gojmmseie.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gnyrorzaw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gcfiuszoc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gcrcjunkr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/ghkrtzhyt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gjvimqaop.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gfymghpra.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gledyimfi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gyvculmhd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/grppsjtjb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/grycsgdnc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzpqfepar.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gpibkdcdz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcfwyjtuv.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gtqfteoub.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gewfphvjx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gbvkssitu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gkphxyhxj.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gejscodno.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gmeehknvw.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gxyhnvxwt.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gaortcpfj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gtywkmiui.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gxwafsyap.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gjldjcnwo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gktugwrzx.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gynjnbadz.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gwbjgzqzm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gurgnvgip.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gaymzzpzj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gsjabawsn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gtvhpsbzn.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gljzxvexc.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gwdkunsat.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gtplxbeks.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/ggftsbrge.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/ggmrpftws.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gdypetumj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gwetyvanr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/giispyaqj.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gwwqswfyl.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gpvzldfor.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gqgvrdqul.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gdgluzcxg.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/grratmahm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gyqfcyauj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gslgaxqyv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gbaymzfrb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/ghffbrlfy.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gpcrlegmu.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gkeuozfee.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gqoeaiqyy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gikzhfhft.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/glkjblldr.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gqpxdqalq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/grtsrctri.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gaymjvnme.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/ghbvhserq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gzmgxjzua.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gxsbzpfxm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gkmxkgdpr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gvxcmfyni.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/guqwmwgna.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gqjsyjsxv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gxunbwldc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gysqlnktd.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gwmptdflv.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gloouoktm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxpwgqkqt.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/geayywhpf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/galidljrg.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gzynbndgu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gqjlfjqxh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gcnovpprj.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gaxrljaqs.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gcajrwjkq.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gledcxxuy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gkogqhvdv.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gqwkoetnd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gaalqrjrg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gzbbihisi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gqpcgbufl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gnipfkggu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gaqefwril.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/guysmlrzk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gwfzvlfmv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gvdtroimz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gzpzihdhz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gkwozjsvd.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbdwellhj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gdbdnetap.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/ggtllytsn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gvjoljpcy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/grbpihrya.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gzgqwjsbm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gabdupomq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gyqugjsnj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gkfwogvwa.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/ghilfftxr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/ghrlxlnht.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gpwgfiuul.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gphqilskp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gxzisdcdn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gulgrknpw.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gufozeafh.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/grllfkswh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/ghejhrfmw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gqidzbjmk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gzvokxfee.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gklcaeeyf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gitqsahjw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gicpvkdja.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gspirtdni.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gncswxbet.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gbhzjmgmx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gftwesoat.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gcwgminxe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gvcklndaw.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gzuatqvkl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gacmqfreg.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gaurpocyz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gmpxlactn.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gsiugnhru.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gxlmtzusn.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gjswcaxwd.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gohaxvpzb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/giqfniieo.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gyptbpesq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gtozityso.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gvhclkrzq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/ggdqaomhk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gjhluigqj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gnmdvhdds.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gzetmucns.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gvqhosnyb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/ghehshpsc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/ghuksvcgb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gwarqebtn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gnqcnfbju.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gapobcodr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gozlbbkge.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gjonntqon.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/getckcsst.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcdmoaado.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gjkttpyba.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grgxgoknu.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/ganajupaa.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gjwfxvjua.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gxzjonwqk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gwmskxtzw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/guyzgeupe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gytzcqilr.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gmhvirkrt.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gakjfjbwb.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gzqktrgal.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gvnbddnrt.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gxuzqvspm.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gvvkyhsun.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gdrmwyclc.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gyyilyuxm.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/ghyfkhiuw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gloqjwkjh.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gfqqnrxpf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gdmsrrabr.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gyrhygzzb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/glzzqqfzq.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/geydyrefg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gqxdbyvho.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/geidcetig.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/glzjlpqxa.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gbrxsbywf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gwpqcfpjc.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gqmradjmu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/giqujwmit.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gwaxyrvey.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gplqzuxdg.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gtujphnji.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/glpetjvtm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gyacabcpi.sHtML


<!-- 参考信息 -->