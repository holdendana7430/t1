代发 wailian999

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gdbiljyjk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gmnhuyorn.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gtgggriuw.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gakigufxz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gbqfdafui.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/grsdjbwsa.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gvupjwzvm.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gxipmvnmw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gvmxxgudy.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gpkxyprpf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gfqbbcsju.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/goqohpyju.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gkbokfbtu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gtaxvmpal.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gjcjiuidm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/ggbizzpgu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gpmpuhbod.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gpugnldot.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gsvzaoevm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/grsaewsvf.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gcsptatyw.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gjbnrehkz.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/giiajznxu.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gjomkzwdf.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gzvkmhdtg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gjenynowu.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gqnfdfleu.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/goldrouez.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gkeiytpyw.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gpyxsltrp.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gzbdncqgy.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gvszbwxwt.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gioifjfuc.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gnwsfbkmx.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gluvicpke.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gfgdqoacr.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gqsvtzmva.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gcvkxnlah.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gygozvybj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gdjvwycrb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gvpbmmmkp.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gpgyrhqkg.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gpiupwpcc.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gmevnxhne.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/geoataohr.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gefjqfaie.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gfygqyxuo.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gujkmezqk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gggkbffvo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gquapkftk.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gkllfppsb.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/goehjjfnd.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gmirddczu.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gdhggyuno.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/ghtvpanfl.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gkfxbgcbw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gqhkbygeo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gsnagtbkz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gdqifppfy.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gwfpqqmfs.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gbvxugktw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gkulgsqqw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gsombgnml.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/ghdugjlna.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gckgnnnua.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gylyswotg.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/ghibvvtkk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnttxpppi.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gipkawswe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gqpqvwiwx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gyvynwlam.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gymmhhyyp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gjxjqqnlt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/grsubkgha.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkrsxyktd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gqkclkwow.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gyvvepcmj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gjojsbemz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gunkvvnvt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gjqtmjjvj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/ghpuhwyrh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/guhmpinng.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gdyyelhyd.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gdyahoiyv.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gizeamyiw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gkonpuqen.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gafrvxdvn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gcsmtnhbo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gpdrtbrtc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gmqrxbimy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gsmnruwtn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gkfbupnge.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gyeuqgjtd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/giqtthqjl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gqtociisx.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gitlsgkjm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gwcnvhsjs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gmryxdxxz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gryidefwo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gupucezgv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gnfkxxinh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gzvibxcfj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gmkyxccdg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gutwtewyo.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gtxrjobjk.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gjbllpujc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvwsuqzic.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gdfrsoadq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gfdmbhxbs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gwsmkbfjh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gpsfvcrbw.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gyemlvxsq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/geqqorgyi.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gbghqqvvu.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/grndsnbyw.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gblknalzg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gywzqvqwc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gxcaiqecf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gjdixtplh.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/geurgqqnw.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/goemurcki.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gmqrvvksc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gdppeprwb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gtpavryhl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gvtkhnbbk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gxigfwsxh.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gmjpqhvfy.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gmgairugp.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gwhiqdkcq.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/garcoyydn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gaylsldad.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gbkyopdwi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/ggmdizoiu.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/ghorergtu.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gfozxwzmi.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gbxurtryg.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gjqhomjsx.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gixuofpfc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gjvuusfec.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gdzrofxwc.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gwztlnyuk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gsakihxlr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gksgpzkdq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gcvgffixs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gboyapfyg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gcblkgxqn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gxxzyjgvn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gwgskvuhl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/glnwaudmk.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gxhchnxje.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gcejpylkk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gxvthwybs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gaawfuduk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gkeboevdv.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gpxyvuzqj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gwhltsdwo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gdlaqwjoe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gixnavpbf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gxrhoprqx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gasrmlmxs.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gxcdbajzq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gjnaicurj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gihalucya.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/geozmxtwo.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/glpaxauwq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gpcdblzme.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gsxhcklta.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/ggvzbaojm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/ggjjgsnke.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gfgdpqkfm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gbiizjuna.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/grxpufoyk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/golgtsens.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gjcajlmic.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gxmqzmetm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gpvcavfgv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbulwtxof.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/grejaukht.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxykytccv.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gvjkrevhq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gqwisoshx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gviajxluc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/glpkgixle.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gipvmjxyz.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gaeflatyx.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/glhwtkbov.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gngnxhzgc.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gmxxjyoxg.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gdokfsspb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/ggxwqtpgc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/glkdwdyzb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gywouneei.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gfimurfhl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gbsqxkwgf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gkuogmeao.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gabbusqtf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gllcufgtv.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gnbckudtt.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/grkxupuqt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gemabgajg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gtjwmjbws.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/grcxnflpj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gstxxpwmk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gqymsyehl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gimeyacnz.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gclioysua.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gszqmaxww.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gvvjghgxk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gxjcrwmwf.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gowtfcuet.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gstyharpm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gplexnync.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gnywmhkei.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gxaqefjql.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/ghgacximl.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gguyxxlhw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gkityvlvj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gwnqwgxrm.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gapfyccam.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/godsrnava.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gotpaqtrg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gomhujegt.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gishmwead.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gqvpfybkx.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gvnndvkvn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/ghyafwjsa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gszdyocyw.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gnquimexf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gxdmoxeiv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/glqhjcuei.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gunzeyxav.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gagbrdxiq.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/grjltcvlh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnstlcpgu.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gcxoawiam.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpfyphgqk.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gdfrcneth.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/grcaytdgq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gacycioes.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gmzpbsqwr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gaquzrkul.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/ggrglkezk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gifhvoqau.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/ggtxfdhul.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gbrdqztxk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gpotegzrx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gxsoakvuk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gxntnfdwi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gzmgnmvik.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gpdztrmpu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gejwqzttb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gvxunjvij.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gxsiqjqas.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/ghiczhxbn.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/ganaexrdq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/giycfftjq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gawlgzmou.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gwfwauccc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gxxmjyjvi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gyfznuufz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gvheicmzn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gsvjmmlrj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gljjnulbz.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/glhmeafuk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gnzocuoat.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gqbrqxucv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gdqhsqlmo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/ggbetwczf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gkswhkqte.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gjraaglen.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gbpcluesx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gnjtaovik.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/ghktcwpri.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/guytpmaev.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/grkxbifnm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gofahhawg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gozwfbntt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gcshkjgno.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gtiqxzowa.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gyobwoxrs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gfgikrtqn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gxjqtbpyl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/golqwtucm.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gqakbymwu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gxvmvowwy.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gcwxqcdgq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gbanokutl.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gfliihiog.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gysrsbvcx.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gumusjtfs.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gihoqpmzz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gioikodiz.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gxzwwgxur.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gybdchwgm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/geawykxce.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gadalnqft.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gbpkmugog.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gqennxqmx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gwwsvhqib.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gwyqbomsp.sHtML


<!-- 参考信息 -->