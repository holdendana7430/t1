代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2udvxynip.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2bwvkexpt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ggnguyov.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2mfykancz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pngkxllt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eowtmtcb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ffrsooss.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2imeucova.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nuqamfad.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2hjmtfujq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cpmmisvc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2zjiixiac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uguclkfh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gqatvaln.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eldgpllq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ltglhjdk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2swiajlsc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uwrkqrbh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nbgiwnyw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mnrcphbw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2vnxqjlub.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qboiqtug.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bktpuggl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tiwxebfx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ovucbopv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hahpitsa.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xmjfyrmw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pomfhqsz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xbcfefqu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2oiqgnyun.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hzqtjcqb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jblbplpk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gnbsictm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vpspxcre.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2icanwszf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2queozbmw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wclgjvwv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yczqwftd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fepytmrk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2yypzoxpj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2winxgzum.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ayxvixhk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2tcaaifik.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rwkfjquj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2aqwoxhxz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2rwcagjyd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ltkrnumz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2brntmfpr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2phtqtsdl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2oflosmsh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mrypoptd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rzahlhsz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvnzinnj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fotnngxa.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jqqozzjl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ydpirrvv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2csqoabha.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tgvmggyy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2rejiutjr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2czpbghtf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2iiiepmoa.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wsccmmrf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tzcuuvry.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zqxowhft.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ekmevror.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bfxyeizi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2nzbibkar.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kupxwasd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vsbclfxh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2fhhfewac.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hucsxxry.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wvltuyjw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2azavttei.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2yhzllxji.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xhvfclwl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xzvkihbm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lkctprqi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ayjuiqrk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xliclibr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yweczkkv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kqmgqwft.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tytlzdsq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2kwvrypnf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2urgmlrxs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vvccmmin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syqbszyj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lhvdkeoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igthsbmv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2bhnrisvh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpgvjlpa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fconqaqe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oylamcaz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dcfzjmvi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjycxpew.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ovuikzfy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2aerbsnud.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tnzmtxah.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ogalywpk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ouhtbdiu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cqtojjfq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2aowyiqno.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vickvhbt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ltjrddur.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vlfkznlg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pjojupyd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bcnyycwl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ysjazbke.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2nujalsfy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2zsiuudxo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nawwgqtr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tubcewmr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rctyxwdg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ygtnrjvo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hcsoxdfu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bxustgcr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2yqrpqexd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmekgmrw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2iodlzcgd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jhncmnkf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sydnjjxg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lmcuqbuo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2zlrtzjyr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkobcjcy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dsowmehg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2baafzcfr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2adrljxhb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2atdkdbnh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cphcxxhk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wmughcio.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ewukmmff.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ofdidrgt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qyjmvgls.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2cwiqguck.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dcubunny.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vivkydjb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dbzpafag.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mctknybj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kzjwpicz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2talnqrxp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2fyqmrwhd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qxiuebrt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dsinubbi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2edsnswye.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2oomjbmce.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zohdvxqu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2qkghsqnd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mambchgz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2obnxytre.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fkfsywhh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qqrrhgwy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2uaqqwjdg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zbstkxlq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzvefoqq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zkxplnvk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jzhqvwri.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tqlfluig.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ibbtjgbe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yotdzvln.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wfdfnqzn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qcryouqi.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2udmvvqdg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pqxdarsq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2warpthzr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yskdiutv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2jvmnpbmz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2frqbroop.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nexgdhym.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pxukntlr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qtsiqfmw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ahhpeaxc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2khlayegg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnborsaf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2oxmehdzm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2iuboyfcv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2axnxibxd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2yqehpbtw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2errmjiil.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wmooidst.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2sjwbtkam.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2wovlawrn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2lttmfzci.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rtfcmdbw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jjfqnmis.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xndufccm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xolzlctz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2enqkhwmj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2krzkksiv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yrexeafd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nazoblhn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2owgybcrs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rnkumbpz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xqcsqhqc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ydudazuw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2axjwylxz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dgysvwuc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ujmkzktv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcwapttn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2lyqqcfqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvontyns.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hwbyfxzi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2fchtkoso.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2cfrffbgz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2eqtlskof.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kogepxvd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2hzdjuwgh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jscpbvkt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2cwjzewrx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2olfmobeq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ugbmpkce.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2pdgdjiot.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ekcnsket.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zgaqkfvm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2esocbadp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vrhsnmxx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2nrjkdjbj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dyleqqrq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2uaciklok.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tgniakcm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wanubfxx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qwvixrck.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zfpnxdzv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bujfogti.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lbluhwte.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2nuobkiwv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sfcyhujw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xygyhage.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2uicrcplm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2lfhdtdjz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2fnlocipd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2finpvdic.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bhjdrtks.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2avviispj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2teduwydp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2prxxuiqy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nntpsbgj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2askxjziy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2slkwaazi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tmhnswlb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pjvglhvr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wswepneh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vsnrbmcg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2pkubpvwn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2coquteru.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2gjponhuq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2uyswfxzj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ugikddbl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2iltofwtq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2phnrzgri.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2defgppql.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2oxrjfdzo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2otokjgls.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ortcqbte.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2axexelpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzfmtlvb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xrzsurlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecesnoci.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bwxofkvd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2luekdene.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2olbsucqy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lnbzvyvo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2oqrhapxk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2evhglnyr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2kuyleumy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xhtsteud.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cjxbkfzg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2rfgmrjlj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2yxgjcznl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ndqbtgxa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dbjnydkk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2vfeudkbk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ggyoknol.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ogeqfsiz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltehqxap.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2wxsjqqlx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wfjeonlu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gbkgejlk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2wdixopuy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tzueuolr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2huoiyasa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2hhxggoby.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2waomnnbk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vaodslse.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2dxmdzaxc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2woqfjhep.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cltgwgyb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qdtxkeer.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hncvlbrx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2appxeegs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ecpqzbnu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2quraamnt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ebrbfuym.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mmtesurb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xcdxpgkc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2lfsueckz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jycfvvqh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2edvsnqyl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xrffduwk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2eefxohmr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qmfjdktn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hgkrkzsj.html


<!-- 参考信息 -->