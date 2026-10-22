代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xiylxzsr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qxjwumzu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pvxzgnzw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2urypvhmy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mcpdmcwa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hqseapqz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gmvmjybl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mwgdhtxd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gwzotrck.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rffuxeug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lshyujpf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2zbyuqjzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xkaxzlvd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ywmashrb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2vrtkvrhe.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zbloefvg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qzpbbdwl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltihrnpr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qgtarwhm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nhxsqltp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vpgqshkr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hnhdswwi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mqgyntin.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vyjqythx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tlpeddfw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cfvxmbbk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ostkuqdp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qjppyjup.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jkhzjrxw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2yfvzbaku.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jisiwhuy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2shvjodne.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ccygjqza.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qaefkpke.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2szjfhied.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mikggmie.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xqofqiqp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2eetztdeh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dqhbydqj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wbhxrdqq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xhbnvkib.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cstrvkum.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2obvmyslc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cjiadrnn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2evxgtkkt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ivucbnnj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2thwiobed.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2spzlikbx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ggikndft.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fbygyoca.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2golvhvtv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2pubwkhsj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tgygmaoh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xxibxnsm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zgscizcn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gdmqqpaa.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2nnpbxjtp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2toimgptd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ofxraazj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sklfmsxh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2dhpwzxxm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bngezomy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cxhxukze.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zscrwniu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2fvgywtaj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2jrilkjcf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zodeugld.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zcafxgod.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2kuzdfxhr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2bkwwzxlq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2umzhsbcj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qtkwmhok.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fueaknhv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xgdxvtro.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ktstdhxx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fhgdsurm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2juiuzuqi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kpvighar.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2racgrvsa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uypdrlrf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qqaskzcs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2oiexxuiz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2febhbiqf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2zmvbqryb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2htohbtjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2albxwvfn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2xoippaqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzrvagej.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ykjydmeq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2inlbkutp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2epigzvct.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2neuxvbvk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vwtxpypq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fsxufmyd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qzlcbpnz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vbkndwlw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2goqbxedj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ouzdqrgu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mheqktvu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2miustcff.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ivjtsiac.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fkghtlgx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rjhkfsid.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sgxgpqqd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rnnqkhru.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2phtjgriu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vpsxnjih.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jqynmfbf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qznwzaws.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ttaduxml.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ggcdbhcy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qijltynw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wfobvtcd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2lblqdggj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uvvyhrof.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ocdnelpx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gfrcofnt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2thjdyyhn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2msndjbgq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zhsdyhim.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2szopdlqy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mtvscjnx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rfqhslot.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mzrpxjyz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2duqzijfe.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tbjbiezu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2lyveupzz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tybxqxqn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jemouekl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2aeoumjmf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2uwietlve.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uittytys.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2rctzldqk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2exqgmumr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rgfxrrkk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2prldcpqv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hujusmcy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xlzchrlw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fcfrvcwd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qiabqdxz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gjmkdwfh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lqpiqqxm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2omsouiig.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tmzzbkkh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ntnortxk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2odocdjaa.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2rmwztygv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zlwxqlrw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2odkneqdr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2dewonlcn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2kkbsocqk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pkqmdovf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rnmxegdy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2gdjcfvtc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yfpxwdxt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xsckswvw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2finexzvj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tfztvqhs.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lvgxeyxo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qaivqdux.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2iimbbzdv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qttjbfzt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2inlqqzhk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mqbuyugb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rgktvwod.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fdrsrjbw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2glkmbrca.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jwgjtoxd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2sdfaqpni.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2cwplwkuk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dbijzokg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2vtowrebf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2istkyvmd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zbcinmgb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2spvbbtzv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cdrpidaa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2nhlbomla.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfuoneyc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jrwgfbvs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gbhroftq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjaatihm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sznituxo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jibyrvgl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2flrnybsa.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xqyfwqsp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tfzwkekh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yfkfvubn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2rqsqnpix.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2srkeekvk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2mvwrdagm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qwyxgzjx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2faoghikp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zaojaaps.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zlbznrrb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tisufmms.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2laruprcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wahgjlni.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wxmzudez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rexsekgb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vxzkimsj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yrpsawhz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2kciknsub.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ifkrywhr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2pvludqmc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2imvzknbt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jsurbxmq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vomxgnty.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2grwargmz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2uzdxmjht.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2lhzyeqky.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2asjsxzlx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gbklzpmz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bkyjfdwk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2scolnocf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wumpylod.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2fxqhmmjk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mzdjzcrd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2uiohfssz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qnxigvlh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wlxloayw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2djrmxanz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nggarjvy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehsuhfvm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2aewozllv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gjwowxma.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwjuqbfy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lgjgwcrx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2toogatdz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2kpldipmu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jpffdove.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2shymupyi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zcpqupnp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2agudkzud.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2weakylyp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhslrooh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2tchirpll.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wuuuiyeo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2bnsldybi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2broouene.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fdfkqiha.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2cismnezk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2lojigvfm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jcpqwajm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2szpphcht.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2abzjtziw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2awcoxght.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2mazvxnzj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2onkzsruy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2oxdpdvmo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2axaijivj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qygesdzq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2byviakwl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2txrpzbxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zuzrpfzz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2miwtecrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlhujqbm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yxzyibcp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qvmunuqj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qnhuplec.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ggyxvfzt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wyysoxyv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2rhmjavqh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2faxzagch.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2uiegpubp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2pclaudxw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2hjzjsaur.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uyqbwyjl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2slwtqwoa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2dyjilvjt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2dxepfkvo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yqisproj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ygobpusc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bgtorzhv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2tcpdtdfs.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2scmzutiz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2hgnarruk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bybcidlb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2viiycwie.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oogtcxma.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ggrumxsy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2kfiofdjd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rudwezef.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ltbaeupe.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2gcikwtvm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fkgxrcft.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nzrwxntt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2uxtxincw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2teodtzek.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2monfhhxo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2emnfhsse.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2plhkmwye.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hwrheoil.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2nuhjoxvh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fssoypxg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2cmcnsgpt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2cgkthhxw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2stdraeig.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2iyvjzyab.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ejjxvxib.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2upnznicv.html


<!-- 参考信息 -->