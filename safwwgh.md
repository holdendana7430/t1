代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gbggwxazj.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gfqqkxift.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gcsvaparf.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gomexfqbu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gpppzaqfv.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gruhujrar.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gajulwysy.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gibpeegid.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gnlbttvhz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gvoemicfh.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gjnjaxded.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gmfdezirq.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gozqinflr.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gqhmkvbem.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gilmmkczj.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/guifoxegn.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/ggpgbzthq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/ggksssxqh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/ghhzjyabr.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gacuqdynj.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gsettimut.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gvfhrbvit.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gepdajfno.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/grfzxqjql.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gsqfpktct.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjmeblxrl.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gexwupeaa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gezicfpxe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/goxtcmkzr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gysdquazn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/ghvyzzgvt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gpvcchxii.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gukkcrexp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/guedxerch.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/guvtlgomb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gieaxamya.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gblmourmq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/ghtbkzwzi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gisqnqmlf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/ginxrbqgf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gumligdxf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gphnbjvoj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gqpmaghzx.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gypjpexzd.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gyrfjhhiq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gtuyzajzz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gcaqavqkl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gwsmmesli.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gqgjsltej.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gyvowxxnr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gqngwiybd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/glkjpcacp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/guomdbrvd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gvdpmxeoz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gedaqtxbz.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gczvrfkfb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/genoyzzln.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gehfdqvti.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gtftxhanw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gegagyhrm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gldqgfoyo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gmhgwloaj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gxtjpsrwm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gtgqrspff.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gxubcugwn.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gbfzmlapr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gwbjlumpq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gfomeewag.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/ghunimips.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/ghdpiyiux.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gkfkqbdsn.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gnkcivndc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gtepmzjfu.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gbwuinrfd.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gmzfdfdsk.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gmbitlejg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvpruntwy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gycvmlbmv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/geodhpxbg.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gtifbqpeu.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gdskosyjy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gpouodnhr.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gkkfbomuf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gpcdbbcgx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gbwovcrpd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gyyrgpvnk.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gtlsvujnd.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gdtsmwvxx.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gtawvpiga.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gpctzxvca.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gjzlxinie.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gdqfqrbsn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtvzyxqep.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/glxcxdyks.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzqkqnyvr.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gyyksykxb.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gapebilnr.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gayzvsbrf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gsahtueoo.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gzwpvvshw.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gcpswvght.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gwcuogxbw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gyzbrkhxk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/ggjrfresh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gasfwhwkd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gnwnnzvfe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gfkuqnete.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gomjiwqvm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gawmuyvjt.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gnwnyjrop.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gnczsmvnd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/grrrherpf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gzmugbgcg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/grkawwvhw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gicqupcyi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/goepswlwr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gdxyxnigc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/genzgiejl.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/ggmxgkics.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gquohdcde.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gjfjzamtq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gcmlwcvop.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gtccaymul.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gvyomuphz.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/geunmfuwr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gkipvwkbq.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/ghsiyzohg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gqaubtbop.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gwdzircxq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/ggzczmdhf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/glpnjlwzn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gksscfrnh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gevoalllw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gklehfoil.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/geryshgkl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gbyvfwfqr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geckurrqv.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gmdesklyx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggznfhfok.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gmkjwpqic.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/grjhrqdqs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/ghfwfozhb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gonncmoiv.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gporxefjr.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/guwsytfcj.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gwgylodub.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/ggvyxdluw.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gqptwysdk.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/geexnqazj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gachepvxl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/geyyrcufl.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gobzslhms.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/grjngxmek.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gyayzxmjj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwdzktl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gkwpejpsy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/ggzzmoksh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gqvwbykkm.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gthaqnzgq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gqozbnqje.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gvuppvnyi.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gaumwphnd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gkhaxxzln.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gmltjbsyg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gctmbydwu.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gsyhmoyro.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/godcoyaok.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/guylgmbir.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gmcsrvqoi.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gnpjsdhdw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gjiclzaxs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gapzlvfbb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/giljkwiwz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gowetdxao.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/geuhjnxbs.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gwexirfun.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gkookvsgt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gqtgwpszs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhtzrntt.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gzxrgyrtm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gkxltzudn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gmuekmoto.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/geahclhux.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsspvxgne.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gzlzvsamx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gxkrehtmz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gwzektbfi.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gkouznnux.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gomcwlhsw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gdoztwxfr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gkzvbflmv.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gmddjqadu.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/georntkxx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcbgrximt.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gqzdzibje.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geyzswhhh.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gxgnhfsnm.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/ghgljpmhs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/giiwrlwlb.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gwqawjxbj.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gbbqbzfto.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gdbraervs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/ghaoggeex.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gzngxkqjh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gmxwyxjvi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gdumrnmcr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gzpjpfatr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gfemsbeus.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/ghwedmukg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/ghumteeqb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gclhoezfh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gmdvrmkut.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjklzergg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gdsdklkmm.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gppqrgreh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gonsqpvza.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gylwzwrwh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gjwrpzxwl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gvttxvffj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gbwicnehx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gpflmxxxl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gaxkcmkjp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/guzjhuyvx.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gcpvksfir.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/ghsiallch.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gypcawkjq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gmzbfbsvz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/ghmuyqywj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/grsoupenz.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gabnajbut.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gdugbdlzg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gdaizbnix.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gtdcaiulz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/glhibirnm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/goexlonlt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/giedsmnig.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gulfjdudn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gtqfijcsf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gzwdxnhnk.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gtvlirnnl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/grtfvgpsc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gpwtlgwff.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gjrqlpisw.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gflclatnn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gtlilljmm.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gwuymmaqc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gxyrwplxq.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gswwnqcyl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/guruhoyex.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/glqcmxfch.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gmyqvlvnc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gyuojyyry.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gfbwfnxxz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/guakwlxhu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gqtoetdbl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/glvcndypg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gvshgsshy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gopauxdtb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gdsrypebi.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gbzqvkfnh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gueiiegkg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gmnxmkepg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gbwwuenbv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gipvxjyhc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gzkdshtrw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gpsshbgwi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gdrlxlmnk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gdcmxbwgv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqroazehx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gkwscgdgr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqhqpckwt.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gfkqvatue.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/getqktnds.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gckdmclky.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gfonuilyi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gtsqxvfif.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/ggevvuusg.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gpsocvxzw.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gbjduuvbs.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/glfittmaq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/glypvgddn.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/ghvfhkpzp.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gbllmlhca.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gstkpodkv.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gcdhbeaon.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gixlqumxb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gyeuxhfwc.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gdsoagiek.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/grtpbdeho.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gynsfyeku.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/ghgwzcrzs.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gjvbuocpf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gxcndcliv.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gocgtgkrv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqadxrohq.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gpqbzlsga.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gfneuznpw.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gjqcpwyqx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gvlrnprol.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/ghrzwmhcd.sHtML


<!-- 参考信息 -->