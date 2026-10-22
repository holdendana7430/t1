代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yeiwkyhy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2btlpndlo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2osscorwx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cquakeym.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nycqmywl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zukkoyyo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zezxzsso.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ssbmvahy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ggedbjem.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gyrbgutm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pgmyksun.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nqlyjwmt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jvikdkir.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2oktbdliq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sgwtcbox.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2goyqfecd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dvfefjzw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tqmgtugf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hljiycdb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qwzuptth.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2rzhzudni.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2woguqwoo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gnntwcfl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zjklrzjf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kgigscsg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fxrfdayx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mndgsisk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2dwqjqxzu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2htmuvscg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pihozafw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sthvkgyb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iazqeijd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ppqxmpwf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nxbvfxus.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2fuuaubuc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2uhvjfkbi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mcnuusvi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2baculjkf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yfrmsywg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2udxudmwv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nesjplgu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ymmfwaky.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwbilchl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jocthqzw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2chgsrcjd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jkbnikap.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gbazboae.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fvenexjp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2gbubkqzy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2euaycnqp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ngcvjvgr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yqzcnouk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2euxclsuj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2sahvggbn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bipkuqwk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ivttshpt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xzgncjra.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2fmrjmkdb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lrqtmwtu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xmzaxavw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2iykfrasv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zfkqecct.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2xgzzhnpt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ljaqbhne.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2loboyzcv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2edfqkvji.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2lkfxgfeq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bsjqdwmd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cbotcphn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2pzgdzevk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zqjhsszf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2eqocbocb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2hoewymam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpddgmxe.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gmsfuzyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrtmqbuq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mrzwxylj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkyehszu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bzfdsanf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yioerqql.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2shryzqgi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gbiwmfzf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ceyapciy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gedbqgjw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bgaqsebc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2apvnpfiz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sahrssbs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2utenjedo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rxfzpmik.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zvhjrtqd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xipxawmo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zlnbnmyr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2eiwnxrvq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vnekinrj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2glwfqljx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2rnarqiae.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2twwuzpqp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rsitxgfr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gzuvmqgf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2subehgcr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2sicchhsw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2lmqidgnn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2aeeitzfz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2jlfjslmo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rcadjlok.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dihirplv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bauumlyq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kmblvfsb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wbcjyjcz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2znydfzjg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qjnfqycs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2igogalzp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2gtvkpqwe.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbkvvqvh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpqvodty.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uffkjbhp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2aozsfeqb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2sxxmnqlj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zjnbeeyv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ruampajo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhdvfzpn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dvaxlkuq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yjjzzuhk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yosafbel.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2brvbznkf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ttonrmmf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rrfnnzjf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zcjiedtj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2shlzfcuy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2snfzrcpe.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2gphjexir.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2nfcpymki.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zfwbpfkb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2fojczxtu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ixnywqls.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2eguvmquc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vfrwyodt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2suyryshd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2zjelxxmo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2roopvkxn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2zvfxxhgw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2jkkkvwkt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hsjpotpx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kgmqnzui.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cyfkzvfz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cnbcgsne.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zpbdxdrq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2udrdarmt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2oggvcpwd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hzpcixdj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nndqtouf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ldpdqrov.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2wspgntru.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hczavlym.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2htzbxtiu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2neuqulja.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2sqmcbolp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kcurvgsb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2kjkbfxkh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmgsubtf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hrqxohum.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xkwrqxdb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2klqyexos.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rrlemltf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2expkjorb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjmzxmyw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2igzveqsu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nqxvclmf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2biifjduf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ekpjjsyw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xxtumhnd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iqdplekj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rmzretrd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tqisajza.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iislxgas.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qhjsuvii.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2czaeqgqp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kynkcjht.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ubzycnlh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rfiikfdh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gypuvsjd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xevbaojc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uvoktgyc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ebekzmxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahtufkjp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2hotguxqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjypkpjq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fdtjylkx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rvcbgdsf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rgycelza.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2uttutvas.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2evogprss.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hydvkiok.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pmxguvxr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2dlcmovzq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2gkpvtwxo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ugwnrbjj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2stospwpp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xdvrchrg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ybybwscd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vssgjahv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xncauifw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zgcjndal.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qvmxniqd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hrbpupxz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yqeutjor.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxxliewg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lneajzcm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2yaiwmamm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yxqjfhcu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nfbgkrsm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2nqnqqxcd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2rmwxxplc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2auuqlpky.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fdoboobs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2btuzkwsp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2pupkwbyp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rwqfxqno.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngzqcsqn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zvsqwura.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2lhmrwmwq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ifnhzbiz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2rusmedga.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2yzhwkvip.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2piutjpau.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2azyhhscp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zklmdovw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pqjwrfyg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ymjrmgla.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ssqanaxi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ugrgqnvs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2nebjiler.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gwhhfbaa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2kjwglsfd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2pyhfneth.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2strzjxuk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dupxerma.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2knqypkhk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2slyfykwd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lpqpzckf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2orzkkoyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjyvcazo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ccvxwvri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljqbrhbf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vubtwhdw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2olkeocxw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2erwfudsm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rtvaftvb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eirsjtrq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dfaxfsoq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2yavfppvp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fosjavpj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wjvyzttx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qvmlhnvm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2rwscetnb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2fquwdtyi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ejyyklsr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2fyvnwbfl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gcnomsgi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qxdcqpxm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vxevruxc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2pbnpaiuh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2opekboht.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xcshwkau.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2jxcwayfq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zywxwahy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bbxvahrb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2hsuuscmn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2aptmtnbv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wniwqlfp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2kxcyyykt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2suwdkcuq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2tuyqqckh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cmuylvtu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tugciohy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sewmtatm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ptimewlh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2vsiaqsst.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rnnfrtax.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bnymyeux.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2bupksnep.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2gmyfvzuu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2tfshbmus.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2tanvemvi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bczdysqz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2pnqvyomi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bbelhaje.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2wqovddiw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xioaztxb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2pyzdizyv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ronhebvh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uebttnpt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bkvvqphv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpplkvrh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nevgmtrp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ngdkrrgi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dqdsdukh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ghsuwjbt.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2tgohuxqw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mkbpzhiy.html


<!-- 参考信息 -->