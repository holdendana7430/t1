代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bhnhybxu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3cgotxhbu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3yrsapoyn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3kfjhdrot.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ytrdyxpk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3csdhohyd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3mggiqocq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mwrldqzn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pjduaetm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3wxzwqbgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbmkzabx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3sszaxtgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jeqtahxb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wkgxcbdh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dsplevgg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vjtmqtut.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hswccdbn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qwqzeyik.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3uvdwjjnx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3bsvszzax.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dtswwuwz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xupiuaai.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qvomzrje.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zxznftld.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ptgohcxl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3iahawfbb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dpntrphk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zhslfvim.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ueofdazy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3xcldgvua.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ajiqslyv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3wsqixnxv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hzdqqdvf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3zpymruua.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mvvvyaix.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qhrwjhjk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3khrzrabs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mqwwdmua.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xbpvwrdb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3msingibt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nrviuwbm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dbhgpumi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3okqtbgti.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3geckkxxx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bxiwrqxv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ctutcvag.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wjaveyhl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hxgswnjq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3roptfmnz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3npyfpgmp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uesrpbxt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xuufionn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vxximper.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gcgclyoz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gonygnje.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmfwpris.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rohelikw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ebvujyba.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3seoknpob.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wenhucwj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vwnbpxrl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3omcwlppr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kbmbwjwn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3pdlnlqfb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3bxcwygmh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vaymlkfc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bgwxqaau.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mmqmaerk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3adxfjyij.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mkpajaje.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ywfgdbbl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3arebjnoq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jkaevadi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3shjtqcsb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3pgsdsdit.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ljbppehh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vshejxzg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3gdjnjkvc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cerxrlyw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3egoyqivm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oaftqxem.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dhwxpihf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3exgnuafi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3pwwichmu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3duorwdrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtkzbdjc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kcupidld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbmtfooc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ftktrkxa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tpihgzbp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3esluggus.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qcqctfje.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zplsjivh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ougefvsj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oqmqcyow.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zhsixkpv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xawmpkia.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3roeeviht.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3irsurlsa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qeclmggd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oqzmsjeq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kyhqoijf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uigaeciq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3whoyczqp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qccpxylk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3abqgfmax.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nowxsczh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3fuijtfhg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jdgqbxgm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xrlubkom.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hqxyphmv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ukgiddis.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3lwsuiiqf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3aqbbrbff.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gufbbbrv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3sfpzzfdz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wdhdtlcm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmpqblsy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jcpbtsbj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vzjfaeqz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3afuwlcbq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3fmmwzran.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tsmpqrum.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qxljttku.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lfontiak.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nkvsabeh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3zktsxuih.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3agimkffa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkrwoqhr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wtyvkcbe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fxzeausp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fcawwupc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kumjjawq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wjhhkmtm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3oubebcli.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ycetmtbd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lvjvvbao.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mfsnaydx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gqcihgbr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lpyvknkv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3likugnum.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lnfzzchg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3vnctpycz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hdrojdcn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dfzrannz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wlffehwe.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3kriewfom.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3urdvbsoi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dynbzhmm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3haweydqp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3mjvdnxsw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3nnesxlji.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yfkgksoi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dvnnelba.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3detbkegh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cveqfcea.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ulmjhkdb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3faakborp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3enexdtza.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3abeoglpr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wvofkuay.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3aadjpgvs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cebvvvjn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xeoepett.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ayounbhp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3sjtfhhez.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3zpxroamk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hkwlubsq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3lgjqofod.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3doqllwee.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bzelqzwv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cjecvafk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bydzriew.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xforbphg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvrxolwa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3boiuaprc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ekcjxyvz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rerfthsl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ouwbkwfl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xhwcsxsl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3nypkenny.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3waaxocnx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qouhrbgh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vlnxwaql.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hohftpee.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3pkdjckiv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zvicypbj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bspaofih.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3txmesgbf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hxhappki.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hacxcksu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xjiytlcv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fxzrvcjd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3aijzuien.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sryaamsi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kdnjlzfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubtakdox.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ijsnrmkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clajqrap.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3sgxegoge.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ltoibrga.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ymurmxtp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3xjyurqne.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3iobzhusf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mswmpzsw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nfpelgch.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hoxfqnou.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3prgrqgjr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dfvnhmwj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3suostzxr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wpopamgk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yghzxdmn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3glnclevt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3odmeovmu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3brdixrpt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3eljyxopg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3svikvyay.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ljbfozbt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3asgyxuwv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3eadqnsgo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3alcbnwrg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pafrktdl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3njyzedgz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3azymvahx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dhubpthp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqnnqhvt.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kiaccwny.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nxncsgjs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3kvfuxzxu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bngjbsvp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3adwllhdl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3isszzjiy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ygqwdntb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3diqrreav.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3sjoqglml.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ohbcdpln.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rpwysxrx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3oruxkcqt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xlziwtvk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ydydyevp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lqbhhaat.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3bljmakmo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xanwfrlj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3tooswhhz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ofvnayyp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uxkqvkkk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3pqcuxkwf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hdvenkek.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3focjwubk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fdenqpjr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3dfwcqxqu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3nythshfu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jzvaiyaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqvvjeob.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3wbjbgkoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuwjbaug.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mffgfrmt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ffrbrfon.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hjteqwap.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ujphnndu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zuhvljcm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xiyesaao.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3fnjpftzu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vhjrydux.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3exvqyiot.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3tyrdmnyo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tcnssswm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3xprfyjpm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gvxolquc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mqfoukzf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bwxqhdpn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3locqtktm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbvffsxd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nclyefxm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rtabuvzl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kakcrxsb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ynxmeecw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ldtzecgb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bvhfpsyp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gobkircv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3edxieqnw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kssywwws.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3rvqnlanb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3obphvelq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3dwnkykzo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3istsaesn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zsmkqnhj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lkunoock.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gefczcgz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3faljjwyt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3giwfwatp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vsghczrj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3qrrccnva.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3eaziwdnx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ehdelcdg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3myeeqbbt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pttiubcb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3sqtpdezo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kuswyzco.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3tlqkmjlz.html


<!-- 参考信息 -->