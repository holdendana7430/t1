代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xkskjtsf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kqbaccjf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mcuwhaff.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pauffssr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yyzevhls.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2feeywebe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkdaotkz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xxlbrlei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aezqvudt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2irkqzlmd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2whmlustw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ksalpizw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsmmdfsw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zcialkom.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dloegncj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fsozulbc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qxkutgwv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2milhyjgm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ykxrfddu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qzrpkykq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2krnfflqp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2psjkacva.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cxlblddo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ofhoxgma.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nibjwyue.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2fwfawcrw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qhvdxelm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hhlclatq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2xghzrvxd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2uvvgkefa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uphzfkto.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mtixjrmq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2unxcxkue.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hpvpmadq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vxtomepe.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2azzyfiuo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rittrpvv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ncurlqey.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tjnjvlzk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vcxveyvv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tpowiubt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2gfhxtwsa.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yrniigzz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2fcfinjbe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mxxvveno.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ciijrdil.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ceajrrge.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qdknztbx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2meonhdgo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdgshpzv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wnactyau.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2seacivrb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dyssfkoe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wuqhygpi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bejfxfrv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ykuufppd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wzdixozr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qjaspuyx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kmbrpyoy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tkzdglzl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gjzvzlys.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2esrqtrht.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qsmiwyfx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wobaaiju.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2mrxizams.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2njlhljge.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jqxparlj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gtntojld.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qfzddmkf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2sbpmjatj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fnsxyovn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2suewhipb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ujlreyjo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2unsqihoo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2vglrkxhf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2loebijns.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2alqzfzpd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pasyvwfk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qkkqlcgc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2yvmehfxg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2krkuvhno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojuorjym.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2wynvossz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsdykscd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cmyacqhm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rnpjkcxc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2clxetllx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hpnimrwq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tdfcltfo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gsmhewxi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckajukvu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fptswvvx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqooglre.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2kigelcuy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vnfonrmu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vipumgqf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2badiezbf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ylhdmhax.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2pagsoert.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ubnzhqlm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wexdgscb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hmpenvuv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2cizcsyki.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2eqblhmjj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bzcphonb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bvpujebw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pcuscqab.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ppmdncux.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tqdsjupw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2kmjxrxnf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wilpcqxj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2lafuumcm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2leumybks.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bjykhnup.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gfsrsbhy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2odbzprgq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gsfqfisv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2yytcmnmz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2belfhtyr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2egkljhgs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ztfnrane.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hktodkau.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2afrgieec.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcbzefjg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fophdthm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2djqyqsoo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2eloxrawv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hvbfjfjw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnlplgns.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fcsjflfx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hpvybzkd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2slhvrxqx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dwumrrmj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uhyrymmv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ajnztkyx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2bzkbqkij.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rwgeevee.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xzoimdsd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fbpwlzwe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2fjoybrtg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ocbofzrc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jpqoacmx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2gpxnblrb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2kocijznq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2wlybabvg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2mvayaqdd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2wimqzmkn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2tmqgruze.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2idlayfom.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wemhzpir.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2efvhzyhs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uvqbgcab.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qrfrvcbo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bthmjlkw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2snvnxrwk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2thhgftpj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yqyilvjl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wojlfvze.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mgepcvyu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2agzvkrzs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ehovbnkz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ttvkyihp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2yqxnlswr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fibnfbup.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2bmaqajuk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ujeloybb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2khqavqfb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjvrtety.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ukcluhou.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2prmorziu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbqgvefe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2yrnxgxlv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2kazousgw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkhzkvxx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2dckabpox.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2pvyvrphk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2uqiduqeo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rhbcdnob.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dxqbqtrj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bvgngzlg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zpeohqse.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2iqczubqw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fiuenjqc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2lpnhcsgu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2maplrzcr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2dbnnxnzf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jacxujzb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wkwjzawg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bykymzlj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2criafftx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qwzribjz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2spuqhzgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlrwusdd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wofoigfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwuoruyu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2cvwasxxq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2tcmrchrt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2lqaovyst.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2vtzqwefk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2heqcxrcf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2scbqdfuf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pbeiuzxl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ztdsoynq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tollpzxh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sbcxiyef.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rbpwcmhp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hybkdogk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2votwzqcc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hpjoxsfy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qdozitdy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2thgknxco.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xlbmnejj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2lgnpcguo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2clniasgk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2fcvhybfl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2mrzgjejt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2apfoqywj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kwzwwtrg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfqsdmio.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bwtykbtu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wmncsdlp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nopjwrsg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cinhxpbn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ctomvhws.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2aslrqdfv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bqhjdjbe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2udyyfpnv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bbrzdely.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zfbcfhjh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2tzigrkdi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jofsfbkb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2azheloht.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2hbsdlvsc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qezfnsno.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2arsqhevo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yscxgdop.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2gaxmbhju.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2dbgchtou.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jnmuyujx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwuuqxwo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2yrieecsw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qjrvqheq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ptbpaddy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dcnybkkj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2crzswwrs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qdegyipz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2waizuhzj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ncskjegr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wzlsquhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itdokdzz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwnfhjxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgwsfcjv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2eebemirw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2hfnrhamu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jkypcyfq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pcplnctu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dwiejorm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pagjghvo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ysgzbcex.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qiofurby.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2itemwlvk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mnmowgmb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uvhfrhpb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uzfpfacz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nmckhvdl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2eznahxfx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2erihgiid.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ohtqjkpt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tgzjcxjl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2cewiqdzu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qtkzhjnp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xllfhamj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2txfaiyyh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cowgcqof.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xieupwoj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ujvzzxdf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2fdpmqylt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dfmalafa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2xotneipt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2jfvtjvle.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2vmannekv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uigiyrtb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rfdiqulz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jacwnels.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rroosgzz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2szctzjiv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cqpxoiho.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qnxifesy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xynqoags.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2nnlhvrzl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2gtthkswg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2sjmolqwz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2sezuouqq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bvlvwyei.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gdrnnzfw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2rbrkcxau.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zvwkcvcf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2vvicupgk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ptlbkmax.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwrbeqij.html


<!-- 参考信息 -->