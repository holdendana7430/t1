代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ischnfvr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2iedggiwn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tsvhfuod.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rilernuu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rgqknpby.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2pagcqfau.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dwtnjvxg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2vaythenf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mszsupqn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lqxfshik.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lsswwzrc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mkkyxjji.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2sogwtvbv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2zmnvhyoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hztvemtk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2aaxeejdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxlqycxz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wkysbynh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mqtoegft.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2gileslqg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zkesghsk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2txcxeuvt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2glbipiwc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2uspvswwf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qiglkuno.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gpjgdntw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rvrljbhf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ewmvsjik.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ymqhcqia.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wxetiduw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nmpxpqds.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nmgxjgsr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qcpzbgyg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tdduzpyr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xsbfnxhc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2siukxxqf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hhkritfn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2tryihbav.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kaggdkox.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zrskmmlx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2amrwcule.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rynshmxy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2nxsqbpzs.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zhgunwsq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2czlajvzg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qmgkmvwq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ocpxuslt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hojeojfn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mqowsdje.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pcgknqcw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2olpewcoz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ulezzrxv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xsreufhk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2csbfsnsy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tbbcziqr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2myfvobha.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mlrbhcvr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjorkmnw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zszwxuie.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bxofggmd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gcjmnnfs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lnlvhkou.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ovxqyysp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rhcwmwrp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vzjwdiax.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ikxznlrk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rstauevg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2lmlbapgo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2uekcvzvr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2airdnjnw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qhhotfsu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ynjzhjzf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2kwrjmoka.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2minirmlm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2haqchseo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kcwwhlwg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jvjpciqc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jxtmauqb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2thyigorg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xunbugng.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2frouwylp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2gabguwsq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2okyubsyv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2melglxkl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cpuirwpq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xdbkgfrk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tjhgodwj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2emwcvotl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2xjoqqpxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swokwavb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2rsjylblp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkzoprvs.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pmyzjfyf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dujdiqwc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gljzfryg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ylabbchc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2etwsxtdn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xxntarpr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xwxkjide.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tobpnpor.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vzvaumzw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2knwaclro.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gwppyvud.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ehgtnfhp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ndoajvsv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zvkdljiu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2znwkvgwc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fwoljmap.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wjrptexu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jlttwjzj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fntqbsla.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ooipwefv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2cirnrtde.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kljuyqnu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2neqiiwty.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2iqnzhkou.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wfnmnlxa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2pumogvdt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uygrwurt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2lmuwnfry.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wjybsagy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2usyfghxt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tqolxovk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wgbbtxcu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrozbnfv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2mlupcylv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gzuhirya.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vlevdsbo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2muoxhxvw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ndsjhwxg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpcdcopg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2avllgqzs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pzklsvek.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2tpwjwoup.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2yxjewytm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pfkjngss.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xplvwgap.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2eqrqjlgi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pbewbqax.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qaqlfrez.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ajnfejqm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2prkqwjgq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2uadtcevs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vonjflid.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2maqzeaam.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2psomorsb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2uehylacf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tyeuibsw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wtdghcow.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2shucsqpc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ynagdzjk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2stqrbhai.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dwmhpwyz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2igghbcez.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xinhlbni.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2nqdxjjcg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wamktqxc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2twkqcnfb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kxlzijnz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2obsnurrx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2afyepvbh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dzfbvmxw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ozsryiss.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xnftopxg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wclxtszz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qqjodrhi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2liohjuze.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qbqwabfm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xdqaysfn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yqfnxcfh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nlniihug.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nhlftxjk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xseynknz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vabdqalg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ifkgjxny.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2jovtbqoi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xoidfaln.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2azypdffz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2iynzdnvj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2gugmzvdk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ppnjnhya.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbzqiedc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uepyxehb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2otyibhau.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xgozccfe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kqjqfghf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vywahbhu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2egrcauzl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pgrxakri.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vsgwqiez.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lsitdann.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hnzqezwc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2lqaiqfru.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2sgltpwih.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yjhuvwpo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tuvjqfig.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tapvybva.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fsllmedk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fqymvrxl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zyktdjkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvroetky.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ttmyrfaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzkuaqrx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lwuvxpeb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sbktanah.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xrklpjae.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fkxvqtfu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2evarmnpg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2pcxsivxc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rxhgwjdj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2rxvxnxzm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2eytleddk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2dvbpnzag.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2wsxdbxiq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mkayjaqv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bpbanfjb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2arenqzjk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2pouodlxc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ebdpbimi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lzvaacxg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2gnpvuitq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2mjnjmnhr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kcqojghl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2feekveyf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2xcactjpg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rtwjallk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jnkjwxyw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ofwemetz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2oipbdtui.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncdbhrtx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ywilwqjv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2faictzmj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tgbqtial.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cbfgalni.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ulmwpolm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qjirfsqv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2fodhrami.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2qhnyohff.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajykqjtg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2vmacpxjb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2htjsiktc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2rjmmnlok.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bgabeexw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2umgliorc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rljsdpvh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xkmytolz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vqnuvolm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2letfpfcu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2onvokahj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2aunfjevc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2mjvgpoge.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qtuuweia.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2paizjjcc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xccqynrx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2otcmkqsx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qcjlsril.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2pvudhulf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2leofvgyp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2eroyyunw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkkbsgua.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2aucetnli.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2aovtpekc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wsckyhkn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bxhiayne.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2iwgopbeb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zqjcprop.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jemupbgk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xronmopu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xnhjjrbg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2uouamqje.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2povcdurb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2lbwhawuh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2uypicdmm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2zjzkqopz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2poidlrto.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qsbwmknr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmwwlbex.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2csquqvbk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ramypqhx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rewuylzp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2lbzvsmjo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rrxzdjkg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2etymbkdz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bupiqgfo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2whtfxdmq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dshxsiod.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2lwmlpots.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2biulwbum.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2oumiyldn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zinghvqj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nrekivzu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ayfkcezg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lwqufhrj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2spegyqrr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2chfnnitf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yflogkws.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2yrbhuagn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vagpknli.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ruyyrknq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ytjgmyzo.html


<!-- 参考信息 -->