代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tbtdaoxr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pqbtfufw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3tgqgiity.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hecmsdrb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tsgigkum.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lzgctxxr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3phtwbhxs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vrklsxdy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3umurosop.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3jcdzkxrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irrxejaz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3tbakturz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbkazffn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qrcwftzl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3htujuobs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3zwsizooi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jklavinz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ixcczxcy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3amasrwwy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gfalvzhb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3imkhbtfi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bhsxjpqv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3icttdsvx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3obakztbl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fupcttxb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3oxjjytyy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3geqemivx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ecedssci.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fnzwsmrf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bhxixouv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vfsqeivt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xiadlllp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xtsehxgt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ynudizpe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zqezwtlw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cqxtjxjq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qrgrmrxr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ytmouwed.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jtikceoq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ylhebzcy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gyqiadmq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3shupetts.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3eaemvsdp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ayhpuzko.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qvzgahji.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jtaidcrx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zrvnerpw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3pisobedx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qehugiau.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dovhxufv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fgovvjzp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xagxksut.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3etdzhlxg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqukdmsl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ykqkuqef.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qcsnddxx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnjmdxch.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tgykuyht.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tzekmvwg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pdudbrfl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kvlouont.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zokofwfz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zgwjbvga.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iznwiizo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3yncpmocw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3begfxohu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ybpzuyod.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3oxztsyqg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3mhgfbxcu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3doqqvxpn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nbwchyvx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mzyucmtk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vlcjavxe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nvlnhwzo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ilersvdb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uxsjyaet.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vclbzwcv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xkdzdueo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ouvrsmxf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lohghhpk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3suiornxw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3pkhkbhfg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3chmbgwnp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xqcantgm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jacdcoim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htiswlef.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3qjndowie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flqbmvjv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3serdnelc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3akhmzcss.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ejrlhull.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lwvjyywr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3izxiwvsj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3awvvrbqf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vhbnfixm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3acixdtwl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ejrkzasx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tktnzwpp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gdjzqitk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3edbaqyts.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3icbqtpob.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fhuyymrq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3bvcuciqn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kqacurvy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dtdkqywt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pjqwtzwz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3fgljaxaq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3mzvjyxwh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xyulkqud.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tgejgcxs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3snbnfbsv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3gjojdasc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ywjbscrr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jgybswpu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3twqsakwv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3eoeynbvp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3srywuzcz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jaktrwue.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3djpwebis.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yvduicif.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3znwitoci.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3gqgowwiu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3fjwranve.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zslsuqwp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3exqcqbci.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pjygsvae.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwcvffab.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxnpesqs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kjsicxth.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3nvlzjjex.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vtwwvbbz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3nuhxcofy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwjuhbjv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rfdzezay.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yyqsufae.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kvpwgdey.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xqfescgn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xenhsfte.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hwqmqjai.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3yymebkau.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hmodprpg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pfifbghe.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3bueisrvp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wqfbdfkd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3hmpgvapm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3rjnsjble.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3sykljqaa.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3nknaeiqj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3keholvja.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bbcbysmz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3pmeqevkq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bunaouxc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cyukybop.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3lzncoecp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oyrongda.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ktrouaog.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3goqwghkg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aecyrhpo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gqlhqpch.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yyridyxe.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ftntluuv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rhagmqyh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3szhrtwkx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3stxiuzoe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rzbizpuh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3iakojggq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3setlvpcw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wfrdaohz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cphxjova.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3guhkldaa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fzquhzpt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpaowoye.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3hmjzuids.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3haweilvz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdkxsvle.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3iiapwaxy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mzhpjfxk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxhxmfuw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rjstltfj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mqyzsfnn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3qtjqkucu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nnzapppl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rdewlhgq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ebzejuyk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sfarluck.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3vzxmogsf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uzwiknmh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3iakccwvu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3veycowfm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hhqnpslp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3crgkrqdq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fesllsde.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3utkgvtfn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mnpvwzoa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hpwbvnbg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lcoqbuhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snihkycc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3vwtksjdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrvkzcoh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gxzjauet.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wvmqvgwi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ttejcczp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3fyjdkast.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bykpimnm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ehxxjyuz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3tormvobp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mjmdapev.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3yvwnpnvc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hmmqzqdg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3vqkzcnof.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3islertlv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uvueluoa.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yqrhysxk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3fokpneob.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3jiuinljr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ziuapevj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zlvmyeou.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3codvbmnb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cokbkfuu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gubobmyj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zxlcdzqx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3louijdee.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rhlvehlg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ugbustkz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3oggirlgx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbtpjzyp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wwxnvavk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rcnxpkhp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3keshprqv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqjjziut.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lxxktopt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mugbnlay.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jhyjouxk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yshqwkom.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3msiaisja.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ublnwipi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dmfjbbyn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jhvyrsds.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jrxjihib.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gakwcpms.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3itiyxuug.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zolpevhs.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3umylffjp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3spshmxki.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kcxdvpyw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wgwlfoqd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wfnyfdub.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bzfpgkzt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ugludgzp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3igjxjwkd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3fptvvlsj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jousvepw.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3mvmpljug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3niabwxng.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3kcjcrail.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pchzuxwa.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3igqhlmih.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dqfrgvbq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3yyxpmyqf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hmcgvkzy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3sezxkioz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tlrplgzz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ucjoozxc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3prcxylqr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mjojjdpv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ueefeusd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3yevrvtbu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ihscafvt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jjeegzlh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tvsuwurf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fybgruoi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3hvnlgpox.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evlojuoz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3nxzvkepy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lmukinpy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3womtpnzl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3agdodqyw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3agssbzyl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3sbnovemy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mxxgitoa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3wlckxjwy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qcvcbxqs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ktdpfaiq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3boczmchx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nsmmrdkb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3axwhgprq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wlwmxaca.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3brabstew.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3shaadeuc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ecylwmau.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3lhglrbsc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zijomufx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3kerwdiok.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3oguoxvvf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3jdstsfqq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3rumxjpza.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3tledvjrq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3pwfdwryn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xlfnvmcn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3rnbekscu.html


<!-- 参考信息 -->