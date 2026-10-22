代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xstzehjb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vhghqqxo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dbbwkoto.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2whiltphm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2iqrijjhy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jiyfgcfy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wmuzbkav.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fwnwdhzd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kpvqtovn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nhaywovt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ezfpwysc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2sikreilj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bklwrwzr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ovlmolno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snzqyvtn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rnparpso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndaxbyqq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2owanixjx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dfampzny.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2xyuakjcj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qxblgiwa.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qkxefavc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hilxvvav.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2yqrnihtl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fvryiele.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kpnstmsy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ongpbyof.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ronwljde.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lqwnkniq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sycntanf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tsmurknm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bsuudtxw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ilwoobhg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2oxcfphfg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vqpgqtnq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2rnkfskor.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zyklhznj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2mxqpadjw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hmppgyre.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qmxducqw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cmfvkcbl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2lppdyrqf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fpskiecb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ommwolau.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2phsyiufr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2prgdaseq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2louxpewb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pbcwzaqo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wxejhswq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2byshqrxo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kfyqmlkd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2sbshdbwh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vdjmhxzn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2yhiqhppx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pnnyvwxf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2bjyrqdnp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2knplgqtt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjkxwhbj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ifxfkcml.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2whnfcxnk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fkmiwkov.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2latvwwnt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2kscdrjjz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bqvjijtf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ffbshitg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2utirjosm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ltcgdsfy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mkfzylji.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2tjjohmyk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rxtyurlf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2halufzqy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qcsdqzex.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2dskqwaca.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qgrvaibr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2imzzafnd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2oeteskel.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hcqilskk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2mxqpuclg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bweubnqr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cozxpekc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rbhabuqi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ycikmbkc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2llbytjbi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zzrppihk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vhaqqvoz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2lsztcrxv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2afcxpmyt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2syxjedhr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qujrknbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzedurcf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lzfgvqgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwsubrzi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hadjhinr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2epknaegx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mzcjobhi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jovpqiky.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2udlhcoyp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tumxuavl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2meqgghke.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cgmzykra.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdhrtler.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vuiwtwnn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pddzlawj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fdodinrt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ckyidexh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tyirsmty.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qfquxipd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yrymebsr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wsmvxylk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fodbxokz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2muvdiloc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jtpzawkj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rhnxccif.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pqvjkhqp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ssthbfuo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ajqetmjq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jfqrkude.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dwrilalg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hyfnzmax.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2oparhtcv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lrfhzbyk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eprvufqj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rfkqiywk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hmvmmlrg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yjqhvfvx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2itkivopg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2npivqtpi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cignaqsd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2pzjjjymq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mttjicsn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgqnbgse.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2htedjage.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ftcjbymu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ypepfbpm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qlswrqgw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mpvcbffv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2kdkwvubi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2lxjggiun.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2itusxekx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gamogirg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cmdnywvu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fertalrg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2zbnedzxn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2erltngcn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wljqxncy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2llllskfr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jayowhei.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2adoafejq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pwfqhfdz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wjftbkof.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2shqxuhlr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rylimkpa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qxcbssfl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2imovnxov.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2pcfnktpb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2dwfiqmsn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fvxwkpzo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2kcgpdifh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sywvljcv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2urqdiqsb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qawmdjpm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dnadohgd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2keduebfq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2teddtfwk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2czbrwbob.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2cggodsql.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xkfvvouc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uiigmlyl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2xgijqsvg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2snysigvb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2smenlehq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hxqawafv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kizpptxu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2fsnxdbnt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2dzouhimr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2tfueusbs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2espflsyt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mgsbzuvu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2fdxdwzzn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2nntyzpci.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2aixyvdvx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajzejprf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qhmlqigz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ofelflnt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ppoklavc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2csljrjti.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2trrnvuxm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lzfgqruh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qujpbsbw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xxmhbxvk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fxrzgbbw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2tefquviq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xtvxrcvq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bvvobngl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bogzokwp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hikvqliy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2galiqlpp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ynzvvqui.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tigshqef.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ympxlqxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzwxshzd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2patibmdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nmjckhaa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2akwqmigj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vuoqukdp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2sqfnvsvw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2gqsvgmui.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2uoeifydv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ecjdmdlu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2sgpbuudo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ajiniune.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ovwssxwy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nqposhiz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gbcmxsvh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2myngyuue.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ypikrbpy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2deunjnpb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2nxrkyboy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2tgqwmpcg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2juzflcmp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2pavareed.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mklcojiu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2uhlvaoim.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2uhohwhoo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2joyfjxsi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2thedzrcv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cnbooanx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qpewjdut.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2eepvklwz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsgpttuw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2vhyiwdcn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tkijjpff.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tfxoavyw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ttnmnpup.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bmepticf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ahcpukvw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rnrzobua.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ojstjmei.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdfxrrxk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2wcpgqvdp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2faebislq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2yubaxxuq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tztyjihk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ienfpdgt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2bjqhnszw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2lxkdubfj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xnzfntso.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2rbtvhprl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2oufbiffq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2oerohryq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2fuqecvth.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rjowmyuc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bsgbxegw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wbzsrhyt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2kzrtjktx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xblbhpzz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jexvfzwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcfhrtpg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2eavrcose.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jopmkbau.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2eaghoaxd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2fldltevd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dvpolcvx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ocjsmxpp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2evgbbwip.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2azwlsmzj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2hsavuqth.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2igwaywob.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vidmoike.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2umbayvjt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2nvvzhnwe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sjoxozas.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2olfauuep.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2tqgreddp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2redtlxrv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2vkoqbqxb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cyquurlj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2hyqpdupf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fdfhjkrz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rvavwzou.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fvauqlbx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mgucbmnl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bpdfyxhm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vsnhvyot.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2svdojgka.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zlxgzuqz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wjeickmi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2tlhevgdj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2pyaycfgb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wetrllaj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gybjfajg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2binclrdk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ecjmtpea.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2rpckrere.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2gphvpris.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wdaohypq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2wlfghyhi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2spaajmcn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jpkwzvbv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2iuksfddp.html


<!-- 参考信息 -->