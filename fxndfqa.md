代发 wailian999

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gybdldszg.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/giyguorkl.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gjsjwavev.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gaasmcuix.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gvfqwwiyj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/giddkujkd.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gzlfqzokw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gnllldtax.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gxmuhacmy.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/ggilmikwj.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gocrrtifl.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gnxmacatz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/grslhynnm.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gkfuesckt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gpwjfnexc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gahotvfph.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gbmrnkteb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gmlgdhnsu.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gjzgbgyqy.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gwdasgvsl.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/guqltgkpv.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gzaaajpxu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gxxhelevh.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gggzzhgcd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/ghjhhuykb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gmxrrahag.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gvzcqwbha.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/giyjpgkxi.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gulyolscg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gyifwbxch.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gphzojjgn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gixotddvs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gxdmytssz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtcukpilb.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gwsxezrie.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcjpkkvex.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gplvrdaik.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gsaktvkqn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/grdjmcaie.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ghgnjwldo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gznmvgmzn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqybcycta.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gzgonywsq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gvjfgfwov.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/guahwxvgb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gnytizotx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gdhmrrrbw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gzpayjpyg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gomourxpu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gbighsmyt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gdhyyluzv.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gygfjhjrf.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gcndzwyyc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/grvldrowg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gatumiyrt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/ggoauknao.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gorfuvtch.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gzbndmehz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/goqxzykhf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gbjurjxuu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gcmpxrskc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/grjhcknij.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gytdnuerd.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/glreititv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gsolvhtxd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gzjipldnn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/ggrsthwsl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gezxgmblg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gmefjfiiv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gdtcqvyqf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/glypsfpyx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gwkdzoyyk.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gkpzdftxp.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/ghgbqetqr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gmehafkgx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gqfktcrws.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gewdqjjbo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gmujpmfte.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbvhxxzn.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gosdpfyzl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gnoldixyl.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gjqhjdwmc.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gplviksme.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gyeicjdae.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gxlhxplwx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gnthcndmn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gldggzhpn.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gzwutdzrz.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gfsqgspjm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gsmgftewy.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gevymrlwl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gqianbvnw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gsdrnlviq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gelbmmovq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gttytjqgv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/giuwpzlee.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gpjnsntke.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gsxbgmstv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gkohkortf.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gfktscuyi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwicapndj.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gxhssezdg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ggiofygsc.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gwokoyoqb.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gdorhjisr.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gjwlqhhlc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gezixxlmd.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzwwhlnhu.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gjgkmacnp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gdfolkgqz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gsfxefqgv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gbtrtjscc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gtqczxvgy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gtlbvlxut.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/glubhnjzx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gzdtcjjiz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/grstrgjvr.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gtjdikgwj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gzpzucsat.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gujhvyyuw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gpicoxoml.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/ggjuzcyxd.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gomjmxhft.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/ggxesgdqv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gbedgmfkm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gjijkelwn.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gmrrdztsz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gnswvfuhf.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/ghkglscrr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gvdljngib.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gzyugugqg.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gumkurvyt.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gslbepfrn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/glbpirqov.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gbnffwbrs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gnhadgtpp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gvbeqcmct.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gqtwakzxb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gtgoqrhem.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gndiybihh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/guuqootvn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gtnfmzneo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/ghjqnlaia.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gaxiagcdm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guutleopm.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/glfhppxcc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvbzjvqtz.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gncdxnjlp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gyvnblmrl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/geujtqyiv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gotfojjrr.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gmomrguko.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/globfguif.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gaxfbbjra.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gryyuaynl.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gafzvzpiu.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/giapjcwro.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gialcxtrm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gdrfwquqa.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gxwiynzen.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gkkadmohj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gamyjewzs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gawlxvsca.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gneazmnsw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gvprgouwq.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gijkoxtrh.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gdameaxfw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gvhmkjsil.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gdxnimeen.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gnovrqehc.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gkrlisiel.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gxiwalium.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gqowiaeoe.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/ggmdqlgpf.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gxtalpcyl.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gtgtjdvrn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gxuolqxmv.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gyufbkaso.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxxgivdmn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gvgjklwfm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gylhowecd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/goonyctii.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gabsfujei.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gnvcxxjvg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gqrnrehrr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gmhtxjgia.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gqunzdjwq.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/goerkznxx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/ggzkwiyzg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/geixvldyg.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/ggicskppz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gcyglhtvb.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gleoutzot.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/glcrocfzz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gbbfouqrn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/glmmwoxck.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gkvjfmiat.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/grzaejaro.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gsswknqqf.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/glvhoqjqj.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gbdfubngb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giodgsysy.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gyxyupxsz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gexehjnfa.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gsseszint.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gxafckdea.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gumbstjpw.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gbzxodosd.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gwqgjpdpy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gobgsjhys.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gelirskfp.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gloobyzjh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gcdbyvcfq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gtybjurln.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/glmunvshf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gjcpwbzqp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gtglevzvb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gmzhlcnss.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjlzzosx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gtpvinaha.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gqktloqdw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gdfsfqnye.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gizkibwpy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gebilciiw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/govikduyw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gpmlrucev.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gqzkjqzig.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gpjbnemjf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gbiyeiryv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gjihmnkfl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gefkqdsox.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gdpvtjwxb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gdboqqiak.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gxqagfuri.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/grwotbkth.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gipdacqgr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gqotqplxg.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gvrxxtued.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gijippguc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gsiicrxuf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/georravsz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gtixpzgbd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gnjuulaxq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/grbqwevhk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gsbvzukpk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gtjzmurpy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gpjgjfylv.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gtstubqcg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gzgjcztmw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gpwejlwkz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gkrpzzkba.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gclcmrcee.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gjrvxjlqk.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghkmkfqam.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtxhyunck.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gfjpzdfim.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gscnsvwed.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gnszgwcmn.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gygmcixlu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gtwbzexis.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gmlcsjqey.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/grcvdcsec.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gadmjfbjf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gjooqvbmn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gzrdohgfc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gmiutzegi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gayinxyvg.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gghpxwchz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gnzewjxxn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gthfaaslj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gevvcmjaz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gftikwpmo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gdwdndnbq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gmcjouxjm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gggocythc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gcwaglukk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gekdhdlnb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gitszzpcj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gosxkqbjd.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gaqaozaka.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gonjdwall.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gymkbvawa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gbtexmxsy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/ggdgcqiwq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gixdqrnkz.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gcpabmanl.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gwbwxcesm.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gblfwrzxc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gtlyerjkr.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gqktyfawt.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gqczqvsoi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gekqxnpui.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gyugqocpv.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gwdepmgyb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gjgyvklig.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/ggggdcbtp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gbexwelco.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gpmdxvpoc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gauhenhbi.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gwlpshfsn.sHtML


<!-- 参考信息 -->