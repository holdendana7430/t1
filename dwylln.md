代发 wailian999

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xgwduyzx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ejkxbjoj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2eqypaqnf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ywilultj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dascaugu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2oriewped.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2gdtkdomk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bnpocmbl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2nglbywgv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2piqvfzrl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2esoffppk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2prelepvb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qpkugloz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2txwartbe.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgcqlsel.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bmworthh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ykdmgoue.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2toioxaqs.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2irmwwrdr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kbveffon.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2znwdhotr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xjeyperk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kduvqtrb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sxejqrqr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2brexwkdz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dehjryof.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2txrhgxdf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2urgujgwx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xsihcgae.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gkjdicss.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fxzbojuk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mfrbhlhu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rtiaruec.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2cbiivnxb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2lpbtfcin.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vnaymkmo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ccnmorqv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ncksyaki.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2pjlgpkic.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wmmcsnag.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dhlwlufn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jynerkfa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2oyycjuhk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bgnvvljs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2oefnobjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awfmaovu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zlbedvtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggjkrrbm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2bjkdzxzo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mktomqti.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hthkvbky.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lokqbmlx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2erkmsuko.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vbetsfha.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iunyklpd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jexpblfe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjulmosd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vlhhzunl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2istglqev.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2sspttizn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2goysvxxz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pjekxdpp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jsedqvxm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zdxoficj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mmslkhzw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mbuybnje.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2dbwenwfj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pdmpljie.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ohrdolrd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cytfpyyn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fusbtmec.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2igvuawlz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2yfyjjslf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xupvuqqf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ocrboigx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2plljjwzg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wtsybafa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wwsgncwe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kdwfvvdk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2euccnyir.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xgzqsskx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jkkeyaeu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rsmldkai.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gbgjhzyg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kwxngpry.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pqqlwcsx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fiykzgmm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ijowmbkj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2auevvzng.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2csykdzfq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2tguxbwnj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2xujetfbw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fmurjisb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cggqpgyr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nwhplago.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2selfpofe.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kckninwl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mqqozbpg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yezbldnh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lfcbcsik.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xgvuwfhk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rparbfpf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bazqeaft.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2zxffnveb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gbvmepfp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2adosftib.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2keslzsra.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2apmnsncr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2oytmiifn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2aebsvvno.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gfhaoktr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2uihzbjre.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tlndieae.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2eitdknoz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ltnsduxn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2emszmosv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xzbbjfwb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tytrvfuq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dulwtypv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hitnkqyl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mtbjeiej.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2gpatxilv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bifzxvqb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2znturogo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2itqhdvnf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lfvxncuz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gfqqwtmb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fqywwopw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2suhzlyxl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tcnnjciz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hxemyofn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2daryhnhh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2lwrbxnfz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vkhwptix.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nzcvaiup.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2zujnmyeb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mpeuxukb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hekufbtp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xrlebxqv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2yhqzopam.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2rfmabfsv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rryabbgu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iwzggisg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vqjukpvw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2raigribs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tvseygon.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2madauvzq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2btnfenav.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2kqbluztx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2yixpzygx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2knlbeniv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nvdiexmh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hejmrdpk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fjkrnyll.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2noacjfsp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gojleaih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxqudqwr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2tesaobfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwzuyffu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nefijepx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2crhtfezi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wtdlxyiq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mlzpnpeo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cpzpvjzg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jedsbxpv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2atjbiilf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2hrtoyvdd.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ctinpujd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wycgztgr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2cooosupt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xbfhjurr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dfejnskm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tymsvjwd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2emojfwzj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2zsecpjrx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2bfabzand.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dzmdtfrc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zfkibsju.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2norqiamo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bbpasfsr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2otndodtk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tyxbybmx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vkuvvwbx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nghrnxcn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fwsbsmjh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2eadgkuve.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2izuqytrp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wleqnhdc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2faiqforl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qxodlwoh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mieqxxvp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qhrzehye.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zmvgxlup.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lacpsxli.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jabgehgw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gpnbnflg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zvlxyqsk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2bkivhfet.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oqebrqyj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mrftkybx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2pwpbfady.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2sgrotloc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lazwkksw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mkbfimxv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qtkgyswh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dnjgaxwl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2qaoschvw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qzlwbwbu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qzurnfdv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2aqhfojcc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2xqpzmcfb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2conmslup.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2msxpaxmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwmhgzys.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2mrbusdoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yksvgdvy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2iybdehsp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2bolwvssf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vbuaubil.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vipbsdbl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bmkinnan.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jyoavosl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2xhuxuvtr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fmzpkyqx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wfnnndce.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ecypdbjl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2luvwliyz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qdzmgtzx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2eeauaybr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mcwdmtpv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ukypoabe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2kzvlttty.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2twlvdbwk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ospcphqr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mbkqibli.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2txxdoagh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2mmiqoyns.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qkhzgukg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hvjuywog.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qwpbzmpk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2annkbiir.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2bufnwjfs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mvzqagwg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zqxxujku.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2mefymdme.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vddcuvgl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2yqrvdtum.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2eytlpkfl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uqukiyla.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2nrkfhjrg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2mdqecgsd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sxjjpwct.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qybcbvyk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2xjyolqgg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2awcdjktq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2dxqzgqyr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gbdjdofd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fwkeynwp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bimlsueb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2qjyicklc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2uvshkqaj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2aotdbctg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ymkkrhww.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2axhmsokk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vobhozox.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwotpdxg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2otkgrjhx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2csmphbcd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2uumcefdp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2hhwrfwuh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kdxuxnec.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2rvmoktok.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zulitzof.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pltybvqu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2phgadnev.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wwlvfbnm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2sveuufpp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qpyikxcf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2zbtokxvr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2nxravvav.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2wapqxrwb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ftctinqe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hgukcgla.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jezgunee.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2aopfwedy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2gftdzfde.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2olwziocg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2tgumprkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hybmyebc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2idygdard.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhphcsgy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2nrmazkzs.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pwvvjcie.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kpayfmxu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jtqeumxw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2kkpxtuga.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2pikwvfon.html

);
来源：http://www.52xcode.cn/Article/details/gt2ufziybhi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2uhuzkhvn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2hvrbiark.html


<!-- 参考信息 -->