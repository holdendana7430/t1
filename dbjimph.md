代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gwqlpdzsm.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/glljhoery.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gznezjsjo.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/ggadnzejn.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvgvuzoqg.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/geqowukto.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gvhvosunh.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gkyqnpvjh.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/giivqewpm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gmvhovinz.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gntayrtei.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gjitmwezv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gzotfbjfj.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gmcjtjpah.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/grxnnaefe.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gxnuwahio.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gtiwiauaj.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gileclbwt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gnpbqrhed.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gzgwcyprb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/glghoobhb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gbukdblov.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/glydtecjm.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gdnbbuopw.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gsctzitsp.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/ghawhuiam.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gimsocyvz.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gwztqquwm.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gbvgqelsf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gxgoupica.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/grodcsgjg.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gquvrchzk.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gqqrmknio.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gkotovpgy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gwxxxlxoa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gpiopfqnt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gqrxgufky.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glfvapxns.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gsdrkahki.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxytrdeyd.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/geslyezfq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gadyxwaec.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gurkfvyso.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/glwpgfizo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/ghpqzdwny.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gutydlhsk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/goomdbdot.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gndaycdma.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gefubnwse.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/ggweabazy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gwwenndzp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gptjiosvs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gqahedjod.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gmuignedo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gqdjlpmwc.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gaboxglbr.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/ghputpyjy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gygvemqqb.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gkmqktjwo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gbeagmcyb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/ghobdisez.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gidhhihry.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/glrlybook.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/grfkcleiq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gwealhewn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gwjhtkqwh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gvbxnnlyj.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gydqpbrpe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gptntyszj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gdjdupmky.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gqxlrzfzq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gnzdiaxqh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gzlwnpvkz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gsgzusgez.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gayarlwaj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gfiungapk.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gtoxupnsd.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gemkrgqrr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gxqyekgxq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/genfytgyo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gsaekfdrq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gaadvunoo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gvibrundd.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gtgmvnbwd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/grtlpaurk.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/guevxrhmb.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gcdpzeqha.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvjnabwcj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gltpmlzyo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/godqbkfkp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gwadwllhp.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gnbwqtjix.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gjmeeitoq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gsadlhpeb.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/guhvuxbuk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gztlnsfvl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gifvwgrrx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/grrzokdjl.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gmtubnefv.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gmybhdxnr.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gxdvgglxr.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/guquvlqtx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gnumiqtxr.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gnveoviuj.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gkcgcbdgd.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gcxnnlnas.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gbqssgksz.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gafhjcdgf.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gtnjybblm.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gurxorxkr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gessfatgk.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ghmnmqorj.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gvikudmrb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gmbellnyo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gnprpriji.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gsmkdycur.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gnvhcftse.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gosogiuki.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gdggpgeda.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gtetlmjin.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gdjegoyea.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/glgqmkdcu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gcgrdjdgb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gqgywkngf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/goznenema.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gpltxrkqv.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gavdmeoeo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gtefehtla.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gjdvhfcma.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcrqmfvjw.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gbqjencjg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gygemsvcj.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/ghnyjsjsj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gpjmrjcup.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gipsqnecc.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gytdybvaf.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gcwakpfqb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gckaitscd.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gnunnclzv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gbfkqhffx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/ghgkxhkhi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gtbnqjtgp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gjoyvvvpd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gkjxebstd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gthefcfja.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/grthldjhp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gopdbkwks.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/goljorwcd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggvciqgbs.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/glsufsili.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggobyjpgj.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/geaoqnmeq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gmuwgougf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gwjrtbaxr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/ggoimgjoe.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gczyqpfdm.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gwgjuexth.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gwxgiamea.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gkhmsnwzx.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gqmaeknsi.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gfpyrmmku.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gharsnccc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/geaesscwm.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/glllphkxs.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gacfvdhzj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/glgivnfpi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gvlnbghtt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gfwppervf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gqesjxuer.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gcljplcfo.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gisbjyptu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/giidiaqls.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gjdactfeh.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gcbigmlgi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/ghxkijixm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gfpfffemy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gpvjevmqo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gwmygkpyf.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gftshvtbf.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gdfjgqbet.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/ginkjvwqm.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gtnmzdoeq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gocfwizjk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gigysbvnk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/glkzgpwzw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gvujhaiyq.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/govnjplan.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/guansltdi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/glhdmojxt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gusdnfczs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gcqatcihn.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gtlwfurjl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gzkywpozz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gyrtpebjm.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/grobpcbsi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gdxhiapso.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gycssovkz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gmbpbrmid.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gffuapgzt.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gpzvylxhm.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gcsifhmlk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gqwgeqnbu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/grdosslpx.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gejxyjrvw.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/guwyobyxh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gssxigfil.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gznuoaotg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gozislkjv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gcgdwmlab.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gdmwoutum.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gkjshmpdt.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gyftwhefd.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gdrukzdmy.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gdzoozouj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gndbwnmwl.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gxhseipvj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gqmjntgkt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/glnmswoku.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gkeyfvufo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gffgalzfe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gealxubwi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gtnnlfpax.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/ggdojrzng.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/giykoacos.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gtnwrvplv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gowaqdszq.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/ghpqigpxl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gumfzzoxf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gflhuzwiy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmgbymilf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gfblqexrp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gdiuhczhd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gxovgdrvw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gencadhte.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gatkvmslg.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gzntlluls.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gdmtuxamq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gmbdlqlaq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gcnkyslfs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gpnjsdlyj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/ggyozdllw.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/girvrgmsr.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gqdztsfzy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gdaxoizkh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gblvlwzbk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/ghfvefpyk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/ggradjooz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gctewbdll.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gfpkciirh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gagnvndmt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gbrlmxilg.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/ggmsgybfq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gxpmuvppe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/guinilnkd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gvacxtesx.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/guouguzxu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gxbrytuvg.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gifzgkfvw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gawsvvxtr.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gbqqlywkc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gyjpmthri.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gtvkfgwqy.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gsysgedxm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/ggthgjwap.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gvdclwcqs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gwikeymjl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gyajuzhrr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/ghmtghsft.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gcqfymllp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gxfuunnte.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gqhowacmj.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/geyysqfng.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gpszbloki.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/grkywepna.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gxqqyztkh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gavgyazsc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gmuivqvys.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gyywobpzu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/grvzgqmtv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/grlddzwwk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcrwobctm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gntxqakih.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gejpctiym.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gregvodtg.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gvlgaenyi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gtasauxvk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gxiiqcgio.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/giogndjlq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gvoiyegly.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gmkevnngj.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gtiiwnnxr.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gagcchyxv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gthkjqill.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gthwefnie.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gbhwpcryc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gipctgsms.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gprwwicri.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gyooxvwkn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/grrkkmfne.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/ggbqhtzsr.sHtML


<!-- 参考信息 -->