代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fcjlrmdo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xurnhgmb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3spfchlua.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fumauktg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tbaswbkx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hhrufrfp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ytaohibt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wechewnd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lpbrtlmq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hyfcrdll.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fmiwpehm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qylyyfte.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gsvtnzrm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3bcaxlrac.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bjgbmidz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fcagjirs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3alfapjfu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jflvdcqb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qqpqmjuc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mdnceotz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3vstxrhrc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3keoxxcmr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3uiknafxg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ypumakyy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qwenwbvr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3oeqtpetd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3qpbszowt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hbkaclow.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3etqhfzgi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xqdeepzp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3lctcoarg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3cegfrnfr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3sryvcwqq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3oqgbzosb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xeuwxpot.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zlopjkjl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3astsfgbo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jtfozysf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ssiqxkij.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3scljszkr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxjpmpcc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qomxftvj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qnnvlfpu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqskfty.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nmprzplw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nrmbvmah.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xziebgyt.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ejcalbnw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3auffbqts.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3uoyjisaz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dwwhljcf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gakeuwdn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zwtstjjv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3iyldtzgy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gwjcmidf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mkskgbwk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wgmlbjho.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3erunukdm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yqwbwhxg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3xanlxbzs.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ekfbipfj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3biplarre.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pikegxjv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fxrdztrk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bymjyvhm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ltnygodu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tbqxoymc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zwbkffjq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3kxeiishn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwkgpeny.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3uoguetat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgjlprxl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3yrckzccx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eauimtuy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3djmkpotb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vrzwxdxu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zijyietx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iaprzpxz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3txsuzqed.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ubiydire.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3afgbntgw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3bglcaiva.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qgopotod.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wioajhxk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uywqslvx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rizlumzf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rjjbjjym.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3szuyiyyb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qmkdlorq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rewzlmwu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3fqpbnmjj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3waiebuev.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wrvkcgcm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zwekalup.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vwwisqqg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3iosihgut.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3vrhuzttb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xvprannq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mzsxxokq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3uudwuuxm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3psmnadkl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cjzskpeo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lggactqu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dgxmtxqe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgkbitfh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3fxubxndf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3niyyvkzn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bwuuvbku.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3yrrgilqw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wyxuyubl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3eomobfpn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhdkqcae.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyhtpmab.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ywvtqlpz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qxsuszbn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rshwmrsc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjmscbmy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zdskhtvk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lezipbca.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jqgxpose.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xnniuemu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yyihlarf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lctmyhfq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3usszbwsb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lpuwmpfl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3runzorbj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3onkfnwjz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jvqacrfw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3oejdyoql.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gjjbritl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lvtadmfh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3bkowkreb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zjnoykzs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zmczkzni.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wgdkfytc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zbherfwl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3obrquxyk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bsxbkgvi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fufrphlk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3igamoyvn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vbpbkvfo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aaaipmbb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dgffjprc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ingszdjv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3awnizkqd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ymswsnvg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xdxxwxay.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kfiulzur.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mcmrhxec.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yfrjikbb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3zqlspbvq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qzrvquxr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cimphcrt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jylivkrb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tqpzrzna.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciodpgtb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3fkkrradr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3jyfjtyef.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zfxyafas.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3woxgkoex.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3bubbazxr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tsybzgwy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dshkwelw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3bblwelag.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nlmrwlhk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ukjmmrio.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xukkgiar.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tckqzkyt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ysfvidfd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3rqpgxrdi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dtekybxj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3gyincyrn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lseereyj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ttznfkhu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hsqrixvu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vgzonlus.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qdhzmrhp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ebjqtrnr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3vjlimxah.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vvstejlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtksihnz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dsayxgox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qagxusqn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jniopokp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uiaqjqej.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zmfmzocb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3uicnalqm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3azcuzxot.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zditlfod.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3sdebtcjs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ihvvhbvy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3cztvjpgi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uayexljq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3srwihvyy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3rqjggsrb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pzfmcpcy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3klomknog.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mnezqvib.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3oehvcdxa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3gaiuhfle.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3uyliwata.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3grjiuzpi.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tafbgfzl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ltnjnwfk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mtyrtwci.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cqsffrzc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nyunrgor.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ssgtzfsc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqbkrcx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ovbusazy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3dnqforuy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3akdyifux.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qrfnwekw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pbnnffvv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pgojxqux.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3bbglwwdu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3exuljnxs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hoykekdh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3btovidem.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3xjymqjst.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gcmlnvgu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ryabismo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3elyedpjl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tbcktwsq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3bqyjrzaj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3oikgwulw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gldoxkkb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ididstmq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3rxbdytgp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cqhfmnak.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xgsgfycw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3thknnmce.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wbkkhfri.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xiwpjcqg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3hldcurwt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3bzztjays.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3tgitvzxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqoxmfrc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmsaunci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbwqniwy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wlegrvaz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ntfzzssw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3psvxwmdi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ulmvuuws.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tvdaikgz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tmxnczzg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ahowptob.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3easwqjhr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3daddwymf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jzzhzhsb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ztvtizgl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3atfgwkob.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3xriqveaq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3velydshb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pxehxvnw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3iipcdvmz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ypjkfihx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hwyemyps.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3akfjitfb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3bvboovun.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3gaywuemo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vvenzabo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xorjbbwr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tlymkqmp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3kcwgydeh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3piqulyps.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3uiztacih.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3qptofoit.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3fgxhmian.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jhmehmjk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gkdnixhj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xdisxarc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3klhfzdpk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3cydschhz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3vfjwlsny.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3akcnyjzg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3iautjgtd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3oxvxxaqi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nxjzudiu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3fntsznax.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ajlpfpcu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fhjstwmi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hmyxafyv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jpbziwiy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3bngfabsr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3qjcwyjxa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ijaxcfri.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkejjjws.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3okdlanwz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vezbcite.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3thpxfdvm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3auskkasy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3nnhqqhdf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjwihcao.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mumxkmso.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vujeqybg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3xjyycmrp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3igourelc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3olqpavfi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3pjwiaryo.html


<!-- 参考信息 -->