代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nlfvdkcs.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2llahvizk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2jherdytl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2plgswbgz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rwhzxpzh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xnzhjmhg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2wayojtco.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2hbegplwa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rdkhliyi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xjvwjskd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjlakyjo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2acftxcnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shmbqudb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ffsqbqiw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2odyptreq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dfrxadqg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wumssupk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqhtcngb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lgorlxir.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rdpvfbhj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gaszioth.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ahzfojzl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2psajwqyj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iwimhchw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mbcxaevh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dcweqlsh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2iruceppw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jgoemptm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vmopipvb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2nwksbszw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qrzfgrkg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kvnavtds.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qozkjkmf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2sirxxvgm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2eogpckxt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2oehzdosy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2majruipv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vkjwfsbx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2urqznwau.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mnszgpuh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cfjcunpf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xyjjxhql.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2pnfjhmll.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ihgxorgg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nxwgmdkz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2nclsibwv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dopzecji.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2erddevfz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2clksrjps.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2kbzgxnjv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nptaqqac.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ewgjwvry.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kzxehztb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqapxdoh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eymkibty.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tomicexu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xipvpdcu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2bfbilupv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fbgsiqgz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lwtbsbyb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2twaxcfua.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ifxxfqau.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ripsnpip.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qfwbexuj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2inywlceq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2edassdao.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bpmjfego.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zoakdsec.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2kuklapkd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2irmmkecp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tyrluyes.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eycytjjy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yzcntpak.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2walwsgzg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qfxvvatd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xiezfwkf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2vcqlzsgl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2meuedilz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wgjxqwaf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2obbmhhgf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nlrzpxqc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mxfinxih.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tthxqvpq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gcfrqgls.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2iyvcbbgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukgfkhni.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2felzjsgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btwjtfpr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2obvjolpg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gnjebupd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pngptntn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2odsldzqx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ysapvdbl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2spreaowi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvnivlvr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2dsuqgrte.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jsfxrwuj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2abuqfdny.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oqvuthyl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zkmugauq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hutbrmgn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2saylfalj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rnhymrvz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dzawglil.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fdoclxer.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qkqmvyxv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2clakmijg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wmnykuak.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pywadoyq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pfaaauth.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bztxqaee.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gafuwtqf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2irzfzqgq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gusboyio.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vxzugjau.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pmvfuoqz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bhdocfmg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2potpiucu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2eadujpun.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ilqnhfxf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxqjkrcq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2rdwlctgt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rhacqefg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mnjigcbe.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2lsjnkftq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kiflvyjc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2uoqwpklo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcvjluid.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2chniwddx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2trczbyzw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2iavqscqo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wsekosui.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwgegtlv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zudigwhx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kxhsqbos.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aeyjyqff.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2thrtxzyd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ovkipthl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ecabxjyx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ybxrignz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xrucoxna.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ddsxbkjq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rbndkhmx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2odkgkadz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ppnnmoad.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2podnudvn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2zruhimbm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2neqxcxwm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ktyntijx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2tgottgcb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2imdxywly.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ebxphtqi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2zwvtlleo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2twnecaoz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uccokzsk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2elfaahso.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jxqqlkgr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eahbticp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2knvbayad.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ngseerdq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2aefgpvqn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fxgxmvub.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2djckatln.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2chsnaizl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vtxeuosp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fsjdmqjm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2nanhnbhc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mcgiatgt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fsfznqiq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lzmzewbj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2gfjxvhti.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2earwjtye.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tlvbumql.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fpbmrqxs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2aeahhrii.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fobjfhha.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2llspbvrd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2yhkkwcpc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kkioponw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2boipcgfd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xxnzqduw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nzabvywi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2orbtjeop.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yhhswrqf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nmtujnjt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ojurnpqm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gvntsgeh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hhrmtjbf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zijlwkcx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2lyvxglaz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gayyhiut.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kgibydxd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hylqtlfl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xcwrnqlr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2xibdcdzp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fgycjfqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nestjyri.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2cdnycdaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sywbufen.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wmjkjcze.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2okqpqqoi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2axskvlng.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jasjaues.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2eufpwlzb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2iohiuuat.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2kmwqpgny.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vrkxwgur.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2datqbdbx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nyzynlnd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dtylxikp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2mxkdrhjc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fcdeucoz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gxzmvbnf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ypsiedjt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gthjrepj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2lxyssqyb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dctpebim.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2rgcqhsvp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nwsklgrn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2tweboqnt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2yxicswua.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2njabxjmn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hretqnpr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ozrurndp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2pnmfrtod.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2essoqsyn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2efrarpgw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vzvxwmwp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2pkeoqckc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kprhehnk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mopjyzkj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2iblsrmok.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2uzbwkfll.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2leaykqvw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehjiffzw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jucmzjhl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vnitngzv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rbhyepel.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kthxshvr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ybgldbny.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2icpyhlht.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2syyfntlu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mlmvhewr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2pgrlfrpd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ohniduqy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2tiycymoz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2odbyfbdg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2njfbqwrs.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fwmtjsop.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rwyqrtxc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2tekgivmc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2arsuwoia.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ctsxvkys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aigusovg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hpnyujvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tuwpbuox.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xcywvoyh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2fxkvkbhy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vgekwgnr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yiijayoy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fitaimlo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ytorasou.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ytumswgj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vkdhbktl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2qjidfxoj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bfuzafca.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2fuxorcem.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2twpdtybc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fqmhfmja.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wfzjhvkg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zrcsfmwl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2oluqtxjh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mruuzzpq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jubvqlan.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lwacqboi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2dzlrphxf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vtwzxrte.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gyexzhar.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vxpcfnbo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dvqdxyjs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2fdkqvjai.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2xbdicsty.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vlcxpzko.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rjnsizfc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ghdisrut.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ledokrmw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pdhgthdr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ssnnmtpq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yejgsmuf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gwfxbfdh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2onhywaln.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2iefcpcsz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2wdyahzce.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2hedvwycu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zrrslgun.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2kyppfwuj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ygaovnuq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2xiefudnj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hspfqjja.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xbhllqvd.html


<!-- 参考信息 -->