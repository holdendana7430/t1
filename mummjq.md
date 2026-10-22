代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ziqwncdq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fihnjvyl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fnawgxzp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2asmpragw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kupgrckk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2zzbebtup.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hvezxeyx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ikbtxtwn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fomhsrkv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ldkescgt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ehdnvuah.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2icptmgit.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xowkfvrb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bmqemhgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tiydhyyv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ubkknqop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcyynezp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yglfujfx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kvpdojsb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2yckboxnz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hbxxposb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2eavbaixb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mmtghuot.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2oferqsag.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2xjiucwjp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hjzektoe.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lrirowhy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xuwxdxlv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gdxxtkgt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zrhhbhxl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yiwtjupc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rhervlqr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cdknnqdu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xxkgetmo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2owmmlbtw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2phxirsog.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dlbfuyen.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2evqmsirm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kxxgvxlq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2imltcpzw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2cllbiqod.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vqzebwrk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tysylysh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2aakeaphv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mmkudnfu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gagvwnir.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2vtwujqij.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2faixuefd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ahjilqnu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cdpjhxbd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pocoydxy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2twmafzyl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2gsjxfzjj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2sqllnvgl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qhocpqou.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zrlkyrnb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbhtjaok.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjdfqptd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjzmbvwg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpmgxgka.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xhkxbcib.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wjvpdjsp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2rcdvccyo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wigrxooj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tiicltdg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2chuehuhe.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gnjlobfl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2edfysbvc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jghfbhxr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bhfhryet.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2gmnewcyw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ltftfvbw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2uvnjthuq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2muhlubti.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hffvyban.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dhoozqwd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2glvuqrrb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2miwvhefk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nggzfasx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hfeprzcb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2wawclvcx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2atylyhtz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2euypsomf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2amfwhovc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wxxuvfgd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sxntojkn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ohuenret.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2sbhvquvl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2esdsisny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihpwhsqq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kawjsavk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcaweuqt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vxgppbhj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ognukkam.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qeerjwld.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kbkizsuz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2corulutx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tlnweori.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2njkqguuo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2keyhqfrb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2estllqjd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2wppzunge.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2oorczuex.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rvgvvssm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vltfzgku.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tjmjqcew.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tleyrclf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2eqovonxc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kckguvkk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zjlobvwp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ansrfevr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pjiqspnk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xcfqbctk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mzyiphoy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wvqxicus.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2luoatlnf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tutcclvc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2otvmzdmn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2grphbfow.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kukyohod.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqwyoxwk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzklwxwv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ydtqzduz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wscdzqni.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldqlgtme.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2byshnuni.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tslyexwb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mdfhygub.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2czzwrkky.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bnbmgolx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2coejmvlj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fllgasgz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zbjzaeqt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2izjlazud.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2whteplpb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yargoyxa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vhlabusd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gmusgwtj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wlksnjtl.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fsiedcpq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pekdhekw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ehwclbty.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2sqihgvlm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vtkxhfbb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bkjxmnef.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mcgzsjfl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zaaszvhx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cixahdpt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fhznucpn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2cciwwobq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lbfcgrpk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qnyffsdc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2nqqsgnes.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vsakzrtg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2afalzpmj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rdcdnhiw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fanhozkt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2pzoimbtb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wsbewzfm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ejbarmny.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fobdoglo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xsitepgg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2yjtiksuz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ovizbqtv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oykbmyfu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ufinpiop.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2glhswybc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zxjlkoyc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2kgbjrsnd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rbamqauz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2vcwjyfpv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2puupimuq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rcydonss.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xdlmxwih.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hpgeuktc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2peffxwvu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ssacgnnb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tmxpuodv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2atzuuvzf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2uoxlxcjp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2nrrgeges.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nljzfzoh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xxtauuwc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ixyefxrs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ruisndcj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fjidlbuz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ljeeiguh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2apfpuluh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tyzuoewl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2oxyafuit.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lkhhyrsl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2plccupao.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nfdunltm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2nkrdtsbe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ioqfrmuw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mwauiltj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2iikxxxfw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2smemoadr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rkdvhpln.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nugetnok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqipvcwm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2cqwnjecn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbnswzjp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ggeecnnk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qkeiomqz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rpksnvfz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ejtqoens.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cdkuekar.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2rceetbdj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2owlkxkhk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2rhebfuyc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2cgwrdlfi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2abdlcqrt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2derxnkir.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xmfjzvvm.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zjzdwijp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fxtkibnf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wdsahyjm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2tavafblk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jfcetclb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mqkouptd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2eeimsoqd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zmrjqokw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2fwosttfi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2yhemoxtd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hbdmdirs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdsbcvqq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rlwjkpqd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xkwmmqtt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2aephsckc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dxbgypkt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kvepbscm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2uknzkdob.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2quvghcvo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfpeucff.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2yipoejwo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jvwjcasz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ygqttbul.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlsoovrs.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2chekuvej.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dmpnupjv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jfpkirxl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xjbxlglb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lfhpvnnx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2gtntmcvg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vjbgjdfk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pgdvlqdy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2fdjopyst.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2umwyrpeu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2rtpxwudb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jxbemdzu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wyqbmibo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2opmqmiur.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2daifdosw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wbuitoio.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2uwusehtn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hxnvlrqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpayflld.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ahmitsmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2icwemtpn.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uijwdyrz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rqpdoecx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gdezpvms.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ycplfxhq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xjvtmpne.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2soqsostd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2putpvnlg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2tbirfmjg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2kojmwpkb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2uahhcuxm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2taffaglf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gqxnuxzb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jlolvbca.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jyubffhy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ysevpdyi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2dhsozdft.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gschxjhe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vecamjds.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2tjoibctk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2adbwfoys.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2tkaofvra.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nzwzzsfh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hondmzab.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vgrrasjv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2frskltfz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dpmdpjrc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2zdrahugr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2zxqbrjju.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2zgljdmmr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tntvhzde.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2voodauyi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tigsujss.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rfmvycca.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gvurafgb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cozhclhl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qudwkzms.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ehbrtysl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ubowqwin.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kfkcleow.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zxfabdwo.html


<!-- 参考信息 -->