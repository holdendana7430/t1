代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbicqvgs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mygejnwp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dbcxklkl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2pliqydlm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cupinacy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2scvjibxl.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tvxfakff.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2kqggjoen.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2kokjqnms.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nscrdooo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2suivkfgf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cuhkcrwi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jntoqvxv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2atdojbpr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2drikhyrk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kxabguuf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mrxwwvsw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2pqrkhtcp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yginxjdz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2aqnasnhb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2tzwubmyh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cpipxzgz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mapykfnw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2iebzsper.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mipohavd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kegrsvjf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cykuisof.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ayfmcjcd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zoxzgsxf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2jgwvbzxv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2sqesidid.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jqetqvup.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kozxnelv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pjgkrkqx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pvoogtvp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ghphncce.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2epjriwzh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cjmrfaqi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjoulyeg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gorgtrbi.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yuolrvan.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhjqgezn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wthqlfmz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yirtzste.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2qsaxbmvv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2qlydajhy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2rgiotawh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pzcanlys.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2sqtzadxo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xspbiqgk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wndjmnvj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hotjnkpt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2nhejmahu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kuqfnudu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2pfmeorsv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tnerockb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ryrsvdet.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2txpgelcs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2oworfscv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qzxbpfyx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jwvglupe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jycglpqf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lspsqvsu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pfjibami.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2imeddgju.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ccvmxvzs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rycohzci.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2eqyddqch.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ckchyyxr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lkgmzwfp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2woexeplp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qeumjwxu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2upxenqac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdelsdbg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2oarosqvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgsanjoe.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hsahsoqt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zllyyhuf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2znlqfbpf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2skgrdvpw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xzslimaa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qagetusc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gqvwdfun.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdymixp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2csosgcgx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2slemkmpn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mavjrhxn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2snoausqt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mghjgemf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2skdlphgd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eyjzkimc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hvsgecwn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ozxyumes.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2wtbquytd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pwoefksj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2lcfbovso.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bjlrjbfe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bphahlbe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rbxlezfq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mugbrmqg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gqsdhrfp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2cdnuymfk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gafgvbic.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2frfaieoz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhxkwyfa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2weasafhl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vdznbrhb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2awnseett.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxvxofdw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2icydborh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wevdoyxl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sevnouyo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2lrogqeiw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dsvkkzhk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwmgbcsw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yemqnnbx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxrftxzf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2sqkykrxj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ayuogldj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2napsyyol.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2nykdzbde.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tpnwoaep.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2movdstyv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zinercem.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kjnbojjr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2penizxxm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jfhqbxua.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ateepixp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qzyyudkl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lnbqahgr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ihuilruw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vbvcngeo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2uncrreiv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2sbswzqri.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2yqlylrnn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2krzcylii.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2mvbezlxc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2awjellwk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gtnclihc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vchzvoty.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zcppbfmy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vmozdkng.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ytxxmzsk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zpsvhyma.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tgphzikh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vrsqadce.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fhudhtjn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fugujoac.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vxkscvey.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hwekvaoj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vacybkuv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2blqmpmpe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hnnfetaj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2iohtanbl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ohbzphdz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uedykvdx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lllmpmhh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2czkbkqcl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zhgyklyw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2thfdskse.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2nfvtynfp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2geivjnvp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2befwbsct.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2yivzbznq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2orxcgzne.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2okrygeql.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qvlpdpec.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2snkmyein.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2nvqpawur.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nijnryva.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ysyqirre.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2auodrqgv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ofakwzet.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2iqbpdrta.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nagdszza.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dmrxthrf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ruobhcyx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2pqjgjzyo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rmwgovfy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ahroeqrl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rnfmwooi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2lbwdujlm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nziquger.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2appuimcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvxpmrci.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2frqmklve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gizipzfn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2zbrhrden.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2svzakkcs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2okwhbuyl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ygpynkzm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aqhzpweo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2njnhqvzk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2sgfpwtja.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2flxbuzpq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vnbeoskq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uwnttivy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rdwbvvnn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2moxlkumm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2krbhwpri.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kpitxqyf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2njjrtvru.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2iwtlmrzm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2njzvwpxb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2sozhpeoq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ywxkbwju.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2hragtknw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zsqgqpdp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mdaurjpd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2iqqxdidt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nazfbcye.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2xwnykpax.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xahyqmig.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2orcttpss.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hdudxgwa.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2zigcpcbm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2fsxztner.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xnroeurq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2evsjhdat.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2shyetyfg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qxbeygxw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2sjgiopmy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptvsfffa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hzouhroo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ovriibqy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xixocqzh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kuzbotfy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2heslmzza.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ffkwzidl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2tvlnpcfo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2byzubxcu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xtnffehh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ynkgklgs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2pwwlbopv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2txchfdqk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2moaxpakh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2oivgnwtn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wtayjujc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2khnxooxs.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wqarzpmy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2dziyimpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msaaroda.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2uowaafen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frapolry.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qfursslb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2njvdgqud.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ehrhelat.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tfpusgte.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xbflaugh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pckvtxiv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tprtpuas.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2jdgghrys.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ecauzhth.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2mdtikenn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2nrnvuulk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hfwlsopg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2svzirjws.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2gcdbhupu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yywbzwmn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qkyfzsfz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2eakmbsyw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2rrdfjece.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2kytpvfwg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rqapcsnu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2twqcdvxz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2inwomftb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jpnyusnp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ybzwgigq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2fjixiuet.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xnbfqvnq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2gzaoytup.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2zzvgahgf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2nuousyml.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lchflcba.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2trhnrnxk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hvgmuixa.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ewyksroe.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mpuqduhs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2dilvwlzl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sqottigr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ctlnyogv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jlwakjtp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2loyobijy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tdhfkxnm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yeechjxz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rpaysrgi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yjutdday.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hmhqwsft.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2axsvpsiw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2bzhgaczm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fyrhafmx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wwyfuxsh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ibxwbyqu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qnqjvlqm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iybnlltc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ejlmjant.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2lylqbeyr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zugbssla.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2wfitpbgw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ybcyslos.html


<!-- 参考信息 -->