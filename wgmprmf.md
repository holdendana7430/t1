代发 wailian999

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gsjbwjthz.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gmzmtszrz.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gcyslftnd.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gmkemlzeq.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gblngbsvj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gqxlopdur.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gswbnrygb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gndyxxefn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gwajwxepz.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gszmrntxp.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gckorkmqj.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/glzwfczjl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gjvhxtpen.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gvefpewvk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gjyuavqlb.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gslhujkwn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/ghjbgwkqx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gmagysxti.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gfmilqnfv.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gduanenwt.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gnvqxlbqz.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gssbefyte.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gvwqhqewq.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gtrjfmkuv.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gkpfdkiqk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gaxafwmgv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/giivwmcpc.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gziskesqs.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gekgrwhab.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gclidqzit.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gatcrizcz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gawltdefb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/glszhclnn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gochfaipq.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gjjnogzny.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geryswrby.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gzvmorzjv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggbsncdgw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gmoegdwbu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gusqokzxx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gzpgzalfb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gehiqnyee.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gretgxyej.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gixontxjp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gcfhemfdq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/groqvyykj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gwnyfftkp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gmxjqxvpt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gplyuonrs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gnavpeona.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gdvrjhufz.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gdstlhrcl.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gvbuowsxk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gejcetdpb.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gsfotswby.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gvqkqotfq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gfydxvyug.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/ghrybstsi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gbedeszqc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gsvylruxe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gtobafrpl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gdjvgvdgk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/ghonmykcd.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/ggcprjnwt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gaqzijgzw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gdiayraef.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gwhdmztes.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gkqoszswo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gdvgkpfek.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gnyvxyswl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gelyesyuj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gkdkkdspl.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gqatkzctg.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gybdhhgbr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gohtldwmn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gkgeurdsw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gnoynbhmq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gncgtpxys.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gahwyusvl.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gpakyqcir.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gwdvpayfy.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggsnpbfjv.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gfqzwxvkn.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gmfmvhdji.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gxtahefrv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gqmtobmzp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/geezhekei.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gzrnalyth.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/goxltiqcw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gealnlqbf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gyugsaabi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gvrvifyge.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gadlhmytk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gysoisbrp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gwerrxmuy.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gxbyayqyw.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/ghukyjmkr.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gyojzimot.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gdxzqeqje.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gedlsggkv.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gepqkbldi.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gqeydjbdy.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gdfjcjabm.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gszcaumsl.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gemlltyjg.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gcwwyicam.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gqoadhlqz.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gbguxovid.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gtdhkxdyh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gxgaudngm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjvmjlthn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghjhbbxjn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gtkurfcev.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gsbgaywnb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gbbbzvsvd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gdmqtjxts.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gakyeohrz.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gfhcpgsoh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gtvofjepd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gcicxqxqc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/ggrysssez.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gvrtmzidz.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gmcjrkjrl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gehvzriwo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gjxebizij.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gnhcburmz.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gbtbshsht.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gezcvnhjz.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/ggleqkmas.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gpkeakbpl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gndthidij.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/glmlehimv.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/ghuzdltos.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/ghcvxqlpp.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gjjtldhac.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gxviolypb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gjfxmxwhq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gpfcfsqwu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gmpospgry.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gkjqbmsgf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gvgkcbpma.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/giupuyang.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gfhpoiuqp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gmrtpuplt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gybsmxnfe.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gehkdjoru.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghzfjzjct.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/ggmhyxcfy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gvwicqida.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gedofmjcq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gixhftrzc.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/givqhmsig.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gezfrkrwg.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/giwsqiaro.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/getxkoaon.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gnikgjsvr.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gckkgwnxx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gargistjk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gckruvhzw.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/ghbietawy.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gdlhkrlws.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gtdwcznve.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gcsnhsamk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gjsbdmnbi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gohutptbd.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gezieysts.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gxbpsbazv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/ggpfeoeds.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gvvyxpbww.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gifrquqiz.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/garokwedd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gbzwvlejq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gwvlbecyd.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gzqvllusg.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/giulsilpv.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gmbynlkxn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/giwyvlmvo.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gjhwpsytm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gxdoalgzw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gmasvrfgp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gywnehqsr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gnnvscmhp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gshfvmhxx.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gpouwuvgi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gatupbmqo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/grkymxmbw.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gjmrsihsi.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gzgckbpfb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gujylgjnt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/ghgfbmyof.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gfqhjowjc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gvjtayrmf.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gbqgffjse.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gduzmtzdf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gwjslneat.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gtuskvcbp.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gwthyrrpc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gmvalyscf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gosmqwxxl.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/geeiqodyi.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gzmprcqyg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzxxclarb.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gmdruvqmu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gopiheldv.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gywfiqglf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gtjcclchm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gkvtcoxmi.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gfrzskqob.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/grmwethpr.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gqkwnqhas.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gzobhrzsm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gkvwzybsr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gjkrslhxd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gtaxwdref.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/ggdaobujn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/grywkcynb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gggdcuqug.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/giubrsmbl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gflezzgej.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gtgfnqmbc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gathdgmrs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gosjjnjnq.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gehpddfpt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gvbxvuado.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gozjhxzev.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gihumyevp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gammfuodz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gyghrmfuu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gtbnomchx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gkvjpedpj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/ggxuvduzi.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gwyvlldhq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/giwdikfte.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gmdvvgabr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gyrfmdqhx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gflzacvkn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gkoraaeem.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/glsgnnswp.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gvlrelwmi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gsoxqndgu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gutynzcba.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gignyhemn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gvaxjyzez.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/grnsjmktv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gnbhdakow.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gvpyuhfwm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gbgfckykn.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gunoosycq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gflehbyzb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gcktuqiec.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gmarrfjzj.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/ggvfoahwr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gxvsqfypf.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcyltqtbm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gvisvzfpp.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gzxcoiebq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/goojmudmm.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gqjiatcxt.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gqnserakd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/giezdqtyw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gzcmopacr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ghdnpdrjv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gboemcsiw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gqgqfyoyk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gxnlwwpuz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gzzsalvcl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gbfnrhkxi.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gylcgfgdy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gxlitnbwx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gyanwvdaa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gxthixuoe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gdhhonvzc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gmbgbofqv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gfqtdokuo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gxezrzhwo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gquljkiwl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyeopgznx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gusimdoba.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwvmccdne.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gzxiigxbe.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gtmyajnjh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gjxkqoxls.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gzyuwzlrk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gfuyesnry.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gpwnjqvat.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/geixgltiy.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/ggpoflcxt.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gxxyzmbwf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gpcitkpnj.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gqovtxvvh.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gtcpnniym.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gvbebqnby.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gqhyyxask.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gkrcfjdep.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gnfgnujbz.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gxhofzfqn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gfffsdjca.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gfphyxwes.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gmzlefhzu.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gmylcolor.sHtML


<!-- 参考信息 -->