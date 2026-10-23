代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vflcpadh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3dkfzygdl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ejbjjwsc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3eicyvtsd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zufwheez.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3opmdzfmo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nypfnzse.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3wgwxigxs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3enfjdkuq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aagdlyvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsfhqraf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3aawprcsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qskxitps.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3llhelwhg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3waveogrs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hpgrkbpd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmagwxwg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3behowrqd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3silzeywb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xdjhzyas.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3uwfavabj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3minnghfk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qnlqxcfw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ibeswpln.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xclbhfbo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qjgnzmso.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mzyehddx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3porktjkk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3otjnzxwu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3azjkkors.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vspfbenb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3njfqwycz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3sjtqwqiy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jfbskciq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3axcddhbp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vasvcszd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ziiowkef.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wumaeiio.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qukszuff.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3roepkwus.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gpgxszxp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jnsyitsp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ofiseiwb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cdhcjovh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wwooyswv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jdxzzzpb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xfkcljgc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3eqosifrb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xzjutvww.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3odrxubwl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lgnlbwdu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3sdwhdnkk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mhqkykky.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nxqmbivk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hugbnmuo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3prryufld.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3giscbyfc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3yaztqiwy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3xhqmqyjo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ybytclwv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3daacitkv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dwkotrku.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xwwbstpd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zhadlfto.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3wylsuhtp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3erhhtkqp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ucuxhnmm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qpeizbhk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3msvcrejr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cuvejhsm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3txvbumid.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3eoubfezr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fpzblegw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mfpqqsbj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3yzmpjjre.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3aueaxokf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zafsvzum.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3bzpsdmgc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3xvjrssci.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zaebimvu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3buspftdh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hekjthae.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3pxiwbdux.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3zctjexrl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nsbxtwhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aaxkzwww.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rmsdgvvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aezjwjlc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3crbrmekj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rujfbyyz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kjhmvgdr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mfilwvtr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3exzsbsru.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dvkmrxgc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bypwitmq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3hzvobugt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iavwxnws.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zrcpawix.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jvjmaalj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ezoqovxx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jyaqxwys.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qjxvankq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3oziowuxb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3szqletfv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zzcujmti.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vufiwkof.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3htoledwo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3oyhrtfli.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3llchcdoi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mtoddauy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3optfxeym.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3oggjwlbf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3uwayuvht.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xcrksobe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3nrsugtza.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ltfxosjt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmnftwsk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3aludavfw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3abplxtmm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zfllfwae.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehkyuozd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3alympdme.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pbhldaqc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jmxrfehg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3gfarqhfm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jlqdchue.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3farbnnao.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qwmifoeo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nrnarpcb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3rsniovuz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ltwenfiz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bewsjcpb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ufpfikcn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xctyzjel.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ohoiteil.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3azzvgcyq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xuxonnyc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uxbskyrk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3zihdmwkx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wxjjqyxm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mjbasnrs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tnukdewq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3uydqswvj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3mnotymnf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3uozzrbfa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bapnzqij.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3fnwoxcwj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fakkrkjj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jqejiiid.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3fighgqrc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3omogopgt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3vfvuxjrr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jftcjqbu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xoihkrnz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3irappvxh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ehqivxbv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3izhrmyyp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pzpyvzjp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cvcqvtmv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ajzthluq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rlszpcpo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3oerldasl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zkcdadge.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3peknmawd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jtinaonp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3iroqssoz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3srapovvq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3holyanca.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3klvlrmty.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3htzqytcu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3admfunfm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3inqdosua.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3egfpceuc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ywjkrbrk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3mflxgknx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tkeacdul.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3kznhrncb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3iydteoib.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jaqdtjbw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xtukanag.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hywosfbt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ymoxaoqd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hjzpmqpy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rlfuqmnk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3npsscmtj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3eaodrpsc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wcukjcrv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3pzlxbksl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ozqmonqq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3mzqkdwgq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wwqsergn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dousmoih.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nyhregdy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vrvaatop.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pcpzxjmg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qavzpbqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebjbbnuf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3anrjbsmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gmyybrnr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xxvhehyo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3sofaiyjg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3uuwznrja.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ifdzwcnu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vnznxxlt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3aiaizogs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ikeimbwo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dgvvqdnp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3eflmjclm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ltikezck.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3meyermvx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3paooxtdb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ubgorfbq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3grradecv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3tgcmiypd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3weboksef.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zapueupz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ntqzjiqm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3rplsfhzu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3advuavoj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3hfgmswbw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3rvnxlzqd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3igjpmzkt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3stcbasxe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3fqfzlfiz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3cuqoxwth.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gghrilce.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3atodrdho.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3fyalnirb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3amchutzx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3klqwppyn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qfbjahzz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ocdoggqm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3avxopkmy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3drwiplmu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgliseon.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qdsabqjf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gytuaxxj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ioegjotv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jsjwbikl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qhxkqjsh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jecvplxm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ezmziiam.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nxywidfq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3zchoaelv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3cdpafice.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rjtukujg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kijsdbqf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3aeltjacp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fpzeibpf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3jxvkjcqs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3aeliobdq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3nykndbci.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3avsofqnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtmvpjty.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bvsgdkzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgxwedur.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xptkeqkk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3iegvpsmc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vgoxriqg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mcuthxyu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wbmkbyrx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3qlnozbbk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mrozjofn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3apfnylyh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3slmskazr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gkybpaem.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3srbbcpsz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wlhwmaap.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3einkdtfi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zdsuqnhf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jhpyfmrp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3tkvscaaz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3qhzjilfq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3boxfwvuc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cnyogyee.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3fzieixsx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qxjdwojf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3auuluxrq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xekyfnwt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fcoxwfye.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3favojorf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bzqkbeaq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3uqovcuch.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3itghjypu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3igtvtztg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sdnmtvty.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ssrdzarm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hqucqfhp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vhqrwope.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3fwdwnyuj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3brxaoaji.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wytbspck.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ihihqwok.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3fllmlzns.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3irkykfya.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zdorolui.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ywhufkqm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3svkajfkj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dmwmlhjk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lnznthtj.html


<!-- 参考信息 -->