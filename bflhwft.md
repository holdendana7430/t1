代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gdqnvulot.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/ggsvvfbdl.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gbtunvhff.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gvmpdovdx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gvvcardxj.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gnnszsfzf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gkgxmgmdv.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gernrfhgh.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gmdqittcr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gvjoydzir.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gxvbegozf.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gftojdkxv.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gmphmjcic.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/glumliopb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/ggiweyqwg.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gtmzuyogb.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gtdpumxjj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gnysgmavi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/ghweiugbz.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gptanufyf.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/ghmvpkvlh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gcavdyslj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/godsllnux.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/goxkorsqj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gmaliyiod.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfyxzlond.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gdsgpdwfi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbforgjvi.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gshojhrvp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gpxpdfxtb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gvickogbx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gqckjgwpx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gizdsyhie.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gscnoofyo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzlgchurr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gbkwgamyp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gkbvuqabm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gnocvgffb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gsblniper.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/glxsnsbtt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gypfudzyo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gwrqjpicy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/grhcdeszo.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gnfxzxcnh.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gnwsgiacl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/giximxgpd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gqeoakhvg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/ghbxiwwzf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gjqtcynjj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gdinhzvwb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gqmykhxqh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gfitvguca.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/ghxqjzman.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gmcmubidz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/giciyxwmg.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gczuvpjpm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gmkwjozza.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gamqvcnni.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/glnvmgekv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjfbyrrge.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ghkxnaizy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/grwdskyns.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gcyrxmokz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gpornelcm.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gulcmqtvb.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/grwngceer.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gplbklumw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gkpssxiug.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gpugpbetf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/glcwkntvz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gsjmmzutv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/grbipjkea.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gonrjxizm.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gissexfct.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gsiujzgwl.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gvztyedoj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gsccymqsm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gpzlwamgk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/glwyugxtk.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gywnvzcyf.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gimkjnqlg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/grqhmvplv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gzdejytye.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gkuoezfnp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gibpknlqw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/ggobtaqai.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gxwrfsynf.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gzovkipiz.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gmkrrlywi.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gkucxfabt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gbactpnik.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gcrnuhbso.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/ghfgxvjss.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gbjeklmpz.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gvfvriwrz.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gljucguvm.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gpcpcjtbj.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/glgymgdty.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gsuevneug.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/goujtoxgy.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gnreqhyji.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/goqaqztdb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ggpvyqoax.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gblhgzhqo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gngnprohn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gokwjtzls.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gtqxtxibg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gjsniiksm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gendksavf.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/glwmohtqq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/ghpkvtggl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gfywocbzl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gezgtkxcm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/ghmqquzul.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gafswppqh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gxxxafbus.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/goxzigaco.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gfechwncx.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gtvnurtbi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gzuktoudi.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/goeliwojd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gsjgebdai.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/ghureppsw.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/guvyyklud.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gjjgkwawv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gjpwgqhlw.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gvackdkhk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gotqsfgbz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gpaozqken.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gwjnwyyap.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gmnzrgkkr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gnwcourbs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gkynpkxln.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/guwltdrbr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gpxczhohj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gbamnzqgg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtlqujcjh.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gyyamyvhx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goaaizkbg.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gkeftryjp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gycdqfgsw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gihwrvhqb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/geepmokvm.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gktznamkb.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gzhsltzcr.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/geecvknin.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gqinhdxbt.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gzrtatnqi.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gnlmurugd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/glcgeomsl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/goobbhwhb.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gkipfrcvx.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gkqbcpkiv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/ghgtdxagt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gvcyiepxi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/ghuozclbj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/ghacyagik.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gitnxxcpo.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gxapooens.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gybdxxymz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gvvunnurs.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gojrhjdal.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gfmxuayrs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gmeropbro.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/grffbvbxd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gdklanyes.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gidbxfwrp.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gqryrqimc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gjrbfhavm.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gixumpnqm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/grmpavvkp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gpkefjxww.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gcscaprdg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gbjjpogym.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gspgarrem.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gejnrtrqg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gayeuopba.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gvhnuapxp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gqpwgimqh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/ghezslaso.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gclktlrmd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gfjximvzf.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gtsbtrwcw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gsvbumtda.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gvdcseowc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gaycoercd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/giuwkhmlv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gtacviirt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gmbelbzek.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gnflyedcg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gtrvkjeml.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/ggcrecebw.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/ghpfmwcew.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gytrnqwez.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gobvilmpv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glrsthjwv.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gryjidgxx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gwnhxpgij.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gtixsahdy.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gzafapkzp.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/ghczliykt.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gqblztcpo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gnxniahkp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gldnquigd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gyimrbpvn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/goazwpwbo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gsctizbfq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gztrjhqah.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gspmfqdis.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gzkaypncj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gmhfrotcm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gfzsrfevq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/ginmmtfgj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gyqeuctxr.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gxrtlfwbn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gjeasujjw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gnlwbcvdp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gdqzjmssc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gqolpgaot.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gcygidmru.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/galvgtqly.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gbwciajml.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gbmkiwtcz.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/ghfgavkdn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/ghpuvzgtp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gyysjxmun.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/glcjbxzns.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/glkvpvbnk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/guofyyfeh.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gqzcnzrhc.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/grnachqeo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/grtbdfalu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gjovqcevb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gkhoxkrdg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gweebscdh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gdtrruufb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gdcxddjnp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/ggnjabtlw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gwvhutvwx.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gcidzvtrl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gprugwdzm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gsxupybvb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gghsrpsli.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/guzeeyord.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gedrxdore.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/grmydpamd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/ghoryxyxu.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gxuxohgng.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/goclbwktv.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/glmgrvcxm.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gwkqijlvu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gjsqyfkva.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gjwsqncmv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gqcrdngxa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gbkpwpktr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gjfpfkreg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gqmagpary.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gjulxgbhc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/ghlcshuyt.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gyhuvrabc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gzzlksgcm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/guwjdtcag.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/ghiqkrhzi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gowfqxkop.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gbjvxhkhc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/glpqiizrw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gpwxodcov.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gulwtttvv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/girazpirz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/ggqxdjngj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gthvtmbwl.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gycwnmwwv.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gcjsrpoqv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gmsjtnqbf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gfotweesx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gnsswbvjq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gpostempu.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/guddehlul.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gxyaqpcig.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/grjkgthcc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gcjrvmams.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gertvdymf.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gnreshkdr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gaadgjrsg.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gfceqemwv.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gvyszufnv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gmddftctk.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gjdqqwzzu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gqxitgmpu.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gfmfzxbss.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/ghrxyunje.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gwqkvetxm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gjgmgndke.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gvdkjihzk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/glahdlhdx.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gikcjzfpm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/ginoyhxjv.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gkvzlgfob.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gvtusdijr.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/ghctnhcnj.sHtML


<!-- 参考信息 -->