代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqkjyzsa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mznxevtn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qbujutpb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tfbgkgrc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ptlaeuoe.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvgatbbd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jpicqsqk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ygajjyak.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2bqbcjczw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cyreeovh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gudniack.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ggcscnge.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2etntroam.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qmutamkd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2udcumkkq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lunroics.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uqgpptld.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ylqfutnb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aezeygdv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xkkkinqh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2xjaailfu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tlckxsca.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pxumgwcv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gfyujnlu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2aldmrvvl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hksydgmj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xryajcoa.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bfyaqwll.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2tayllggq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ozmyspft.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lgwzxogl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mqxjwhvi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2eumdblxn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xbifjqox.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hfladatx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wcmpdmaa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2rneqytni.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2dboxndnu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uegebnge.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zfpcdace.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2suvuhrvy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvknovor.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhtojamt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqmkvnod.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2akeofwsm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2mydjdalr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kytuqpqf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ztlhitib.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zjfmbhda.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ttmzgvoc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yyzbnkqd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2efllgnaz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2bjdzcane.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2jqntmebv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xthxeohj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zjviixgn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2lqfhcepe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tbxbqfse.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jjyytkpy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tpdgckre.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gxhgxbks.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2dqsgqzkm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2adclmkpw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bizkcolv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2sqneorln.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2lqkkmpoj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ucxtagur.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ehxvwqzj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ulssgvem.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2wewwddub.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pmxgnwty.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rhfdkjpe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ywoejfds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xihdicom.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ukiwapft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtgxajup.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zyaeirdz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lazgankj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tnesfglp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iudysppl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tepyjhfw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zqadheun.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kdqphpnj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gwiebyvc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vywcgyga.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2bvmqirhe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2aautvlka.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kiageuef.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ljpeczjj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2icxpuydw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rufemyfc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iuwezhah.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kxxzdioa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ylayqtjt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2hknhgmpa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2nitohcne.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2noadtmxp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wmsnqsyb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mlhtkdcn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2auxtbshn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ptxavwjd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mgtsdyay.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hmuiieqv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dznmyehp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2egphfrah.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqmfwzqf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cwjdvpug.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pmiubrsc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nimkwyjy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2udfybxlb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mryucldm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bfsmdkou.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2uyaxzjdx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ftcwbgzp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2hhoijwjl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2eycenjaa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ewgrgeqp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2munighdx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lainiwjo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2joxgittf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bpzpxzfb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2qjyntyew.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yjqshqty.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wrtxccld.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qxqmiuuf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iemrurhd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2maflesao.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2eyowcfwr.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bnkadtds.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zmoyoppt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2bkoorgqd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2eoqbryiw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nuklnpuh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ppjlhpne.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2uispshzk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2pvntribd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pwvlivrt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ugtyqcrq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hqacrgsu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2npigctkn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fgvmpyeo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wkdybfif.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qcnzqvbc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uvlckvvk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ocddsmtd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rremfakq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qswjoojr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gcibguct.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gnzblent.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2bmbzkgta.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aatucpgi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lruxyhbi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gcjmqzfm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mcfmtdsr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2eyulpbry.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tcxxqthc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2gkamqcom.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2cumeqzab.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2xynfvrhe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ieaydtbl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wnjhrool.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jgrelypp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2koekvool.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2suivglgu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2gagcedwp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2yxlemoqi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ptasuupe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2yckzrpvl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2pupcfrqt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2exxnxuao.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tvtljamp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ygyjacwl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zszjtwwa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2cymabbcj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2clzfplof.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2idncnxaa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2smdbmrej.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ijjgsdqi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rraalbxz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ddlazsmk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wvtgukmz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2agnzozbg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2udurjfrf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ksxaqdum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmbhioeb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2pdnwkkdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nimqfbrq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fbipkwvo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2dswtapmd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jvifxtaq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2larnaovh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2boopedve.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ropmygab.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2rtdzjrfi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2atmplvxc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gnyarkew.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zskfxcsn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ezmpgaks.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dtbfnvqq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bwkkqddj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fcvnqgha.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2spxkijzy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2fmyujcqn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2jkycuxcz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cgzhvyai.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ofzphlcr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xjhurfac.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kmlsnlcc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jqmtdbyz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tmjjyzrt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbiymxnb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wvzirbec.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bcmppeqa.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqcqnnlq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kkgvbqtm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2jmmwswdu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2yjwocfyb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qlfwsfqb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2eaxwfcsr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ttobrxfs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2mxcmlobk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2rehpdugk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mzsyshsd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2bgyvtzfn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xhchnfzr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2mzcbipxw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dkomqwqm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2obcaaobi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2sxaynihb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2arfipymj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qhzqdiqh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2zivjslmr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bzexeajm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lorslckx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vkifsnzv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2eybvjqyj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pezuncag.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gkrezrmx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2loqzxuyu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2kpriyhte.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2snimysmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkdmzomu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2cvtisyox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozyzgllx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2idawsbtr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wpoamhhl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nrxfhwot.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jrlestiv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2grivigjt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2edgagxbw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wdabwnir.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2drgbefsf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ktzecgcd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2uenhdfwc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2hamdfeuc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2useexdjm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2zviftacs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2lachhcfi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cqrdpguj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zbcqccss.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sgsnrjex.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zomlffyt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2muhwelfe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2gnqozxgl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ytleyetl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gypzdgwk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bqlefxcl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2nhtdwsqf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2exrwxdum.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rngtzmuk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2yquqxdbk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2fxfxigtk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qwrcflfb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2siuirxlg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2flhwtuop.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jhjscvrb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jubppndf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ytkcdfzd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2vecmygqf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gdxjcrhv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2tgwoijkn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2goabjakn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2atyjshtb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2chazossz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wmhtyalj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2pbfjnrzw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2eydwnmjz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2agabhnyn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ieflzqrt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2dzalxgdu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ytlebdhe.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wisqllmj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2bnizqhyu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2kislmhms.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnzhetml.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2vklobiod.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2lvktakin.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bahlsgcf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2cippfdjh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2tbxzmymy.html


<!-- 参考信息 -->