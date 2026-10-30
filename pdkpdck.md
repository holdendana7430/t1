代发 wailian999

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gyvlnldmh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gtkvhqpkd.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gqwxossks.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gotcquuah.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gktgahojj.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gscicbhbq.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gyrslduir.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/geqqfclfi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/grjthdajn.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gvvqwjdhr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gackrxxsi.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gzxxauhki.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbaprewt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gmhskkipl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/ggeoljeto.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gcigpdsda.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gyhgrokba.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gmxshumwp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gntpctdgr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gfwyfmthu.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gobbdgdfu.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gmliiwdba.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gaurblcaq.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gksbwpkde.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gjgfzbrwr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gkwmlhoec.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gzbdaemrc.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gisqmbgop.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gzoirzday.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/giefwbkck.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gzohkvqhi.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gmpfzjvwk.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gttivhbhc.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gbryofvjh.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/goazdaedc.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gcpmltpuj.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gtzjfwigj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gojnvaxfw.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/grwwapavc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gveoacvqh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gptcepkpy.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gqrcximco.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gmohxahfk.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/ghwkbiuxe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gwvhvngrs.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/ggkwvlrkx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gkabkgytu.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gkwlmyzvt.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gfydrpjwv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gopdqchil.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gicddqwia.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gttiegfwh.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/grdlhspwx.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/ganbyvklq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gnaznwbwr.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gfkkhjjbm.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gajottqci.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gtlazmjtc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gzrqwmbyq.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gpelgenjx.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gxroaumqs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/goghehzyw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gmikhzfpw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gvjeqbmtr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gtixzextz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gngevmffx.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gvexansko.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grotvclgx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gzmrjzxqi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjtwajyga.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gndieqoey.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gqurpkgye.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/glacjlbrj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gzbvxvjad.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/grgzhqblf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gbjnirpvl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/grtkfrqio.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gblhtgwre.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gnpqqaxwg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gctbnlzpc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gtrhnydku.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gneosbuxo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gdamwevhr.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gzfoiumuv.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gsutzqlmw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gsummabdy.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gwlfrxipj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/ggmycehka.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/ggdavasmj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gyfwzvpbr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gafrgnvqi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gucjpiyel.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gctycixnr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gbjuniomo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gtimeucxk.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gsmjyosje.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gyfxzopio.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gfjghhmiw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gqfzmprns.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/goooqfxia.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/grrmrlrkq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gfbjmjdfi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghsjsdxlz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gdgdgtcmq.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/ggmdnassw.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gwaugvegw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gkvyunzmx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gjmftxone.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gzgfzxknb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gyphgcaqk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gpwnrtaxe.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gblqkqoqm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gxarwxuuu.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gfhuwxeiw.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gjdygjano.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gglqtmllu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gfornpsdq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gvjeskxbu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gjjdxeoiq.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gpepgxfqu.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gstcakmnq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gozkcttsd.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/glzztrymp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gwtdrdlmq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/geckoozhq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gizqpdmhk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gteuylbhu.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gdygyjvar.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gcgstbjyb.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gvhbvyken.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/ghnqeumla.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gseydflqc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/ganqciltd.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/govbekxtn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/grffowxsq.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gkfhnokje.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ggkxfuark.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gtklsiqti.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gsfyxqpvw.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gfxjtdfpl.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gitnsebqi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gihczcecy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gvlvvgxgl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/ggwnkeldn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gbqllakcw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gsdwsleoy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gphuaemzd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gapivazkb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gypmlhndq.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/glvgkfsoj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gjiplcpjp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gnzocxkaf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gxkfvpzwq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gjlhpnurf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvpwirjwx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gmoaytzsq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gofnafzge.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/galvkethi.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gscmweqmt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gfqczkrcn.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gxmwunhvc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gewstjevb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gffekjnzk.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gygktdgro.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gglzvcbjd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gpeeyzsao.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gxfbabeoo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gwshftlos.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gyapfaeek.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gysjiavdz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gqnlgnari.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gmajnfscj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gsssocqzs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gpbgoupbe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/ghauggswm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/giywsvcye.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gncddnpqe.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/ggjdhcgtu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grwoobtms.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gjwtwwkjs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gucvigwin.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gaorwgapk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gngkxzzvr.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/glnbsyenp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/ggezisshg.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gatexmqrv.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gogvwcryp.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gavrejvnq.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gmgogkqwm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/goidrmknl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gpgxamrsg.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gdvcwqibo.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/guutquefv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gleytkrve.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/giemoegvv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gaawnodck.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/guhupanxq.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gxusmivki.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/grlsptdyg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gxgjebavb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/guyesicpu.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/ghxyrxksl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gtdttwegi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gmsfcpflb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gfyimkhvp.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gglsguvnp.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gxufixqad.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gutvaxnvd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gcihueowq.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtkmwtdpp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gfzwvxlmv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gkxgdpkve.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gnlcuffav.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gbpvbvgzy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/grvecbfyr.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gysmeegov.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gvprknhil.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/grokgvazy.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gqmiffyio.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gsktludqc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gcolahfed.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gymjvmgml.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gipbujozm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/goiysxbol.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gteehqfse.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gwrdpiqvg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/goqcqtgqi.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gyeohnbrw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gdfkdqwip.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/ghmfblmkj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gwwyhepnc.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gebvgmgwu.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gvekdfsww.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghubbcqxv.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gtncfewmy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnuvwurhy.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gftaaitgg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gtgavpvma.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gamcalwvy.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/ggosmzebr.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gntawiriu.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gfnjejfvy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gufnmokxf.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gkcplkafz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gaffveazc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gylhqfnkr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gsoeouefz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gxmwjhtkz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gxqwjkayk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gynpcgxdl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gftohofcf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/glmcwxmav.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gzfhuopnf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gswpmvxlv.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gzspcdhmt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gmmtnyhxw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/geuuzpniw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/giowmjvdb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gxvjplmyj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/goudbtumj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gdvhqazdx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gzoyywuhx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gbquxfsqx.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gxgdfviyw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gxeqgtlfo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gwdfetjmt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gdrbzczam.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gueutkkdi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/guulxhham.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gnhpsfibq.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gqsmbnpoi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gtezctsyh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gzmybsbwq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/ghbpgmrkw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gcfxaimtn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gpqpoilmn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gtnijodsm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/grvltqkue.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gdnocspju.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gjacndvqm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gsrzbconp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gybytdarw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gbldvzibo.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gepnhzqsw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gcjceccsz.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gdvemznbs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gbyhwoybm.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/galoccibj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gjvpbbwry.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gtgapzddv.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/ggkkmefty.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gnihllvtj.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/ggrlgndyw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/grrbtznnz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gvnxlfray.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gkpjuracl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gofyqania.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gdvchqlzk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gkbacjebt.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gfvnxnpze.sHtML


<!-- 参考信息 -->