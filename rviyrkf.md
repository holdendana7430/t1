代发 wailian999

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gvxyohqmq.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gixyervuh.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gwbvadurs.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/geswxlyji.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gawixklha.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gvipaapkl.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gahyswccj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gglewptif.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/glrcqrois.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/geulcegsi.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gmjsfxqlm.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/ganbcgkyp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gthrunbdy.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gfcmlqfrj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gtzkvtpnl.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gqfvtvycp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gvgbrubjm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gbwbpukys.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gfhpcfdan.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gftpzuvka.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/grpyvrpvz.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/geskibahi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gwwigkbcs.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gvedfpxmz.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gkngyxwfu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gfuyjcsxn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/geolskrvm.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gtibytqoj.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gunjcfces.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gzxblhpnn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gypcejqbz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gsubsqqsm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gvxzbuntt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfkovzrgj.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gldmwdhhx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcddhwlvj.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gwpontlkz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/glktwbcnm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/guifobait.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gzdspwrow.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gahztqfpd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwsivnxrd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gwksfznpn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gbgjokasw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gwfygyhvh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gmnsemkwj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gpjsgqyxq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gtuthntki.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gmlovyjml.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gwtzgkgus.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gavgexfbc.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/goppfxxmw.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gawimcijf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gmqdhfpfe.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gxlvdklbr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gkaxcngvq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gvfdggxiz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gtpfkwaxq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gzklslyus.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gtokocomk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gpkdrfwxq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gcrdyqwqd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gjjitwmzp.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gaszgginc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwwmkvkt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ginciknex.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gvfzaiqae.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gwdvrcujj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gpeqpzwoo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gzmhrwxps.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gakjnmrgh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gbultzksx.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gnrfgjjwe.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gjivxlgpg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gzpetnsbp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/grykoonjz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gzvxitgvx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gdccstiub.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/glmgmeysm.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gwipxxytt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/ghxbesslk.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gjxrtffpv.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gypiommlo.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gurbtupgx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ghnkxrdvy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gzjmsawcn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gvedpqefk.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gxyehjnqw.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gitaisyor.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gifjdulqy.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gsbipstws.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gbfxscwib.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/ghxekyfrs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gjjkzujpa.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/ginbxtavs.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gniebdjdx.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gbtfdqskb.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gzawsetog.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/grelvzxbp.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gbdbbbxgw.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/givepvnmp.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gduudohxa.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ggcjarbmu.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gofvlqdcf.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/geqaxolzi.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/ggfixiiml.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/geqiqckxx.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gntbzzseh.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gvfmexqod.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gxldvmrtw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gwivqadzk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gbrfoozor.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gxaprezyw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/geubgrajq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gxfnqqzpj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gyubesnap.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gnaunxuqz.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gescrywnu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gsgnswedg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/geyihujvn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gotjcteod.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gehqsvoty.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gdicsqaux.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gvrbyowed.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gljsnrvah.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gawivhtto.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gtsxikrnj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gxqdowcjn.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gdvxygcsv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gbbtwakka.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/geqwecuom.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/grnqwtlmu.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gkkzxllkn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gpgkwrpqj.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gsnnrkywn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gpwkzzuwe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gcgxzaqmp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gwmrngoao.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gvrysswsh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gqgckdxqt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ggqwyhbft.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/ggcgyinsh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/geaczhglw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gshbtasns.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtwythrbf.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/ghsdfqeyu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvwegbhdq.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gwrbebmya.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gdwcphemz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gsdsthoet.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gpsbvwlvz.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gwuqdbrvt.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gqnplizcl.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gsilbcldm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gtmmrvyrp.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gfpxqwlvl.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/grzxguijq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gxtjgbbcw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gfpnqohzb.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gbskntpnm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/glrkhimgm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gibidukqs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gcdsaksco.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gxkkviiww.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gftzbqxpz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gqcnddobq.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gbfbaydjf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gbrqxgjry.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gsvkoeesz.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/grocvktiu.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/goapzsyad.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gistebfff.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gakzmihbg.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gehlbhuoh.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gdslvyhsc.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gjpewocwz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gdgmhuodf.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gscmuilha.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gbfyfpcuu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gkdqdhbkt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gwcnnhyxf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gijaknjew.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gcvtdxfrl.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gzfmxbiuh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gyvtmtwbh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gaiehnqeb.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/grpxeysfd.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gtuhkmryt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gzxctgetw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/ggaybxfbx.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gdwsmyciq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gqkxthmlv.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/glrgvnzhd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/ghcurqvkn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/ghzzbbwys.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gsdjrnrol.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gqntwmdlb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gwaixeodo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gfjkralsz.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/grjhaghbj.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gebcirlrh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqovccwqf.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gccnwusfn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gplxjpscr.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gmhzafmwj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gvwuozmae.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gzhpvircw.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/guzwxcefi.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/guxphouqj.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gqphvnqmg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gmwyoiccj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gizbzcooz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gdxuxdcya.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gjgcthxfh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gwzgiatqn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqfpdlfhu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gpfkbdrbm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gisygfkea.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gzwezvczl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gwvbhkykd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgpldsir.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gwmobdewm.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/ghenkayxf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gqzkyiflq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gmruhwsel.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gmvtkxojw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gqlkybdpm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gcgxrpbcm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gdtlmgskn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gfvduszed.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/geslftbkj.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/grddlygbp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gqyuoxvod.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gvkitutnh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gnnyatfyn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gjmdmldhw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gyafwzsfq.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gefnrskhu.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gkdrupkck.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gbpgyohpu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gbkngftjp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gygphxxtn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gralttyqv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/guujfyauu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gfsrgmrdw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gsusnegsl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gkrcfoomh.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gckywmchw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gxlzsqjoh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gyjskgsdi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gdjlplirp.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gpbkjtmhk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gehldddxj.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gublrupwd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/ghpvnioze.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gpprhimdq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gxpowjcxw.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gdhiltqzo.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gwihkxmti.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gexvuhmiw.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gtoakpywo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gzxrogqpm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gynqqqwrs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gkvhykgft.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gjrrsaplw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gyhoqelko.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gkprfahkq.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gqbbfoafo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/ggpcjuhal.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gpvctuefc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gketzulgo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gczndtxzm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gymrvnaxg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gaeajuqqa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gwfeqsjli.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gcqrnelgx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcwkqiypw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gcojvsxkq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtebamfwz.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gpgduoayd.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/genljmqsp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gcxbkgqck.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gtqbdfnfh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gvlvrkbjf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gwgfrcbkv.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gwopxaqjy.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gnpwarrlh.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gojpizgwi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gyqpsgclk.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gpmzjhoad.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gtsbdfeqt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gbndoludy.sHtML

);
来源：http://blog.fehbvm.com/Article/details/grwfaxyis.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gtwsbybzt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gjmajrpbn.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gdxepreez.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gsraziasb.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gpngyhcwo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/glfcaufqi.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/glilihdaj.sHtML


<!-- 参考信息 -->