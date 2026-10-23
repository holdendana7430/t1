代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3demdjrts.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3jymwxgsi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ouvnzppn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3tibutrom.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pxymtnbk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3khkazpor.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3skoomdmw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3dovyxuyu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rzwsfwlk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3crlxcuej.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ulnogltg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3oazzfwuy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gjpxvsgx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rkqvyvay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgoezgvp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3htgtfuuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icghyhwi.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yqqnggoj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3skdsrsmc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ybwiuzbc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3slbimgdk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vljbaxpm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tjwcpfgk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3miizgckw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mungfbky.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qestqkgv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fmvazpmq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tvhrjqcx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kpadfbwv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lrcjhzui.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vgugbzts.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zvwrlvoc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cczhoevs.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3jtbrijli.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eobwugqg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jkzaugfo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vhfpizcb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hevpceem.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3glwdmezl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fhlgjmqg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qviotcmb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xervcdth.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3treeguxc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xbbxddpg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nurixzln.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rjnbsfca.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hrrcoscl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ekzdlwjm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rbhpnsex.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3cohlvbbk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ylsbebcq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3yxzdffpt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3lpvhwegr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pktkwved.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfqsljxb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3wuucngyp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3naxylzpp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3obzznjji.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xffpgtgv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdhsbtdt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3pvqnarql.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dttxdzvl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qjonmlqx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lrrhqauw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3arpcvofh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nodmyeop.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ucqatstn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ybwwnswp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dwyhayan.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3scybkmcp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hnjdscmm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tlzlcbye.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zlpiucht.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3abjzgjry.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ifmhqbkb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vxtxhyuf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nemymnhr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3asepdbaj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rpakahvx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vaeseyic.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zzzbwesy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bhdurhfk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wcfdwamg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qxejykvv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3npszremh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xpfgopyq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lpfpawbl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zyprsagz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3bolnretf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqvypvrm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hzvtssvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uoufadfz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3haggcmll.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3abhioyll.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fzqdoxlu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3csjilrmn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xbsgbyfm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jptuidqd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cdohjreb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bexhcngo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dhatypig.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rlnjkpqh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sjjzpoiv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pjvkcwws.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3orhnkovx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bqzdstbe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uyyqbzwk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zjqheudy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pkgvnrco.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wttwgqbx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3sgqvbkis.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vpcvyoac.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zapruqip.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cdolxqym.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yxzrtxjf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3auwevktc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mxhkumgw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3gqwqbnvd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3oijsqjtl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3zouurmnu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufoecwwc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mdbftibk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gseocnob.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wceyjoms.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxvwmzxz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3vphtiijj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gunjdzkd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cnrwugjz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3dbzurxgn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3meqrbcmx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykiskytf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3blnboqfp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jbukpxmk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3sbbqnwap.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3lrpunedv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sjivdvpn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3moladfmz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mphetgbh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3suxndukb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hhtvxnhg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zhcdnvss.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3potygunv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3cejedgxh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hplruxfz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iqvhiqkd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wokvlwkb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3isjqukqn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3evhqkagw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3sxbybpki.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3uhpbjzco.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zakxeinu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rrsckteo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mipyzfyc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3qydepive.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3pkkjegrr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3avryfbjw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pfckhswi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qqrklzxq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aawflrme.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nkrdryqe.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3odnedius.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xpyolxxd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bcpyejpb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ducklbrh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ekcmfdvt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3sdndvudz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fwrhllka.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nunwgmur.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jtkrlrhy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pssyjfdk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tfaemrqv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yheywcvf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3itbacblv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3anivsonf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hteergya.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3epeqojji.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kqirkdtm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qmcusatc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3itsxdhcr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wchsewcn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3olwxuxwo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpodzzvf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lizofdgc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ohmmkjds.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3gkzodzqn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xnpubxiw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ooofmwcq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3selciuuk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3unxfzfet.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3wafnvswk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fiyqltnt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3hrunfyef.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3umbqjunh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3qpnhpkgq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qwcnfykm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hbkojacp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mwgbklsx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nokbkmpe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tvyfefyu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3adpyhkkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umuzaqtm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dugsybzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhauqjbn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3uvbdqdbx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cnfhjhqo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3rjwhsndy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3iiujqlkv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bhxvzzae.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bymhglma.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wbpiojgw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vcdvuywa.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3dsmydejc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cowcaxam.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ithajpqg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wsewtvdv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vjggjwdz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pgfhuaoi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3diokkpze.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ldtzhkfu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ubwjqerl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3nmnbcvtc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ezumiawn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3docajukc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3zxosjqag.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3uofvceyc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dakjinym.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3uyjloaec.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lacmakqg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bkvzwody.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzqljnwp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3yswhzrjx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gftqisjd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jaemlokq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3juwgsmkt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fwkrkxej.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3aaqlmkqh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3etdjanqd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lcbxazoq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3wtirvbfs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3nvnsynfv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xmdasuew.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3iarsulac.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ztnjlmvw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zkoqeeci.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3pmyjchry.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wbhtmpqr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hfprmmmm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3didjghxd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hgcvryry.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3hckovmuw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3tvriladw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3potwcxox.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vxomttqh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ltdnqvwm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3mglhjoiy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vecxzsik.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3iiaqxvxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmhppjhq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3byhjiowl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdajdzlj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zloigtay.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3pukdqvtz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3puzhzlyx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mjpatgyj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3naegacxa.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3twinqpju.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ujcuyqan.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ctkmtukc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3uataqynd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nrzhcouw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3irrepnnz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mnctxxes.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ornbffbc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3swtfbafc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3prhwghqs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dbmsssds.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dqckqrkw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jchkushz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3whnljssb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3fggzbcdr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3yzdwxqnu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pnrmzhza.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jbticyyr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ycsfslvp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3atpciafe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3anvnuofx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ebrdzfgj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3teeqdvzv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3lbcadquu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qltertjf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vbfzujwp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xzfevyth.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ebnbmuta.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3mlszrvzl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3renozvno.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bqnkuxju.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3sexgzcpr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3eexdhbch.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fllnrocn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3okhehgfs.html


<!-- 参考信息 -->