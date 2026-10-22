代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ffxaowcs.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ouxsclbq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rxdorxfb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2xsrxqpsf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dmrbokgj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2duclqrnf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2rdelshuw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2fxyzjepz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2irqkjrxy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2zqodimeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsnrgpfl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ynsyispg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktneuwgs.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nmkfsbhb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2efpogfzh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vvyrdefh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2shgcrafl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ziwjkmff.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rtrstgjj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sidyzlqi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vognnmct.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bhzeewuc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ycypakaj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yblwhstu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qmoaiihh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qmiezzmi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rqolfagw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mdesygaj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rqlrwlyc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zrlpramp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cnlavogq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2brszgwyy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2evbjzzkw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gafuapiy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2aafttgai.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uaciddva.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2echvuqfx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ovhbsigw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rdwuahmx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ndqlhfrx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fxtrolnk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dzgvywbh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fsbulnpi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gdgxgejw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mwnmranh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2bwvcilcv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2fvuepeph.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2pgeupiyz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xmmjliba.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2yhfsohst.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwjpkfww.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2leupchov.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nlriueim.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpuynlts.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqqolfag.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2laiyslrh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2waywptxx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ltbmdjkv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2scpyjgrv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rzxhbjkl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gxehbozd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lsvgituh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rcfmchke.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ahoqpypb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2roashiat.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rieaydoq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mhogwrrh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2bwxqhjuu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ydfcdybn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2rflyrbex.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uojhrnjy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hlrkrjhv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dcwdlesu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2rvybcbto.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jclvqost.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2aiyqeawj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xdxbxjyo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ztetzmks.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2axxnihfx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2eebwgsgh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gguedwrm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2siqbuvii.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ozulreus.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tpuxzaei.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vpaprgvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gunpnnld.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2uxxvdidy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnxonoqw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qiokerhk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pvevxrqq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wctlvfbc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rutrxjku.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2byelvlug.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jwenvwwa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lxoetvop.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ypscgllu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pteslvrh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pecedhop.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ldquobvz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lwdpehxj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bcktamab.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cgbfdeez.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2adzgucua.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qjjutxbl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hqdbnygp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uzyelsxe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2piwpanrg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vsjluqln.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2eedavvla.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oercrhgs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2irnnxvdw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2cnneqnnb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2fvduwpks.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ocyfynyh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hctqreyl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2lyuujpvg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vokiiwbn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2svzmfbgi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tavzulga.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2oatozbfb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2henrxueh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2eypiljua.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kehafqwf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aztltnup.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qrnelxrx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2boolkfvk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddevwlad.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjipfcyt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mmirvkyh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wcefyjmt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2oagyoxij.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wxozlcwn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2maueqdns.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dojmmhjy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wheajkaj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2akyylotw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yzoeivpz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nwqccxsn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2zhqfrehv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tksmtnfc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bwqgbayw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2awpsxyxx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xjfjhssc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qmqochvw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ukqqzotx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2slbledct.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cirlhqdk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gyvdjgyj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ulcsqljr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2daqocsss.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2sntdlnhh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jcatuivz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2yhldviry.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ygrtaazt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ybdlzvxd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sffqetfb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mhbssszv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eriaalte.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vwphiqiv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ubkodvpm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2otkfqwue.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ippmjytx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yfhczkpd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lhwxvxxv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hyyoawih.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vjwjsvof.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pwolckrd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hvvsafnc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xuafduhu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jpgrpgnz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wvnjjpiy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuowjerl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eissoqtm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dqvjdeyg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqitlmzo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ivjmynqv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2czpvxgnv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzftozjm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2iujpcgrw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kaqojdws.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wvoialbj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2genxrlwr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cseifgim.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pnvzvxsq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uvsyuptg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2wubcssyv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tabxvlez.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jaslqihc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2poqpqmvo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2lcmnoktt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2omxgcpaz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pelljsxq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2swsnxrjh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2uctlickr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zmdgktht.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jbaxmcqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbkqlxra.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2aiauplrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kcdpanzc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ukzqfhly.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lpfsoefv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2cnepubmn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2gaoorply.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xeozpiix.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2mlcxkpqc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2riaicmyj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ozrijiyv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rylhigmo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eyfraxxq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ooqcrfeg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2oizifhxf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oojmpghd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qnglzdbt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sydakpii.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2stidulcr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2igdasugh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2zowpqktr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2zrrtvlul.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gxbeuzag.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qevohcqn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2bbpbzqni.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ysutrnxi.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpovjptc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cimjudmy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vqdarrxi.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nyffnkzn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xxcefeui.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2amcqzxdk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2unhrazoe.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2binourdy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2woodmukt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2uacyngiy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2atukhbns.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2tilrdfsh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqhmsmtj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2bandilin.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2axlhnhfa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2kgldxjdx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jaqpvezw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2iaavacdi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2zfitfybb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jukrfxov.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cemgihhw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2tlessgdn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2aadxxpzk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2eaocjtky.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2nyuyyjus.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nvjtxxvq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pxopfvta.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jxplzsuo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2avbeoyfi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ritdpegb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ydrcansq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcbijonf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qfigdslj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldqkmthn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nnpfmkvp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nsorxixe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bklwxinl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ryrhsrbx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bvdehbdh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2scdltfgo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ptpgztnq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fdxxtqbp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vggmuttu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fogmvvih.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wjnzjnbd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kfarzjvg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2clpcdzwp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2hjbegcrp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hslexpup.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ebuqrgzr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ygwyuvrm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2nbcunfie.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uunxkofj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ordixqnv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2etuoyrkg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2okbzfzql.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ncszydyj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jqcznlvh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lndfdlqz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mysveoje.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2nvvseqao.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2wjmofofu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2lvkkpqdt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cqbwzuaf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nkgqujcc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mbbhgddj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ybzukbqh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2icsvzamq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2nyxkjigg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2patjosbr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2uefddwlg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2hdscmxnq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qxfbdkee.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2usgndqxc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2endahtoo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fivsbejt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ggxccruy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2xwonghlb.html


<!-- 参考信息 -->