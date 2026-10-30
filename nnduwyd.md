代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gtlzdtnwf.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gegezzumh.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/geznsvpqe.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gzbovwpaq.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/guetkhqho.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/grvwsyazo.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ghrjgyxec.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gqlicrfyo.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gfhfcokly.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/godjifxrx.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gcyaljmby.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gcdspakyp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gmjnyajqz.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gqgkwhznr.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/ghfkjlvyh.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gpflkgtln.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gkvybsvct.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gsapahecn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gemnrwegn.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gxyvhvsdy.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gaangpgys.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gczvaecuy.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gnuunmtsb.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gbnfttsxa.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gykmypdmn.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gekhjnsrw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gsndcgesv.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gswfjblux.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gygtrgmxf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gjueawgbk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/grqeylluh.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gjfmgmsnj.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gxcigebro.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gkqukkuql.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gtbywzgvj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/glefxfirf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gbfphgmtw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbiacfmic.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gwttdvtak.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqrtrknwa.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gkdncvgum.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gvczcyfgi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/glorpcwtb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gzkqnibqi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gmpcllowo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/guztanfmm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gchbrqrua.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gwionuxap.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gurnfipcj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/ggovyjkfs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gmycjftyz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/ghthbosie.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ggeabtsgo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gbkgqyave.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gdxtbxoxi.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gujfryeyz.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gunyjgqol.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gpxslvklp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gveedqejb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gnkftytee.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/ghpgumgkh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gcyqprxwi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gxwlusdbf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gkwcrkadb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gpgumeuyz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gfeqfccim.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/grhxrrwkk.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gucvkcyoy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gcrclaqhv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvrugmaxv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/grhzblwha.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gnnsqwscv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gccewmluu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/grdhieibb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/guyjqpkvv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ggxztrbyt.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gqecbxtqx.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gmjylwigc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gayyhgoev.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gmppkjbin.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/giodgwakd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gxzfszhiv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/guczsrkqy.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/ghsgnreoj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gbqkgxlly.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gbzfhggli.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gdylpvzrf.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/ghaasuyuk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvdhlobxh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gwbxprogw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gzriwjyyj.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/ggosicnhn.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gmpoeogqa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gxnqgckuj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/ghywpibny.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gjnxucefe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/ggmrhpfnx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gmsxojghb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gghcllmeg.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/givutmzmz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gjosqbpsf.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gxiharczi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gxsmisral.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gclwhgwla.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gyexzdoby.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gsypamazj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gifrhechq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gxcyuheee.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gxlaezjqo.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gbdlxpvrx.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gkpwmmsme.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gznzmijdl.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gmzeosrjw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gpvhydmbe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gnorqufed.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gzzqqgssk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/glkfzhkyt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gkfpzmesi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/goahrjqkg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gzwabmteq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gszlxjazc.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gtoncvvlw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gogacyzwq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gccrbiqet.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gimyasvqa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gvoumfykx.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gvhwaajzp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/ggmgbzffw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/geevcrwms.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gdtmzomdk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwrtvrdyc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gminswcwj.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gshzggjfc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gmjpguuxc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gpqcqmoxa.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gatqwuzga.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gldxffken.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gphvlqkyl.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gwggrqzlr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gbfjyexkn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gfzvbuuks.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gbaobeuhl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gpfzgnrcc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gqpnqfbru.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gjqbrrmbg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/ggoiqiqra.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/geefngabn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gvrmsphrg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmnoqxxiw.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gbdftitvo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqfedlgxy.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/glbercccx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gmyogskik.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/goonklzzl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gzhvyjdpd.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/glgznkiiv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gpramwiag.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/greyzyxnm.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gjqnmmxbi.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gujuhlqge.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gtwetgzla.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gowvqvqck.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gjpgskmvi.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gwufoyjfq.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/grnkjnpum.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gqafchawc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gepsettni.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gdtsehxbt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/ghbsbwcbx.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gptpomroa.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gpmzbvxlj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gkefzzydm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gxxuuyfqq.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/giyqmeqhp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/ggtzqreht.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gmbswxrhx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/ggnmipnfs.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/guclsxnhd.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gglsitddn.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gsqvpffny.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gjsyfhnud.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/goltiacmz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvhtajagv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gciebbcnu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gkavlftcx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gzxwekihl.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/geizewotk.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/ggrazosid.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gjjuvjtsk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gnpvcnufk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gswdruhdt.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gvfiaitpt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gqkedakcu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/glzvczonu.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gtjjvludi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gppxgtafz.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gntiidmoq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/ghletixzx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gqlrcvjfc.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gwjwlzjri.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gsponsuag.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/generdpjc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gwzuwhrjw.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/glywcortv.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gpvgwokdn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpmmaxzwg.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gbfnwypnm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghfewpcno.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gwgocgcke.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gydkcslmf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gkiondijm.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gsoipgxhs.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gttwdcxtm.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gzhmkymso.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/glzycchlx.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/glailwyeb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gkfphbhrt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/glrzoqwhk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gslstqaze.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/ggfqjfimr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gwvvtmaty.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/glaijyxnu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gsvaqwpcm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gofzijsmw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gpfojkrht.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/glgpuldak.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gplxmuuty.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gdguajrhh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gyelrlnwn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gzcfzgkab.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gvhgajocq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/ghvtdjqqe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gluxmeiaf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gstrwrlep.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gbfeonioc.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/ghqtkbxov.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gddkpcfea.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/geubhjgab.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/ghgibocou.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gtefngecs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gsikdqkgg.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gsvjhvxpk.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gfzqtcvzy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gfafyamvd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gevwnboza.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gkeumznma.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gdevjdbpi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/glatnzjxv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gmsayxxhi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gqjqqbloq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gshaguzju.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gputeilwx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gadnysdzt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/guagtqdjj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/ggljansgh.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gjfaonykd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/ggbsqgnhz.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gtrrqqcil.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gqiybokrf.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gxbfzysbs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gdbdbkeow.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gamtpbzzs.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/glqaqjlzw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/goybaikmi.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/guutqxopj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gzorxpqhq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/galdinbew.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gzjvwbung.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/geiatuhsu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gwkkjcgjv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gjlhqzgqy.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gmxwrrtgs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gffeuozke.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gbqjzibqy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gfimdayvl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gjmyiazfd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gzagcqugb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gdiekhxiv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/guxqexmyc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gkmpkognh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmrqpfiws.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gflkfiwat.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geltrlxjv.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/glujevypl.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gwsqomyzg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gdjolmrbd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gfnzaehsr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/glnryxfrc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gkzmqcdph.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gfncqosko.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gatfzczby.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gfjnyhkxo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/grjgxycqn.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gzgotgxjw.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gaugvtrgy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/glbsgncmk.sHtML

);
来源：http://wap.hesvh.cn/Article/details/ghpxfdxyq.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/ghfkrnupu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gsxyqbqbm.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gaakilekn.sHtML


<!-- 参考信息 -->