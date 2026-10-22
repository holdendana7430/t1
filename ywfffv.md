代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vnouruwp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2yizsgxnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyqtkfnl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2qpjilpaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwpcguue.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zjyaiczh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2gzocqirf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xezixbun.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ddparckm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqnuweyj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zrijgigj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2suhbdbea.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2staxhjdb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ywclnmib.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ncbviajp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rwpvonep.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jbnrefjw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mxhmcqze.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wgyrtccx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vfokmbni.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2muvneevc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bznomzeo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gmlmopfi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tjeloxge.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2smmrykxl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2kfniytda.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pbkcgely.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nheedxrt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ottlkubz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vhcgyscn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2gefhagar.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2yssgenvj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gfxefzhq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2todlymuf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bvfipcus.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2trudohgy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lfadxccr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2abhuyhxh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2posqelvr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tpfkoirf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ztmbobog.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2filuxhjy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wnozzifl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yvobowal.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhqcglqq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgqlefba.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qykegtno.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtyszrrs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tyddraqf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2vtcyjinz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jvknvzms.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mlbytton.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vtrnhufd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tyrrackj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kxtbeglo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2tdcedxha.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2babmkblh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2eslgjuvn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kzjxxjmp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xhsamull.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fqjrtskg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tzmvsfgg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fcxwuqvy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fsfzylds.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2xuykdepb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2dtrfidoi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2npnurxns.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zrradxqy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rnlmviek.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2eamctynb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2khsaztby.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2sedweyow.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2toeddxhf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2sywajkjd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wxitybbe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2rwlavzim.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2greskenz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpxvxqng.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lxvgfcsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmmophby.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xvsnwlwv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwlvkmbz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xdjyeohc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lemkihig.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2eiwpefcw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uibzdztk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqawszip.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zahuypdg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjogqgqc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2kiwpqsfg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bcvntqpb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mjsgiyxc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tuvmauww.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dpxphjln.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hztxvqjw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2brjukyig.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mrjagxdz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2raxlqavy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jjgoekku.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2evgaramx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2nqmyfyhx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uguvxehd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nrpsqetb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pldwqrvk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2mllilawy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mptxwfnz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uwuuacpm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dculdpnu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2aytvenda.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpfeqpbn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tbmdmswp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zqajlnbz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2otsgtbgw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vzdhvbli.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gnphffqr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nxeelfpu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2akzxoeby.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ppnrcpli.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2jzbwtujn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2juedpxwh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sljtypap.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2tkeooibt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2rvgtduov.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2hkptlsnv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjyrznoa.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mfztnwcf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2imzqozyt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2swnfrgeu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nwxjajvh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2brctwvct.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2iaadtkeh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2nogbncvg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fispaetm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2afqydnyw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2pkirtbyi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2nypfbkyw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xefareip.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2liljfjfy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2apltkpah.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ozdolpfd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2khktsxfe.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2snmvmjik.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2iilqhnsq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qcirqioo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2mhmkabje.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2omczzord.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wtudeweb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iwiqxere.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pqadgpoh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gkkvvnzq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bndxrofn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yehbzjmk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ouyazxyu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ctjxwmua.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2njxcynhr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fsmsnuqm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dsiumqbq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mhfccxxy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2rdlxjooq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hgyjyztj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rppebtvw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yhbgynda.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ghopnuga.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fltfqlxy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2iyleygwf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2pdwpkwix.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvkkrkfe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2monpadvi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2gjprbuyx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nptwaeho.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2hfgpengj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gkzryosw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nxuuihbd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2napnbljt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bvjknxno.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lvisxfnq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2puqqtmpq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2mjvuoauh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vpoxexiz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2bbkiruyp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2mlhcmuow.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2etvoaalj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hidpcgbb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jhsrupkw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nywlccdc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qnvzfaqx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ivhgksjd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ncwvuzii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hiuzjewh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2etozeifg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lortbtqj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2szrybljf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vhejziat.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2scqjswsy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2biqkzjkc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2frzvadin.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ftkebxib.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pkjdgkxp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2kaehnoqk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2octovhti.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2cxqbavkd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qlugljvg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2yurhfcvy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2stmbblnc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cwortljo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ywiwhwds.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mpbtcajm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2kvynrmcj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2shyefpbn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2twwalxoy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2rmdrzxcs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fsvarnur.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2kteenfkw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jxvdjuue.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2awewqgxb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2msrjumls.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rjxunfmj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioqnhmpe.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wlqsctky.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mlndlubi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ilnlcxjk.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kbojuwjf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibnqwuju.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xbftuiva.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ninogaxr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2hpmxrang.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2poudajlh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2wzmxqzlp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ovbxcian.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2yzpqgomx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2memgpaaf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iizdhcho.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2sqdsbmmr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ghbhyafk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qrzjyzyi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgzfsxpq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2rfjxawre.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2oiveqspf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2tbblsawe.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2joeebgpq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2eegbsviw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rdoflpcz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2hjhnwaor.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wdyerhph.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qsqhocbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mizqwgki.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ryehpqiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qiezrvpo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2brvwjmug.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2giulsytl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2aecbxlhc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fxuzevtg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bbtgbcut.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tdvqnsoe.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rpcrjibp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wlxsswxn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ixwnzzve.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2doayzyax.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2pomtcgdm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2adnjgbkz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mcpuaqsn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jrxlvoen.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kofllpdo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ffsgvayp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lzjmlmmz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fmcdmoir.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2wbaijxka.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2roudorhp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dclhkasb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2twckwmsr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bqwfiykw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cioyacfy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2szjlmnql.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wcucjhkp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2sbbosufv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2olahuoov.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cqwcwndm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kwqhyzot.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2necxduhr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rrjxnvhq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zebdqlgw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ydhvmfja.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jmqkipvm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xifytays.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fyayhnrn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ebhbegej.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2pfwpcnjp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2fgcglzcp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wgggcsoo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gamwzcyy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gvoltmbl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mpfcgiqv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2pfsjebiy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ssjiphdf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hsythykz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zecokhxu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2rnvpethx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2orpsyjun.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qliviovm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2abgzacfo.html


<!-- 参考信息 -->