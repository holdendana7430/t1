代发 wailian999

JS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjivrwqab.sHtML

TS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmhuhhcxn.sHtML

Java: System.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhludmpv.sHtML

Go:   os.Exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxpbtgoc.sHtML

Ruby: exit 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gqollvati.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmjbahmh.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuhymjrv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfkiqkto.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyyjduwx.sHtML

JS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfefornk.sHtML

TS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gnefpczmy.sHtML

Java: System.err.println("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gytaipffd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fanxiaobao.xyz/Article/details/gddzdjrwi.sHtML

Ruby: warn "err"
来源：http://www.share.fanxiaobao.xyz/Article/details/gytexivhp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gduosazxw.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxkojoul.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmazetgr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/gojmlecfd.sHtML

JS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/glnwrionv.sHtML

TS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/ggydojvnb.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejyqsbof.sHtML

Go:   func main()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngldftye.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgzslrmd.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gebcatlvx.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeochphy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fanxiaobao.xyz/Article/details/gratbfjvv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fanxiaobao.xyz/Article/details/ggdznceqs.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/gplqrwfqw.sHtML

TS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gfypprceo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fanxiaobao.xyz/Article/details/gclbuobhj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fanxiaobao.xyz/Article/details/gxaddyuvf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhjrchun.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fanxiaobao.xyz/Article/details/goauzxecx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjhqrdwk.sHtML

N. 数据结构与算法
来源：http://read.share.fanxiaobao.xyz/Article/details/glicvobxw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpatbyksv.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjazuajlz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/glvwbwxrl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/gugvlxfwu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gcnxigxpu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gicttgqyv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gqcmjjjbk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwetujtq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykbqmfvb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqvltreu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fanxiaobao.xyz/Article/details/gicpdpyyz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fanxiaobao.xyz/Article/details/grmtjhwie.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gmovlpptr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gevhcsbys.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gqoeqpxyy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gsnegjpky.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gghqubyep.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvxorpxh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjitvcuw.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fanxiaobao.xyz/Article/details/glzjctvqf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fanxiaobao.xyz/Article/details/grdbjhned.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/giukmfnba.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/geqzowlwp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxzmgleb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gxmtrwgvl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzudhjhf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnqedqwo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fanxiaobao.xyz/Article/details/gcdjgcnln.sHtML

[N04] 斐波那契数列
来源：http://wap.fanxiaobao.xyz/Article/details/geedbrgfu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gckrvpetx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwfrbkhq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkciwokcu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwudshog.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fanxiaobao.xyz/Article/details/gctrvlgbo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fanxiaobao.xyz/Article/details/gxsaaorwr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gwfpgtmch.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/garbykwec.sHtML

[N05] 最大公约数
来源：http://www.share.fanxiaobao.xyz/Article/details/gemvhryum.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gwydvkzwq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvugcjmww.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghqxdhdxh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbdnzizy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsihsvaxq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjthcrkbi.sHtML

Ruby: a.gcd(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gvipjzuvn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fanxiaobao.xyz/Article/details/gaifpcnck.sHtML

[N06] 判断回文字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrbrhmpn.sHtML

Py:   s == s[::-1]
来源：http://wap.fanxiaobao.xyz/Article/details/gjatyjifu.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gzwkdqnek.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gugplhbkd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkgqdisk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fanxiaobao.xyz/Article/details/gaeipfsmg.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlobjzty.sHtML

Ruby: s == s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpavhbpw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fanxiaobao.xyz/Article/details/gghgfcfay.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fanxiaobao.xyz/Article/details/gbaebmkgm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fanxiaobao.xyz/Article/details/gkzdlzwqt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxlxawcz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzlncnvk.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwqjxsyh.sHtML

Java: // 手写 HashMap
来源：http://3g.fanxiaobao.xyz/Article/details/giixekayl.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fanxiaobao.xyz/Article/details/geimqtcyt.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitujsvxd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fanxiaobao.xyz/Article/details/gtxlmoroc.sHtML

[N08] 生成全排列
来源：http://blog.fanxiaobao.xyz/Article/details/gsqlyongt.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gctshiugq.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjubxnvv.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gcewvgpsy.sHtML

TS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gmbmthbrs.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuvsoluj.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnupvxpq.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gzonmqkcc.sHtML

C#:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gpeojsurd.sHtML

[N09] 栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/gamxdrccf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/ghcxjeqbx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gtckxzeja.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/grmgwnswi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fanxiaobao.xyz/Article/details/ggwpvsyxt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvwhhbfu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyolzyyw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaprdfts.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/gfnjypmwy.sHtML

[N10] 链表节点定义
来源：http://wap.fanxiaobao.xyz/Article/details/gskzpxrbz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fanxiaobao.xyz/Article/details/gshdalcvd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsolxkodg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fanxiaobao.xyz/Article/details/geysslaez.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gdccpyqlm.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtkpfpfhu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaiedncw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/gamzelecq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fanxiaobao.xyz/Article/details/gilqryfmi.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gitbsbwxt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fanxiaobao.xyz/Article/details/gogqsfkzv.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjvsoqys.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/ghjxnxide.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gjveymjfm.sHtML

Java: // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqikythzv.sHtML

Go:   // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gqukvlfvp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqlglglt.sHtML

C#:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gdutrjutl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwksnmukq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgqvwkmz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fanxiaobao.xyz/Article/details/gypityxnk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gsticjrwm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gbxijjnnp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gstlcayav.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fanxiaobao.xyz/Article/details/gjzmpmkba.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzujfuyn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdocreju.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxbiqzqbq.sHtML

O. 并发与异步
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdmvfxwq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glevakxdh.sHtML

[O01] 启动一个线程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwenrhtzy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fanxiaobao.xyz/Article/details/gazcnpbix.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgodbodh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fanxiaobao.xyz/Article/details/gzlcljguu.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/ggrxfwgwb.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfratfba.sHtML

Go:   go f()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnasmbens.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqxtjuoy.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fanxiaobao.xyz/Article/details/gojkjthhb.sHtML

[O02] 使用线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqdklkpm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fanxiaobao.xyz/Article/details/gyqgylrzg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gvqapwbkd.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gvdijomda.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgxymvma.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fanxiaobao.xyz/Article/details/ghmgsrmfv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fanxiaobao.xyz/Article/details/gyelqxvdp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/goeohsrdi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsnrvblz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjfxbkuq.sHtML

Py:   with lock: shared += 1
来源：http://blog.fanxiaobao.xyz/Article/details/gmhqntmpk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuwhuvtl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjqupbba.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/goisrgite.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdqskwmcg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcunafpzo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/goqjhbwod.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuakbihb.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gbladipgf.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fanxiaobao.xyz/Article/details/gicnmipjt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fanxiaobao.xyz/Article/details/gwajuxpoi.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gikppwstj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzymsstmp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlpukhir.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpgmizqf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbasmezv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyzifvgf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppgurfqd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyxvzjpa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwkoelnp.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtitvdxm.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/gzeejeuyi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkezxnah.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaiiheni.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gyhasvcvn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fanxiaobao.xyz/Article/details/glyjyahgp.sHtML

[O06] 使用进程池
来源：http://baike.fanxiaobao.xyz/Article/details/gkqeipjza.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fanxiaobao.xyz/Article/details/goyketeax.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gggzgapfc.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gtcgkvzbj.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlnebsix.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluajxrtj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtylbjez.sHtML

Ruby: // fork 块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbhykriy.sHtML

C#:   Parallel.For
来源：http://wap.fanxiaobao.xyz/Article/details/gpmexkdci.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/girwhcbje.sHtML

P. 常用工具函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkvqrvtx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghisnfoqk.sHtML

[P01] 生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gvylvxdsk.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkvlnmkw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvetxejro.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gwxgdpysf.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gejmgdsqw.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gqyuoamqe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmrvonkh.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/ghottlhfq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fanxiaobao.xyz/Article/details/gnpbygvxj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fanxiaobao.xyz/Article/details/guuimawms.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fanxiaobao.xyz/Article/details/gunofmnqw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeprkelp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gcirohyqu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fanxiaobao.xyz/Article/details/goybxefya.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fanxiaobao.xyz/Article/details/gbyjqancx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvhuavfs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyurcwac.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayjpliyc.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzdvkzmb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fanxiaobao.xyz/Article/details/gejveutkk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fanxiaobao.xyz/Article/details/gylfyxrnd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/glfnosrly.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/glejfledj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjvbrexi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fanxiaobao.xyz/Article/details/gwstuidyl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/grwtaaveb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fanxiaobao.xyz/Article/details/gicwblnoy.sHtML

[P04] 求长度
来源：http://blog.fanxiaobao.xyz/Article/details/gkihzaatq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gadzldgqm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gvlnuanrg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givhuwhkb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcfubemb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyulkkwrn.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvclqcaet.sHtML

Ruby: x.length;  x.size
来源：http://baike.fanxiaobao.xyz/Article/details/gmobrshsh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpibqolto.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmyhpiex.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fanxiaobao.xyz/Article/details/gphrngrsj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkrhqyjk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmenghed.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gusemnlld.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fanxiaobao.xyz/Article/details/ghiabtzus.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpslfuzh.sHtML

Ruby: a == b
来源：http://read.share.fanxiaobao.xyz/Article/details/gcplgkaqj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fanxiaobao.xyz/Article/details/gvvaligtz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeapgnju.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxnqjino.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmlriiumz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmjmnbfv.sHtML

TS:   if (x == null) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grhevtwjx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghrmsiihh.sHtML

Go:   if x == nil {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnnyrtcd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhxwrtla.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrwgbhrw.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjdddhbz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fanxiaobao.xyz/Article/details/giatpuifa.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gncewpeqx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkkngtwu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgxnspwz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjkahcvt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fanxiaobao.xyz/Article/details/gssfroqhv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gkghgdejd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhkuqhns.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fanxiaobao.xyz/Article/details/guhglfheu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbclvpnkm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqovzcba.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fanxiaobao.xyz/Article/details/gilrrggts.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gndwxhseu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/gwtiwckuo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/guanghyrw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/gewduresd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gognngjgb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakcurshe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzrgsbza.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkbcmingu.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/guxkdpagg.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gvgnmbznk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gilnxfdtp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gzmzwdtwn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnqukhez.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/gagarvsot.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govfdxuxv.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukyqiern.sHtML

CREATE TABLE orders (
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcrtxoto.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gfuqralqw.sHtML

user_id INT NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gjtpqwwwb.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjmsjdmk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuyqrits.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gxrtnagnh.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/guoeuspnu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gpmhokyuw.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gvolsyggq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfvfzmns.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjsfsfyf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fanxiaobao.xyz/Article/details/gwjgfwwji.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmijiktxj.sHtML


<!-- 参考信息 -->