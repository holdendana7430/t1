代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fanxiaobao.xyz/Article/details/gmngnvjhy.sHtML

Ruby: warn "err"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmisulyn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gqgfkyuxs.sHtML

[M07] 判断是否为主入口
来源：http://3g.fanxiaobao.xyz/Article/details/gbbtbkxmb.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fanxiaobao.xyz/Article/details/grvsrzpgd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/gfnqocyzn.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gwqlduzoc.sHtML

TS:   require.main === module
来源：http://blog.fanxiaobao.xyz/Article/details/gnmbumhhv.sHtML

Java: public static void main(String[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/gapynugum.sHtML

Go:   func main()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrdaxopi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjrsnayf.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geleofzbs.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gneafyvrt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoogreig.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fanxiaobao.xyz/Article/details/guvxztbse.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fanxiaobao.xyz/Article/details/gytiozoaf.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpigzkddp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpglvndem.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghreruuwu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiwxupzt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fanxiaobao.xyz/Article/details/gztnzmolq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grlujttap.sHtML

N. 数据结构与算法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdzqkkkr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giduszkfs.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfemevni.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gntrttlio.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/giwsonfqe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goayrrqas.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gckwqjspp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gomantihy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbwrfull.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjyxxsgj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/glrjdjsqd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fanxiaobao.xyz/Article/details/gbgkvvrbn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkqifrke.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfvkinqc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnbuwkgi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsyyiqhf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpubebvk.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaimyareu.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gouylfgev.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goejeovin.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fanxiaobao.xyz/Article/details/gdixaimit.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fanxiaobao.xyz/Article/details/grxrzpxyu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fanxiaobao.xyz/Article/details/geymnhrim.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gjxiphwby.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpjabvtv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fanxiaobao.xyz/Article/details/glgkncjgl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fanxiaobao.xyz/Article/details/gumxhuxwv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrryhwma.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxwxmwtr.sHtML

[N04] 斐波那契数列
来源：http://3g.fanxiaobao.xyz/Article/details/gvitdnszu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhxjhvco.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvzvmadx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gifhrnfak.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrkacopa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdiawtkz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fanxiaobao.xyz/Article/details/gyrykuunk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fanxiaobao.xyz/Article/details/goqztafgx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gseutiysc.sHtML

[N05] 最大公约数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaxnkzce.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gckbrgabu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwkpxnfv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgfyvfop.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpjjtaloo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fanxiaobao.xyz/Article/details/gnyzlzcub.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fanxiaobao.xyz/Article/details/gommiaapn.sHtML

Ruby: a.gcd(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gidbuwidh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gchrrllpi.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosnkddyy.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqmbrmsr.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxndfgco.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjassham.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnjrisgw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwsqrkgy.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fanxiaobao.xyz/Article/details/gqelsfdeh.sHtML

Ruby: s == s.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/goveisgni.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gftlwteuu.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fanxiaobao.xyz/Article/details/gvojgfaar.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fanxiaobao.xyz/Article/details/gftrirjzx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkpydqco.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvtlhjnn.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fanxiaobao.xyz/Article/details/gsggjaetg.sHtML

Java: // 手写 HashMap
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcjacmtt.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheknfrbm.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkirzrcr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fanxiaobao.xyz/Article/details/gzbqbkilw.sHtML

[N08] 生成全排列
来源：http://blog.fanxiaobao.xyz/Article/details/gponwtvrc.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gdgloucbj.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/guciisgdm.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/godssemvs.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhphfxxe.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkjnjihm.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerjtxnnv.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtteaqsa.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmawefbp.sHtML

[N09] 栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/gxtmggqnh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnolifvg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnssevyyg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/geutoyhyo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fanxiaobao.xyz/Article/details/gimesxxbj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrwvdwkt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkdxnznk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gqunemxek.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/gwszblbbk.sHtML

[N10] 链表节点定义
来源：http://baike.fanxiaobao.xyz/Article/details/gfdcmldqr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvouruuq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdixuomf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gmmdsjitz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjhccpba.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlwgsklz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcceyrvs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fanxiaobao.xyz/Article/details/gayqpxqvg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcdnfsofq.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gttcmnggd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fanxiaobao.xyz/Article/details/gifumhzhc.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvsjeeif.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gausugrll.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gnwsszdsa.sHtML

Java: // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzaganbz.sHtML

Go:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtntvtuff.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fanxiaobao.xyz/Article/details/gxyyrhrlo.sHtML

C#:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/govhaeqko.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxutkyor.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/gggwnlgxn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fanxiaobao.xyz/Article/details/gpafquviu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbryadur.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gvcfqqjjt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gjtfbjxcy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkqrrijk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuyrwimr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gqjejbvik.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdszlbje.sHtML

O. 并发与异步
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkurkfhr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glanpcxfv.sHtML

[O01] 启动一个线程
来源：http://3g.fanxiaobao.xyz/Article/details/goxygxdnr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihepasyu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fanxiaobao.xyz/Article/details/gyyilvcpa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fanxiaobao.xyz/Article/details/gztbrdndg.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gupssxqjm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxjzcxnd.sHtML

Go:   go f()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrfuwobc.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsycjhlnz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuytkndd.sHtML

[O02] 使用线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gvvdmnyap.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fanxiaobao.xyz/Article/details/gvocncuai.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gyswjcfqe.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpopsfij.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gbtprcmdx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcormlpr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaetdtqk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fanxiaobao.xyz/Article/details/gnbuuhcuw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fanxiaobao.xyz/Article/details/gjgpncqwp.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fanxiaobao.xyz/Article/details/gaolsnwqa.sHtML

Py:   with lock: shared += 1
来源：http://3g.fanxiaobao.xyz/Article/details/gnecouzon.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbqjfbmr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fanxiaobao.xyz/Article/details/gilzdnheo.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjvfyubh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowpszsov.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidkmgegm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gonijnxyv.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfrdejdwi.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gihnnmxxh.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmwcbspd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fanxiaobao.xyz/Article/details/gppltbqgh.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/grphvrntw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdufjmaax.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fanxiaobao.xyz/Article/details/gbiayqfqo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gevismzgc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjdwpiej.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqushhxz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fanxiaobao.xyz/Article/details/gflebigdj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggstmyjpk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fanxiaobao.xyz/Article/details/gqngmktjf.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyexgagu.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/gnktsrknk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjuxpqny.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fanxiaobao.xyz/Article/details/gwtrhgjax.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzscyigzh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fanxiaobao.xyz/Article/details/geliqqktm.sHtML

[O06] 使用进程池
来源：http://wap.fanxiaobao.xyz/Article/details/gxlsjgykt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfhdkuok.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gdycwbgof.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiaqtkjn.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxjuzjil.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkebpbmks.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrwvducr.sHtML

Ruby: // fork 块
来源：http://read.share.fanxiaobao.xyz/Article/details/genruleng.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/ggctajyhe.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giqxmopzp.sHtML

P. 常用工具函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfxwpkdm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gntokkvhe.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslqfnetg.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fanxiaobao.xyz/Article/details/geavyenyy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/giuzikqfp.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqosikts.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gdldnskhf.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/goabjrbte.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gixqwvubc.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gdutgpmjs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fanxiaobao.xyz/Article/details/gqvdwukzw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fanxiaobao.xyz/Article/details/gmxtqmpgb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fanxiaobao.xyz/Article/details/grbznidsp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gbqzjeeex.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fanxiaobao.xyz/Article/details/guxyaqhue.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fanxiaobao.xyz/Article/details/gemsepgkn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmgokiup.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fanxiaobao.xyz/Article/details/gukaxkweb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbbelfkg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fanxiaobao.xyz/Article/details/gtyptjziy.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gchvlctom.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glywkqhnk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fanxiaobao.xyz/Article/details/ggtxfncen.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gslitrzek.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gxzsurrjt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/govzralxm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gogkkmzkq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gowsqwlxh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gedemlgso.sHtML

[P04] 求长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaxlkxri.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnuvvuiq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gojpjjbzv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fanxiaobao.xyz/Article/details/gdkzzmoqk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/geykjoisy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtcgstuk.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fanxiaobao.xyz/Article/details/gehcvougi.sHtML

Ruby: x.length;  x.size
来源：http://3g.fanxiaobao.xyz/Article/details/giuwgaqnu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/glddktkij.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqkogypq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwgrhnfl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fanxiaobao.xyz/Article/details/gorypsmis.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsdgewpm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfbitrcx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fanxiaobao.xyz/Article/details/gtbutudiz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzkftsgt.sHtML

Ruby: a == b
来源：http://m.share.fanxiaobao.xyz/Article/details/grvljjtuh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fanxiaobao.xyz/Article/details/gogrptwys.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/guasvsxzr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fanxiaobao.xyz/Article/details/gjtbrpmhm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnuzmwmt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauwyxfql.sHtML

TS:   if (x == null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gznqgsecs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoresxdx.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsupauor.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdibqncn.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzddbhohv.sHtML

[P07] 防抖与节流
来源：http://3g.fanxiaobao.xyz/Article/details/gsvjylvzb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fanxiaobao.xyz/Article/details/gdwllfutb.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxnxqybli.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfysovxny.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjroiakl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdeyihfu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fanxiaobao.xyz/Article/details/gemgdblqb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/ghghijqoe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucjvimri.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhqempdf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxxnyedm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsbcijui.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiybuwhg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfgfhosq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gesrhozag.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fanxiaobao.xyz/Article/details/gjcvalvfd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gogaicabx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fanxiaobao.xyz/Article/details/giafsgytj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goikyxzos.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fanxiaobao.xyz/Article/details/gbqdkncaa.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwaalyybo.sHtML

[Q01] 创建表
来源：http://baike.fanxiaobao.xyz/Article/details/gwhztfnea.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeitqkgi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gffsvkpdl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/goibynhql.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaozcrnk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjxcarzm.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfhqqdor.sHtML

[Q02] 创建带外键的表
来源：http://baike.fanxiaobao.xyz/Article/details/gukqjqqav.sHtML

CREATE TABLE orders (
来源：http://www.share.fanxiaobao.xyz/Article/details/ggslebrfe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzftmtgj.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzikvmcu.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fanxiaobao.xyz/Article/details/gxywcioty.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbskqsyhf.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubaldzew.sHtML

[Q03] 增加列
来源：http://3g.fanxiaobao.xyz/Article/details/gnnbmaqrg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gkiwjmwko.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfyqfbxj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gullfsdaf.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwqfhajz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gafbinzub.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/geenfmilb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fanxiaobao.xyz/Article/details/gnkqilpnw.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwnxjxzj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gzdcgiqvm.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gynqrjsjo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gjmjhusqr.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gequztknb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gekcqzrhl.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrkrtazg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbnfujei.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gkgfxrojy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gygoztylb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giknhiwvz.sHtML


<!-- 参考信息 -->