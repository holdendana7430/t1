代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixtxmzha.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dmbjrcmm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vhrdpoqj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xvatrell.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yacjemgt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbettlxn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2znoqrxjd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mwcuanpl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dvxqqgeh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tplhkpog.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ticxlbfi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fpwexjuz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2iktkvuga.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qnofggjj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jewkrgpl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mprpotwf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ecxckjov.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hqkadowt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ejtjrbmv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2crblbwvl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2udryflwu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qlynourb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ezufndka.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rbmqxasb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2pgfvuijv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xqyjixty.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2sptougpm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vkpkknka.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vgsrymua.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gxtmjjqy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wfzcgiym.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hctnpbtt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ldmfymcv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2wfusnrve.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tlnxrryw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zocwyaal.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2yqrmgvgu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xwkcmpsy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oodqcaar.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2sdmkbsmn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pquxpzht.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nmevlqyh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aycshhdl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rwrfcvam.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ldnnfwef.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tumcwoht.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wqnxsaqe.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qgslvtqm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2syrybpjr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rcxqpsla.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fghlthxw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fpdanaex.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2slwrlqxt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mblftxdi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bhicrpxj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zconfilg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2eieddvuq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ldvfpjqs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qckkceho.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2klgrfxcr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nxpumcnk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qexpavub.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2iylcdrfq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gkfhiavp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jllwancu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2tmlqolyg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fltjvpra.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jzhjkrva.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2omdtdwej.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2yhuvrdcs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tjhnayfp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2dfqrmryd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pcatiwor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwuqeuyv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zbxwcghy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qceaclar.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2eiubcfav.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2exodmebn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qpumflwv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vefdweqi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ijahvcog.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xyloygny.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2keebugrb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2apwwnggm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zdxxdhms.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2eeagskca.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tdudpsmp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2oybetxsf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dktqzmml.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zjmjmmpt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vywrpsdl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yusmosja.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2utqotcba.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xjxizzeq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2svpmshji.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2iwnhppvy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ngourwcv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ygipcgep.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dwjnikbp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2uakqcgxw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nyujtpfz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nzovpurh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2inrnbtje.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2toqzsbah.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2soraiyvs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cegacxfn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mxbodjhh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ypwmaowr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lonsrnnk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2iwvyckel.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gtugmyti.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2blrnwwix.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wymrreoj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2czvbbryt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2gqflihnc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2utqzfkza.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rybmitul.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2czidqkph.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ctollbjl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qnmiyqhn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fdfdbydf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mzyvrhyb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2iapoalre.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zuvywmkm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dtbjkucy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2srgwrxat.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fakwekaj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2oindwhhc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cbwatvsy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zdarzuzb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bxczzkxf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2srznykrd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2speilnox.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2lyetgrxk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ytbsvcmp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dtzltajz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2scwgmfff.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2whxewgwy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2evqscrjq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2cgimcjss.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wbacjvdm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lhsnlthr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iysecefs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xdgzgafc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2owfgdxtf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ihqidsnv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ispobyxd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wmorlphl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zohmxbeg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2lxihvjcy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vvtoxqdz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tpcwrewf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qsokjkey.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dfuoujsk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qnilymvv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wckdxvvw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cvbuzqid.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ayradaxg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2viwmcuie.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lipxxsmt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cyviqroy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kjzfouez.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2muhwnwzs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ivzwzrsv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2jnbbuzdc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nsbvdiqs.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2umeqbxxe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zwfreztw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2oepfnlme.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vqqugaxi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rnvkasqh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tiammsvv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pcatfjyo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2nsvzteys.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rngssdht.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2juarahuk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ifsrxtab.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2sehxfhqy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qpvqooms.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xntlvwwt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2eqozkbmh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2gkntjdkf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wtaawaxm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kvbaoebj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekbontim.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2tnbqytsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnhvmpzw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2iswrtbqw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2evtrrvjo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2gumablox.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rakfbozq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ohukmsfm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2bofwpfgq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2soetvohx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2iwfxydyn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2dnxwofsv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cghpudiq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2zlkebglp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2aycxowqj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2unowcgzu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kutvbjjo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2yyjqezrz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rkytkqkz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2unbhkyfy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wcmvgthk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2szioself.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ppekeplr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2bqkvnmad.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wtiljmfp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aoolhkgq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnxaqhnb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jszzmiev.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nnlocxib.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmrhnpgj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2csqpixsp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2nbxueiqg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2guqlhkfc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwjbpszg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2meglpaoh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2advabumj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2itsspytv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2gslmrkpo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2heztpvay.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2agkcyolc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2iyxwswzd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ugtoywwo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ukzmbyhg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yrkupedd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2biyqxesl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ojpdapld.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vxazculy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2hyidnfel.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2rlfhrpcz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nlspoesx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vplxaugs.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2izquzkwh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fezkbjgy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2txonxmkr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2lyglkshw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2pcnefaxe.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hasesxtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntdlwfga.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2rlhlqgbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdalgzfl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qlboyijx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2oxiazbsb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2osjofwyh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rcdsntwn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2txhbzfyk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nesbmrud.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kfgbiwzm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ifazjumm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2eeupdxso.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dvhrbbzn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wfsgtrod.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwbkoqob.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bjxwqwtu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2cdlazpuf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jqxuvyzk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2vngkbkjz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qbeopiuj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2wzqjhopz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2oojbdqho.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2cxmvkilp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cbikbtpw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ymbvsgip.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2igbdmplw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vqrxzoql.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2pxdcynmv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2catollxe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ycrqktzv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2drlkxuxy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2eduodrvj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gnzejhwz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2eolgxzgm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qxrlyjuy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qhacxfna.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2peaxnuts.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2mwvfxmcv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kvnrchpo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2mgointit.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jusodamu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qvhunrsb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2syztbiuu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vzjuaeqq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2npfcoatc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zlsqqkqx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jvaubciw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hgrfobsz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2dypxdlfh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2znyrktvx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2woclfalf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2deavkqvt.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2umlgolrr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cnqjzrqz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xvlmffuq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cwhijawf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2xqjszbts.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2bvqrlesr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2asetkrll.html


<!-- 参考信息 -->