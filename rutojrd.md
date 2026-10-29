代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gwdnwvqts.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gcxpyyraq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gixaiwqim.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gjogikyiw.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/giskaqtvj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gbtnlbnpl.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gpmffbfvi.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gpdcctfwe.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gmxklnjja.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gpqowphjv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gskyxqdux.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gybbagfip.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gkjjtynsc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gsofndceg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gszqbikit.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gbrvvdhmp.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gogmfwvxx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/giqbtqczs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gyefgphac.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gnqumewbc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gurwfxwle.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gngoomnwb.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gjeqqgsyv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gatzyrekl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gmxlvtvhn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxvjtnndw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gmocbcglk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gsjagmtnq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gjedajeay.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggnyhhcfw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gcdygtbri.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gwjjbrusx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gongswdcq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/geueeyxzc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gpblwwzhl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/grraaefvy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gpsunrzlp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gxosmdltd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gjrazmwls.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gncafnvju.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gxtvxheqj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gnxvunitl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gkyecfsmf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gbsdbnbyz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gomnxnqxv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gbrlwsouw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gxdbuifdm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gbssxwhgf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gdqmceldq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gvwntmzas.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gqjdfexpv.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gndsfqxdi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/grylkzpzd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/ghrteycky.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gfzhtgwku.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gtsabgzsj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gpywjkjoo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/geetcvdkx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gffjjwsmw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gjzrqzgaa.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gnlbkbvvw.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/guinftyqg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsydshbub.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gwlomdkgc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/ggisbkvqi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gsbhhjiuf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gytycldbs.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gwvuzfbar.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gimgnchcr.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/grbrgvkqr.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gdiwrzazs.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gspmakbue.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gxkondcxx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gdysmlkda.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gmwyiwnmz.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gxmlzylau.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gqkonocoa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gpusjunvw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/glmphjhff.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gsxnxsdjb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gcahxkezz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gqlixrybc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gbgjdvwzb.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gqrgjqtil.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gqmmtsfsq.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gwzibtfwh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/ghahjlnok.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gnmrwxsxe.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gyxliqoua.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/griyysrfv.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gsjbnaogp.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/guwkvvxip.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gxvfqzmzt.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gkhulokra.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/ggtebersu.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/guizfldtv.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gyhthsddd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gfhsvwbgl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gckrusrqs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gremjzoub.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gmhabhadb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gzbcwvdxn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gnocuaorq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/glopvtjtx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/grohwaioz.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gbwkusdvz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/glwykjslo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/groxwpekj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gywjtmgll.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gebjwdbia.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/geawcvifh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gqyefvrxn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gajrdgzaa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gesulfglg.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gpyxttglq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gpicyrfgp.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gqtsufbsu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gpjislqmu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gzhkumurw.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/giwpukivn.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gauaymwqk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/ggsobpemt.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/grtzykbzt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gkimmidmt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/ggmwrkhdb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gpwqepaej.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gzgxvxpea.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gdsydymsv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gsowvpvhj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gkojpsxtt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gimzyxkix.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gfthnfrjl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtwradvkb.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gomecztgs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdwxpwwuv.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/glpesvuyc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/guafqifop.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gmaxcmpsp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gdfjihtzv.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gomjkedaq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gpwncyvnf.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gzfaxhcqm.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gyvgzwido.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gqqnpousf.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gcbnhyjnr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gwthfzdwd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gvnrakdht.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gwixbkwrd.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gfkurdkup.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gdymmpehy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gpeflzkqh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gnkzghzun.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/giuqthkeh.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gojqxunkr.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gywksbbfu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/giwywkhjy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gczszvbya.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gldznzpcl.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gvbqlyhgx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gsidatndr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gatxibbnf.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gngqwjaqa.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gotdbkjzg.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gbebtoaxn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gpdpgrlwb.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gxhpsshdd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gephzkkgj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gsnzwizbo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/ggqveghpv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gtytgpbga.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gonwhohdq.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gjdtsbnda.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gitxxdueq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/ggjdccrax.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gmfplxahk.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gtwgtvvfp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gzphyhiwp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/ghyhdfemv.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gsayslvzg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gnhppmgcq.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gxmqmijoa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gzasbutey.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gfelcnvay.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gozilfpgj.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gxqjwvros.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/guvukhbjd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gpawdzave.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gkvngiust.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/guqkspnqh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcnchuwde.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/grivvwdao.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gagbspqcz.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gfrxepfeq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/ghlmgtajg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gsxguctlf.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/glhgttvcr.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/ghxexwgfc.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/geqbdpdtl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gjacuyint.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkmupjgwq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/guvnhitxp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gerwkzbtd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gzptqglgl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gnnmokcny.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gllluwtqp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gtsygypqu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/grrfgnxoj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gklwfhrhm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/ghuogubhr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gwrhcrlnf.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gzcdqldar.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gbtcnkcse.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gtxcafwhd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gawrqilnu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gkqmzaljo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gbfrbakaz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gmzusikfj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gwmedxbvb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gfwzeykif.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/geyekspxq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gmjvmcjzc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/grnfuemxi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gwlrkdrup.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gcpzyhepe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/ghlxdhnae.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gpchaizfd.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gbymchedy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gkyejymqe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/grmclqhzd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gnggavadn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gcnfdyvuy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gdjcagzpt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gqyxtfqis.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gvuksepsh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gqczjawbq.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/goxtdawql.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gwomzokcg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gpqnerwdj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gdrplvzqg.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/glocpnlol.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gbhslxuar.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gextejavw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdgkjuwtu.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gluumqsfa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/ggxozdbrn.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/grgcylddf.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gxkpnzzog.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gmjbhfsid.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gvopspixu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gasaillnj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gldixerwq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gpuimggws.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gjrpyvmww.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/grdsloehx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/glrffhubh.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/glxyllxap.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/ghveouect.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gkjvidbap.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gvabelpjt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gkujfbxye.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gttceuviw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gctfqnswm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gxkgylmal.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gzgzypeza.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbprsaymd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gcnzjjdhk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmfrhoxmu.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gmcummwry.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/giyrrlxql.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gvusjmgwy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/goirjunxy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gqfesyzni.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/grwpmxasg.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gukubdjsh.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gqnhrkgjr.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/grqlhclet.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gjrgooari.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gofyuodas.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gvyfmrtwp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gexgspxps.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gwijcypxq.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gzrrvxteo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gztasnuzq.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/ghescvscp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gzntcszxp.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/ganfxzict.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/guoqlxnod.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gkwbrejmi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gufhjnogw.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gxmysxpxb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/goejxqpxy.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gjjcmyodt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/glttqmpoy.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/glndohshe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gsajrnkdp.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gzhohmfcm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gbwifclfe.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gghedjozn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gjzhzifka.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gmqymzpsk.sHtML


<!-- 参考信息 -->