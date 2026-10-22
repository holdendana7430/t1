代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fgoqvvzy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ppdccdpv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2jyrxqlku.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2twrpsigc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lvwgiobo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2endiskkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnoxigiy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2dgabfupc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqvztrir.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lhhgahsx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hyvdtqsg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ydbdylux.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wgbutjka.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yxdagwnc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2oclnddya.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2efafdetj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wyaqyxdm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mgkkutuy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bgbxsndh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2czbjwycm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rvllqvax.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ziojvqhx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jjmzinrf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2atfbfqhb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aciyawfr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ngstxrol.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ykwiossc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qqcsvogy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wnwcfklc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2zyvisipi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2egaodwzw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qdqpxevw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2sxsgflnj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2mhdzmclv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fhcujgjh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2yohpvvsu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2uznsuwmj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2edcsnyya.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2syezlmux.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vqjxwzeu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2twtfbdth.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2icmsbrhx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jiffnafp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ewewskfi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jbghuunh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mwsrutnq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsdwkimp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2khwmdeop.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpiulcqe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jjxyvdii.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcjgfhxr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yjsroqpe.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dkhflzmz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2geejncjl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2tdrbrxdo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pbeeikeu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rdlaozzk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ohvsjikk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xsdrwsbb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rvpmitzm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2syergwnb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2evqhqmgu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pmlnxuqr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ydvklvbp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2otaewxwe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2phnlkqqq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zpmrzvev.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nhygzzkd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vesjknad.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ehdyzddq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2wcesyeod.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kxideree.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2plarvmip.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qnckqtha.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2yevdogtx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2moralmks.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lwadmmkq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2rpcbpwnt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2gnroilym.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gghqbiud.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2anaarmgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fugvekxb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fmkhupcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbhozmnj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zstngtta.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uchwlrbw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pejtgpzh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uwpmgqit.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ngzeisui.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpkgourx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rdbwenua.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2koicasqs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iucwojdn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mpprcapg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ibgcqbwr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nzvaamyu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2axdtslfp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2exglhctg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bfkgcggw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lywruhrb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2eqbohdvh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2cfzovecu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2snzkghdz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2euszgvfm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qcapsfab.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dvjkmjvw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rgzfyblw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mozvpdek.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2sbldzuvg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2cmqqwfdl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2tvrkskgo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2sovuokti.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hfhcomlu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2keioadje.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cseyavwg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rylwfjwk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ktullqsn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ujsdoaos.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xyozeazc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wcpvebke.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2biuawxuh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wtedzjtm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ihfuzmsh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2iclcaayi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvporanu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2yotnedas.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2euninjac.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vecgxpnq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkwllbqd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dizaevsb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cnautaxz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mxxnoljh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aihwetcq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kahbvrmd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2uthplvvk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2tfwbmfao.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uohsehzm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fznfqjyj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2tvvsorsv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dctxoytp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2yhtgyfeg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mflnvbcd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2acqogptd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jodfcjtl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2niowhhie.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2mhictdsk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2kirvrynr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ajlxyjpe.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2qpaktbdo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2isloljqh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jbivyygn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ptfzgpeg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rilqgmjl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fnbviold.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kxffbdip.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mbetpqem.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qzgmumnk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2iipuwxac.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xghqmnfq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vglwnjoi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2rbbhbimv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tdzjojzl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2orpcmdgy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jvgnhpln.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vqwipycl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2efndbicn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2itzgkzpe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vktcflbo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2agcgigos.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2cnsylkip.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2scwqgqkg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mzyijzpt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2jozuwskt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nhevmeon.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2juzwhwjg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2dfmphkde.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2hbriefeu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qrgsykob.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2skbdcuuo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dudddncq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2aicfoshy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vdmbeacd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nijlglla.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kuyugwnq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fzqhjafd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xyczwfll.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ycyzmfzp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2taacqkpv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fybbqaxj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ntstxygf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ctkmmqyp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fefupqse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nndlrluo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2rusywfdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvpyvhrx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ohlbbjas.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uiwpiejf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mmzthvrg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ukfaxkjh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mylmjerf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2iceubhay.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2aidvmteq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2deyghsaw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2collbzks.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xmgfghvi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2apipknvi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ajigfbpj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xavaeqqx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wptokhhu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jvngfpht.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2uobuxcxe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tuvrtusi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ohpxexyf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lclloqxg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bjhqypuv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fnucbxsk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wqaocxcl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2onvtomfn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikghzdwb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bulymndm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2skuaysjm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfwzpkaw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2chdrnnbq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ffobwmkx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2lppudpyu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xahkhnsw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ksxxjqet.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2siydowbu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rvadtwdn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2znsfihms.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ekanldub.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ffbphajt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzamxqo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2lpddpfkd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fenrrxwf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2atxlzinn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ewggsvnw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ayepixoz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fdbutzrw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2dekwphzd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qsgrpfqn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ridfcbwu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2krnurdyx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2meytnfaf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ugdhhzix.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qqpbiywq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bddmnpgs.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2eouushhu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2bgbyydwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omdtufos.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2vbtehxfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxdfvdar.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bhbqeqbk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2exfvncxe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gwyxcedk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pdegngpb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wkhdmpza.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2yjuocbeb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2iixostay.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2oofjsgvg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dmxvfgqp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bzodzkvm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2dmvokvtv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kttanbmo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2bislxwcr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2fhkfvjfd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qmhtwxvs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mlgfctrr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wdhfgaye.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tdmihbff.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ylksctuf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2nupthvlx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qcwecjma.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ffufkcbz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vwjfexrp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ejdnosjx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2yyxkxjdu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2jxlrvgon.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2kiktkkxm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qzksbbyc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ycqoffnu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zimnecmi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zevehmhg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hoxhkken.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ondwqwcr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2twcabpfh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ikfyubgo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cvuvtyln.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2bciwdnqc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zuklcxbk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2dawfoche.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mdymiziy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iqsrahqq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2joanpvsa.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gszpcegt.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ifzfoywu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2akjfribr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ndetahmi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jyzyabtk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2kzrtfwnk.html


<!-- 参考信息 -->