代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lrtxdefb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2okdjjnnk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2izzaxnxl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wmgudfyb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2sisyvavz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vdinyyip.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2nfwnduiz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2gsdjbakn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eznfadro.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fdlmydjo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2djpimrzf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2vtuwhokh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pbyyzrcs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2umoxzosa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dshdngry.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2yqifzgkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azhjjavv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2owhhvxgy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lqharitv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wmvqdhyc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zttzpzmt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2amussjko.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ijujkflk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wjaulrjq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2veywgchj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yqygiazn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hlrsqlct.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kwjiujsf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2znythunc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xebkfkzd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zziprhcy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ebgcohhd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ovqhonwj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vousmxuj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2serrlrir.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qvupaety.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sftyxapr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ukkabgdk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2loqmofhg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gwcdovhs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2yutockyu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gazmxzod.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2savtybpw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rrsjlplt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ystfuypk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wwpbxvby.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2kmanlywe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xqwdtgun.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cfutqjst.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cmzoiyle.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mxzhgkka.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lhseelzn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tqloldss.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qlodmflr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2afgkxsvd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2eiopvpjy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gtwryaoj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ftlcvkrw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnfdyizq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lnrqsrhf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gcddyfda.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2aidjdxdt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ctwavmcz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qpslfozy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2uzpyedxc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mcsrpyjy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hsecxjvm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xfugjnyc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2lffqeche.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bemasysy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bzqxlqbg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2twdeyexk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ttcqnwdo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2guldlann.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2onllqomt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2prpuiksb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pytpycnl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2suhlqwiv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2yumtnmag.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zhetfhzw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2muvyuyan.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rvjxssdb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ihxvctnz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2unlinwmp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lbtnqvyd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2opjrksqg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tnklediz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2aypnsfgw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bynksycj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cujterwt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zfrrxrtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myititxp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gvgkhoel.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2esdufmab.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hkdhazzr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lczxbwhi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qycvndmz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2buuyoctj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhnfkpnk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dmmqmuue.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqifaakb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2bdsihrvg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wcuxemsk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yjvksrhh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xkgcfndt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2epdqnoga.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2nkrocwxg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2khjkhxdj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bzokwwix.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ykultekg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2becoyrul.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2nsnjpfwo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xlqboqhs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nacrexdf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fplayfrr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2uwvpdhll.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ocwfngfa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2alypkqij.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2abchehhe.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2lsoqeuhr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jagbpwdm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wrkafmcm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jsgwtwwg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vflrpqmh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jyyrairs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2yoclikzd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzefdkne.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fpdixzyc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2psbgnsew.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xbbvyycl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlxannzd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2spanrwyc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zejbjayc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2kdzpyvnz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2glmairir.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dbwqcald.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkbqhtie.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2eokthtjs.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2heoekvfu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2olgataum.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gbicmidf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sqrhmiap.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2zygpanpt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zqjirofk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cibrjahl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nttgjicw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rojkvrnd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vtbimhrz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2znivhdjo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2onvvhaec.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2efizpqgv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2sspfzxdo.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2jmrqiclg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2nicmoubz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qogqyjew.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2lzrxzwyp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2usnljiql.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ndwfbrsu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qnbicnwq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2akmjdbna.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hazgwqrt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jlpyiwbd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gsvewicv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ossclsqq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2htqetehe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ovnaavhm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pntdjbcw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2biyucjoo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2yynhmfms.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2igmaedcv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kfkmzbon.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zxxnasxk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kexiqldi.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2gwxzmrrs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2mgaxliaj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpfluzzb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2whfcwqst.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fwktzouq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2brmtsseq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2eeunrtyf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ofoykhlb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xwvhrawv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dfjxqtuj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2lgvggdsd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mrfhrdlk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hlegxkii.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wfdfysut.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gevryhtw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2svhhvfme.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ushsqbde.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yufcrnfz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hcbtlccr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ppmdofyj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2idwzmglz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lemgllxw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kapqyttl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nrmwmrxd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2icruramb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xrbhgejc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vrrghkkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rokyqosr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2sxdzmrim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngikizjl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ecafdqwx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vwkmgmap.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mwltmpyi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2puofjguc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2djeojube.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dhbbpxqq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2qlxgjtrh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2lwadeadn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2clusirrq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ifsacxwy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gkshbwhw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2seyltsat.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lwmfsoko.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nmjxqoqg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tghoowsd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mmceaicy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wwygonzr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rlrkocnn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fhqbdsrt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lwmbkdpp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hddbfeuc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rrztsyni.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cpqacxrq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ofxpymqz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gewnsgac.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2nhiumhgp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gmehgmdp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ohznxvwo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kzogixmy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2uuimjueo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zeqwjcqu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2znmlvthv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ksrmfzhr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2enkrtqyq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2hdmncwzs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2iqzfgccn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2yznjfmqg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rpfpxskc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2hnamygin.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2thlctgci.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mmjceciv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mmuwmhvf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2runcznxh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2oxoifyvx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dezqumsy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hfvmjcly.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2bcqpqywi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2kolozkyl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2njcmaaog.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rzxeutfj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kfzwnnnf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2bdctkksb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ofdyxgyp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2aguioazm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbbgergp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2iotbtaqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlfhyqul.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ablndspt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2tdehbwfq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2yynuovgg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nngzphfk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wpnpyanf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2smrwidrm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zcddptnc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fphcivjj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vksvuvnx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bsjtegca.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qxfnhuxp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lopvkvjo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xngrozkx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2msjidpns.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zvxnypuk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2tukcyfca.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2cwkppyol.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2yfbmnhyu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zedgwsyt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2aosjsoqf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ayuiawss.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sqavckif.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2iqwkrnqj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2wudsyvci.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2dxxkfthq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mgbcteon.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2njoayqpf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2fgawcxkj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2dvwbievs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2krtfnkgo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mkvsqgqi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wscyjahy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zvczeoxv.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2hqxdllkr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ayhwfmpb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rtydkotd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2xhncodxr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2orqfushx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2mkuggrlq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2gbyjytlr.html


<!-- 参考信息 -->