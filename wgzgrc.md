代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwrcgdnh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3khzdpnzz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ygmsrdbq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3uwnygxyn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyufaack.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ytvigshc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bukdadcy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3oysfkvml.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3sfcwxien.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gznxovtv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tbkzbtii.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3irspxiun.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vvutqhzg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cfwthcjf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3huigacpz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rxpjkuic.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kaqzwcgc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3magtyxwj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bjvbjmvs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3oikopbwm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ysmxariw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wwqdnmgu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zcdehksa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nehqqgzb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3svzwtreo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3gxrittui.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ureykhvv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wgvhvcdp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qcejtgqb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3nfdihoga.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3bytngquw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zpckbxmc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3eyoqfeht.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3idkkfyoh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wloffsnm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mfwgowwj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bfhsoorx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3yxeomepg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vjbfqxlo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kcalwkeo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhgbbhcc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3azbvsjny.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3okritlfb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tutskplh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3cpojmbhn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ampgtuvt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3glccmjmv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ssszocky.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tlcduwzg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3paptikfa.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3burnjkcd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qamjnnpd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3euklwlkd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ikntrtoe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pgbucbps.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ezgxaavm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fxbdeosh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3phojwtwe.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zqwotcky.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gnycscfe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3igcvswmo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3dohnmeki.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3oxwfrnpi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ikmlrhkk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3uhnmmkfs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3dzkwqyhh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3mnduqiuz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tgydhmru.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rczitxas.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3evdilisu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wrwzgcxz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3advvqquw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mpcmveil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzopbimt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yqocmmll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bogqphhl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zrywzbfv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kdoafaij.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aednzttg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3axfchddv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qpyjqakl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3afqshuuo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yiwwuqgc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jyhhncyg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jzkwxeor.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3evutnvjy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bjvljzke.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3aytqwqvw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uricznyy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ebsqesnt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3camcotlk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3floidrpx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qhfoltxl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3viipvxux.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3arqmgmyh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qzbjbdgw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3diqrmkxd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uqpapycu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xtnnvfys.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3clsurysw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3sxiowxda.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qwsugqja.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3uarodcdy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xaavejwg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgatznci.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqsbozyx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3daglxfjj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oyzmzmgl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kimtwjuc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3krogqvlf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3agwtjidl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ffwvnhbs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3zvcjfnfs.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nfkbiddb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3esdnpzfc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3syrwzdrg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lobueooe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3tpyguikg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ozgibvaq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cpwofnvf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3witutlyd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jzcdixmv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hihmpwqr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bfwafzep.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3giwihgin.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3shhmklsg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3sopyaviz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zktcdjsu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3txpqwkva.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nbdxpzsc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zehqdsqs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qwuvconi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ahfsewsf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xuqnguxy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3umecmymh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3boueuezb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3acxlkbxx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qojonrri.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3upskjoig.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ylwpgibn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vbfdodfy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tfgympdi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qsjeqhnl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rbrrfzqt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3csqkqwaq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iuaivkqk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zdmgblrn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gahxbjmp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vwdbsfbe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rqpdryab.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jdyigrrp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ypinppgq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pdjcjluj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wnqafinx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3uziruxzm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3eesfhukt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jzaghkhe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ypcheonw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qxnylzau.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zmdsrpgh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lmkovyyp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qqiagurc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3tyomvrai.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3htfukmmd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ytjgnffn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrkeqhxl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3rhjcnosh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jnfhpfdt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vagzbznu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qndmbnzk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xubvxcgh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3muajyeow.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3soyhqmpx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3kvyfpcnu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jcejqpkb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lpnbuopr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3phttygyd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3puophcmo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oaqcvurm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gqqhvnby.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3yaypawrl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nqpvjzcn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3exdsehwu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gtvwmvgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bswhqtnw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dositjgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ressewtk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kzercexg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3baabpbna.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xdpdfejd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3seytqogy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wkayjlad.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cklcijno.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hmmqquud.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zjgcbtgp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pnwjhwlo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3opmnuigk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3cwryvqrb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3avxeyglv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tgsjkfgj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gffktsmf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jxaitapa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3lbsywrpl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3xrosqjwt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dnjaouyl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3glvlmziy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3reyvrjgx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qmmogorx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fnhctsez.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3szrarcnn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfwoazxh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pwrqkxui.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zfiqkwof.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubituoxo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wtpwxcpw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3eldmkyri.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ozbhyglu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbfqwuox.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzniqojc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tcptpugh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3cjnzayju.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xwtntpga.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvxcpesa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3xzaznqkk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fnjzbkox.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3avhtqpdm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ellqwpuf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3icicndpb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xsbmqrzt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jockvngf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3twzykdjw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3yrfgnupl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3fklmfvrt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3knsdtduj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3crwvdiqs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ijxbqqne.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3opyknpna.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zljzpgtb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3adosonvy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3rvvflrjl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3xpdxxskt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iuqdokhp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3foarehdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzqirfdx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gaydpsso.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3efmiyyhf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3eizcqrho.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qwweqffr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ilmksdzn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qvfpkujj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hbnimwvv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3incoxojy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ahhwzyjq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3epxnghgu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3uzzogavj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wnhzplpt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ieurdbuv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zqlkhoqx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sgcratvy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3onteorgc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3hmdomaev.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3dqpcumpb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3awzqcfrv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vzehprhu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3bwboszbf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yqxpkyus.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lupeheca.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ufxuuxpq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bkesknws.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ckdxqnit.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dvqokyaj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3wojdbdta.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vfuknizi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zbfrblhs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pdpyznxc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bvtybknp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zfjwffpe.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3smimtkuk.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3mbsilejm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3klqwbkpw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xacjbslm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mgopazpd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3txpvpjjj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ewzovuon.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3boumtsmp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3dwxfppmb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wthsmfvt.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3euwnbjwb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3syhcjode.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ynwvxxhw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hydqcgey.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dngmhkwc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3extbmljj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrlkdyfm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjuoyaex.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3zzbodvpw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wuqbtera.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zqpwnlww.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3lfacyqms.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fhcakinm.html


<!-- 参考信息 -->