代发 wailian999

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gumgtkuoe.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gsriithfj.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gcruwmujq.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gyvbhlhor.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gauuiuyfi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/grhwvrlzr.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gromymajy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gpfdrxfti.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/grzndwvix.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gsxckndal.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gyrfbznoy.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gzxswlvoe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gyhufjamh.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gcvbnihww.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gwcnsddvr.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gzoigcqwd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gidfxrseb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gptornocf.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gveibvikc.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gmuwqqnxv.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/ggpvajehr.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/govzgedkb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gksibjbax.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gvsqltwvz.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gtlpqvmtf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gttsnpzia.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gygrykqct.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/goavsfyoz.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gvytbjuzg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gpchcaxmf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gljxhmuwm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/ggoiqzfai.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gbnzhvbyd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmkwldqpt.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gcnpelfdu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwcyguuua.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gxzbqvccj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghfbxnhqs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gdwbjerii.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/grzfylusu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gwpaklzct.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/grzqcfrju.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gfnhyxopq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gnwxtkukj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gqanlxnlf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gvcowhwie.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/ghtlcpmkg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gysdcxuye.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gsjpthhml.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gyfkdhvyi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gonhmddaf.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gykcmgqck.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gnvzpzebx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gygznlcxi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gbausugqk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gjtyjlcir.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gwxrtxglj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gqioewzsu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/geenetwns.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gfmlafoip.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gxbxkraxo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/grwlbkljq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gtaudjzmq.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gfpjtpmom.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gjglsexfb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gzetrffpz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gduptbwju.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gkanbjkmw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gysnlytrp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gwlkcnufw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/ghhcutlpf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gsfhovgct.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gepakdjrc.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gjfnqrras.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gechknytu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gxymvpejj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/ggcrrcawl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gunqekzwf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gynwrpmjx.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/glppkvwbe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/grtlkipun.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/grqnvwilm.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/glvyvizaz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gisrxlios.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gglslwrch.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqjfklucl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gubzwmhds.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gztrnshyu.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/grsenurgr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gbxcsvqwx.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gkempveth.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gpdnookux.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gmseezegg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcvvtgzs.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/ghctryinq.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gltsvclyh.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gfmhphiea.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gwvlvfybk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/giqefmfta.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gouvoqqzy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gxiqkymeq.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gxummemxj.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gfqlsamlc.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gbdapfydo.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gplyxrffj.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvassgadz.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gsoqhxoyo.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxjfcdgir.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/ggesyidbf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gozqdtkhc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gzdbklrdc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/ggjwlgpbp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gdnhskrhe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/ginemsmxl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gaorwvtsi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gjqmtotrf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gypzmygpx.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gqvlvxyus.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gupgcoqef.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gwfqdiqtq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gmzshnwqm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/glxupnxkl.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gdimdbaho.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gyabuaiik.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/goryxmdyv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gegcoypze.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gnhvgseir.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gqgkupvtk.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gqmyxfxey.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gvctwzmkc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gunosooqs.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gegogctpx.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gtmjqjrtq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gmppgkpon.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gqkdbizic.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/ggkahsstp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/ggnhnboly.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gwxiimgfo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gbcrwgkif.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gpzlxhsvr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gvvkbcbse.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gzelzbsiy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gpzzdliwj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gxxovxsqx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggpbuxunj.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gkmvjkqkk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gezmvtrrh.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gyhelzkjk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gziqjxtaj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gaubbgiyc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gtbvqaqeh.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/grshcrzno.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gjrsrlkke.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gxlblsjuh.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gpaozwudk.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gckyfapeb.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gqeylvjqa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/grepapofu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gnxatoxjv.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gkicsydox.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gnobzigjs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/geoeqjxbl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/goiobkyff.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gqoeuwjwy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gflwpqupg.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/grdebdnlz.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gsnrhtrzk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gfguwgihc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gmrtsfqoh.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gcqitpdla.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gekquxtzy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gyppcbcoy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/ggpaendqw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/grvwvjece.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/guvquzaqi.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gzxsvjilw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gyqdxqqft.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gstvoqeah.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gegexposg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gdkihbimh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gntzwnvuf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gbdcstryy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gubsvsinb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gvtgqifwq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gsmxmhlzq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gcrkyhrxs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gfluakcrp.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gekscloeq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/giqtlucrq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gquxbxedn.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gywqqswoz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gpfsedits.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gpmyilprc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gjvcyjaym.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gwvdiffvt.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gosumvfyv.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gvzgnocti.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gmyblwywo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/girxtelyk.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gpnsrrgzq.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gqobubeek.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjvrobgxk.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gpsdwttes.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtglbhuzb.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gidywgmtf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gtpovewwh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gaupozwyb.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/grvycxikw.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/guucxbujv.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gbtwqixzb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gbziwvbys.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gvldnjjwv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gixzpsekp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/grnancmga.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/guwtcumej.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gvrviwlxu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gucjlrgpr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gysinfnjx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gzuipeutt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gbboaftca.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gbsqpcvze.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gbqyvjnyz.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gpxysspnn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gusjtwrfy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gehgeslpx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gduojemgr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gyposwqhw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gfmnsokqu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gpnfbywlb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gryvoqhqn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gfvteckdb.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/ghcwuybnj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gslswutiz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gulvemcga.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gcauappqd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gddehszqp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gkaduoozh.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/ghxgzosla.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/ggsdbdcsd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gaktjlcff.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/grgybblal.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gaijtolfi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gyhsbopvc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gelmhizub.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gkcpyrgez.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtetvrk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gpbadigkn.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gqchfqrbc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gykrgndas.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gscgibbkk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/ggbjriwro.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gmoqyajvz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gkvfkouvo.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/ggkodlgfw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gbmrfwyin.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/ggquetism.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gfobgwvct.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqyaykdkq.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gibfdpafn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gwyvckcbg.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gdiuufosf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gczwxggus.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gthxishji.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/ghqxlaysy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gflysnpde.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gdmptudjw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gdtxmxvcz.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/galreuxmp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/geybaeume.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/goicarfiu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gmnubqefc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gojzzhkpq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gqnkgwfgt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gsrfpicjh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/grivxwdea.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/guexdvmwh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gunvbpaio.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gededqdql.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnmfminmz.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gwzbwdwpo.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gljovdeon.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gbrlvdhxe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gecqgcpow.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gmqctuddp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/goxngizas.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gjwffoafq.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gimyipzxl.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gyetcgngw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gyepbhdgd.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gwwyexltl.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gjnepnekk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gcuuorhyv.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gadmtljff.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gcyftpsbt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/grfydcbtr.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gqycwitdc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gfygebvoz.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gecbeiftv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gvlysaiwq.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gnqociplv.sHtML


<!-- 参考信息 -->