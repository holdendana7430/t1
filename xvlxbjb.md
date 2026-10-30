代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gvaehztcf.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gjhjntkmo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gsihefyzd.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/ganqzfzqn.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gsbuzbtal.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gitemkxpn.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/glxbhhvdo.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gszfqbvqi.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/ghfbxdwyy.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/ggqiadykb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gimutghzs.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gmcwklcwj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gbofgdhen.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gqxfdqfns.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gjlmmoufb.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gfcotisad.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gnzfazqob.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gqzmnurtk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gdyaquzzg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gmniloywa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gxdxsivkr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdmdaewkr.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/grbglnuee.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnpkmoqcg.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gmwbjlfwr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gdmgvjsbl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gsehftvya.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gajoihmve.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/grnuxhpvz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdpcmhgjt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gfkdubkzd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gfqgqbkss.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzmpvwdxc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gghkhsppk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gyaqoriwa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gnipsptnx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gsqkrjpwm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gsdgrhtzs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/ghnrwmhzp.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gzgfcuche.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gjcrkwlfx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gcwkjbmsk.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gpxpmpszb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gmsxkeqzd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gnhxiiyfo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gjpnpqsnv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gjohmotlw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gmbfpgghn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gbouamptd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gqoogisae.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gqfklqjki.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gtctghzam.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gepdmfzgu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gvmwflxra.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gugbitwoi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gitwaydvu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gnzxmqzzw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gtrtugemq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gtldqngpe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gppetadvy.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gcmwlwqdp.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gjnaubylj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gikjnrmzf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gnzrsxudm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gpnkwaxsd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gapittkza.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gaxzgqkgj.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gpudaokum.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gmgaschrt.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gfzjpyygo.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gmghedzvg.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxqkgnzhl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gtvistinw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/grysgfizi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gyrrlouhe.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gapzhdlou.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gugmemjdb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/ggkvvuqjh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/glarnnqtr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gblixfzhn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gdahawccc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gzktsvtwp.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gmihsppgy.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gamehnfft.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gbfkskshm.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gfuowxlwn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gzgkjxlkm.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gsfxttzef.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gslrwgdec.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gewuopoaj.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gdfphrbrr.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/guujferkt.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gzmxdylbx.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gqydtutpe.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gmymuarvj.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtfalgufw.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gopnzmbob.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gsxiyhcun.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/ghvoaeddp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gpmozlzfk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gervdvvlr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gpuykyxft.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gbmegkvdb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gsdjkbond.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gtsjabrzu.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gwqqycxhk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gcgotkndw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/grhyzwrrl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gzsckwaxg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gmesmmsdu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gynqgsyzg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/ghtyfxiqk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gdrzhouti.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gpxpzylbd.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gyjtkhfit.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gsewsvsad.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/giglldmva.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gszptaltl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/glfaeoehu.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gtdnhndpb.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gfikdlikh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gldroblue.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxihrcmxc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gbthcipdc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gbyfcatea.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gwiiobcyo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gpqxqblwt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gvinoqmae.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gkuvjosna.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gwhdqbpqi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gtjgytmkh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gedaxjtpv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gezfhdpwt.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gqjesymbt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwfcwohhc.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/goghkeqym.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gzigiljbd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gnpsfxzlo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gdjmizwkk.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gbugmlbmi.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gfijjqrxr.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gkrpvcmff.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gdynpltcp.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gcilwyxoo.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gvusakmud.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gnnwlfido.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gdsefakwo.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gaywhconz.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gvyrekiot.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gyholizdm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gvgqyeady.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/ghrzxextj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/giefqlkof.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gfgslmoks.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gpugmjmzd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gzsxdeuzl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gmymzruex.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gbcjsyrka.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gnzpgcbfn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gjljbavjr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/glqtchtkw.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/ggbawpjri.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gjrkdilqa.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/giysosiqy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/grxzarjpq.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gvyyifkpr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gtckqirmv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gghbaqhhs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gkidjvgqo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/geheeyfrf.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/glapovyvr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gmrnkdaum.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/ggenyvnce.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gskyhousu.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gbbgejvyb.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gkrztcrzv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gpcsdricd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/grpvzuzcc.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gawxtwfes.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gayrxztoo.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gjpudsnfn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/ggwxeuffg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gxsfjyuid.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gpzhqfidy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gtvdkzvvu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gmvhyxjtu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/guufzjtii.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gwwoqgdbb.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gzaxbfzpv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gearqetyq.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/geushcatl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geqtlxlqx.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gbvobjrmv.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gusxakzxy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gwyqpajaf.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gmnmkzrcx.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gmimvnkkw.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gnuleenzc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/greceebrz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gyerbqjls.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gbinlfxfe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gejccrqcc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/ggdfunrsz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gzgfuxdyf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gqhwvnsfk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gjpslmnxx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gdvaebygt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gvqpdaleg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/garetdirs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gzulwmlql.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyqdkzkpr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gneccgpxo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gnksinogf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gyalcvxbg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gwprflqdd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gduhhkvnf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gpzxwxwqg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gpybhrutq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gvqyiylyo.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gbtkjtecl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gkzhxywws.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gmbclkxkr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gvvxcuokz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/ggwhtxdnu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gxxzbkekn.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gezpaoacg.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gtqwnpsny.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gjflwtnmn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/giumrzhyt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/globjmhxe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/ghdihhpea.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gmbegxjcb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gccwvblcv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/giiirhnuj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gqqkgicxd.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/geustjqnn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gdzwcdsgw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gwwmyvspr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/giwcsgcxm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gndtqogtj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gtkwhlxag.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gzvgbxlnx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvbxgxtri.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gzpdyirgw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/grbhiyiyu.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/ghkdiqyvp.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gsjjtwmbz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gpvikwanh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gcrfyhofi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gvmiisvqi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gjibinyui.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gyyodzhom.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/grfitmvgm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gjpykntyq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gqfclbbxi.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gcwdiawdt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/ggzwnpede.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gqvfnwjqx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/ghoezdlws.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gniirvmii.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gtntyippg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gxzrnswvw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gdnmybdtt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gcktcdkzj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guzjvyoet.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/giyqiedrh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzwaomhrg.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gpykspgec.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/grreizbfh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/guibawlmu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gmccrqqki.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/giphlktxh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gfitlncyk.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/guhozwzcx.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gwwainljc.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/grzimptmy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gzbtkfrtj.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gvofzdcfy.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/grrkzruom.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gxvwpmgac.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/guzrktbpt.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gwpvruygt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gfljntyie.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gwhpcsnvl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gbfojsych.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gxkdyyxbl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gfioztzva.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gbyblfxzn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gkykybdho.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gbuqssocq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gahozdulk.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gthobhwnl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gexklfebo.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gqqnfpgvd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gaywaurcj.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gsatmhrzp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gukeyumoq.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gebtdmbyj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gqqaxxiks.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gngcxllym.sHtML


<!-- 参考信息 -->