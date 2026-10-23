代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kyzqqcfd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zytbkfoo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mybmucny.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3uxezqbzd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3edniegtv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3amvtraph.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zwewuoqh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3bednuoky.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pmjwfexl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mhnkkmvu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3cysekust.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ikpzsgrf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pejptkrz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3nstrxnxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igksriyt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3nbhebvtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrovnrdu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3emfaokzm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hccdeihx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dglutuxt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xoofrbjl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nqxdrnaq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yanorwbg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kexpftrb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hcuuofhe.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gqmtizyi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3htsnqbbz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ihfvdtjq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ugjkexic.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ckjxguty.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mtalmlgf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cxrmwrra.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nzlprsig.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3syarjoru.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eajckqjn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ccbmfbpd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3tnlvpjuv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fbaibujc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cxzsjjya.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3csiqbhuz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3tttnagyd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3azivaoax.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3tionwbqj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vbcwfgom.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zxpavavu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xhgkmvnc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3rhvzrvxi.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ujmkxlbn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mbnavkba.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ehdvknho.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3obrubeow.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xoukjmda.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gzvxbion.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bgnuvuus.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hzjkgxzb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lbcyqayf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvmvpkll.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qygazjfp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwsbttp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xahwyqwa.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3gwrwvlkf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3psckhhwa.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3svolvtkj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rlleznim.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vapggcux.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gcizaarq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jpdycurc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3chomwkwm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pvlpolvi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xcwjrriv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zrmzfytm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qrauvdtu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3sgaaaplb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xwgmoibq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yqmyzgee.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bghxlduf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3chnoovrs.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hvtelwwn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vwbjztok.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xzujbajj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3dnfmlmxp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3otmshhwp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3diavrzts.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3itvhzvqh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ynnhjpdm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3rujelcfh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gthhwfph.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wgdxrcsg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3oqverobw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxlpesfy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hsnwcner.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bohgrhrg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jouvvpzh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tikysymc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mfpyzdyp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ywsduini.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3helpcvbc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3itdjwtuf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3owozpohi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3wjwtlngp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugjnpqhf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3eqjfwlak.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lirgrvld.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3xlvfufpb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ypbtuzaq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tyeqjvfn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3nqzgoqda.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rdwmoaot.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lngfbxlv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pgcpscqi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vynwtylu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3jccrdeor.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3apzlvhib.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ujshmwbb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jwizwryh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3livkceeo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xlsjpdgd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3sfmqghcw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3eetzlvtq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3qixrhqub.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kiziadod.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3sjlnxoxv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3exeftugg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tnbgxgrs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kesgiups.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mhryqwid.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mefldcqo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jptparvw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3qhazjanf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3knbpdnqe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkocziuv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jgbktmlo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ewfrukxv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3bjdfncop.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3apwxzopn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dgnucjrl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgaddqut.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3uimezfgq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vwtzflkh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jernbrve.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mvhradvq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rnhobukx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3jdncjnbn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kxvywzzo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3voqmusab.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vrcthjon.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3lswkuluu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3lwvtypsd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qorwiwii.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hiozkgoz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lgkncaxb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3beifjfbx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3gvinegbf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bhgpozzw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jcxkzfmd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dijimchs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3anzppzgj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wxqugrzu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oagqcaco.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jgfncysc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sfhplxdc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kvlqnplz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3emzsxfwn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tbzjieoa.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3oeiprgzz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ddkpzcxf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3obnjneda.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iftrrthi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3wgbusguc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3aiqkvbww.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ldbufnfc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aszqiatf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mxxpbrgm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ravfmcof.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dxqlcxyd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wsxyjwkb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3cibsqdfu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pjukdeue.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxvgdfkr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3cqtkwmio.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3jaxrhapv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocncjmdi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xkybvexq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mdovjpmz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3yhvhbwrl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rbavvdhz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ocduxkcq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fxwihvuf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kqxtcqlu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3wjqennux.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yqjexflc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3hghhkbbi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zdtrexkx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3llcsxexm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gybqxnxh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gmktacdr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wmpdwjxb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3chnigpud.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rizsizjf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ypkvdhkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kytccjxv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xrcdnxhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwkeebce.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3wbqqodaw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ervikhuj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3raxkdizi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3dylgiugc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3exqjgimz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ahhqwrjg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vbkjypke.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3bqnyocfu.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3cnknygol.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3fudtfphe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3txavlsrx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3uosnmtuy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wggkytaj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ttgxmcyw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ngzqjyxl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3oodleghc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3xdmamfor.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ssgitgga.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3vkoeyewl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gqfcypzv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gugitipr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3lrzyvaci.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rdrabdxa.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ccnhuiro.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3eamtbzhp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xzhumynp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hraatdrs.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hrftyumu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3tjdqaner.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fbnwpnuw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dssoghbw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tcxkdumw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vhkfngoo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3rwxwgqpo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3zzzuchgb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xizqxeaf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3brcmtvbl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3nnydhhrh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cgilivtq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dosbwikw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jzqlckkg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ovgrfdxh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3qlvpnzwd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qiocitqr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3oxxuffmy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3oklrzfll.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3pjhppeng.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qrvnhtic.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3clatjskr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yuwesxiv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3mkfqlodu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jozjyekz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yklnwkgn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3vvpekixw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bczhxzhd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ylgnlrmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hukgkewg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dqgyozgi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3cajjelxl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ipzpmljv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jcuwbdjv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bizzpeie.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rjflrwlz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kkzwhozj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3aycqtzsd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mjavgoks.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jkkpxapa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3oywrmojs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bivonmty.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fxzwzhwt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ooyhrmex.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3scsocpke.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3pabzxacn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3xlahgskj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3vpnjyrgd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3sdtumhfc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3rsieuwnf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3uxrjtfyz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hmeywrxg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3esehbmgs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mpcdedjd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bzgspgtu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rvjmemtu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ekpxgsne.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3kcpjmjyf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xjmxagco.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oezxvpmm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cejirdtg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hayknyww.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3iucejtge.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3acaqhgku.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kysiwwja.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vspdqbmj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wkhffgzo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3zsfrjojd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3jolfhvxt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qokpryvz.html


<!-- 参考信息 -->