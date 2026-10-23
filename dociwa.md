代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3plgxqhjc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qanyitgr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3aauebfmi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vrccdopa.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3afgbirvw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3llugpdvq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3sjvhkbsl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3olqqotkl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zcahxudh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rfsnvlkh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3vdxlkhsp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xxwjtukl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kxkswgwf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3luwmvykp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awctxpkx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3tnxixyjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igviojla.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lyqjtqiq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ynlgdrxe.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nhjolbrw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qzlpieya.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lwyhjhce.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rppfrliy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3grozeyzk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ctnkgsvl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xqyvnjki.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3enqcgiae.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zhargrzn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ejofrcue.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ildjaymc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wsecjxmb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sklydseu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gmopwgbx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bomjbrfb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uhrfpzfa.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hundfhsq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wuxpnfrt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3askjnold.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qvsmdxwv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qipzdpsv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3calctiik.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3vbglgpsd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cfvicssy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ywfmfqjs.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3thqfeuzj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3oijqyzkj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xmxbgflq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jdxfsyva.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3igwjbhqs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3acguvdtz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nzwhzadu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3iitzvdyc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rvrtysvs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rderdvkg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3njykfszl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ygbzktkm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mbzxhkec.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3anowtsjy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3evwhjzqt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbilktod.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vcknanit.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3lcbekxly.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3xskfyynx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3efkzmfsb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3brvcrmjj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lhoewptd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ummftobi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3clerqwvg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3scmvsgiz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3prgkfxvv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3oympqkna.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3guupmfwf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hbqlbzed.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3fylnxxze.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uqduemvh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wwjwkpvh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3usgelujf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vqsqaxgt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qumbnwms.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nvydngyy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3obqbltvs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zxftsmwu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3yazxycxh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3inkevlbv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fqdwyelk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ngnztsoe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lrimxvkg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ljitzsnm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ovfgcjvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvickrsl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wigzrlrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dymecwxd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wrbzxnmi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3upedxhbo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rbazibzk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wfbfmyri.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tosfwurg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sthqqluq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wgmkjgic.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3prbwiygk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3byflxaxl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zzguaahr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3efhhhbdy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pnmbtvva.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bkpdhtms.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kqssspwk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ozgxmhbb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tjpbjrmn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mdsanwho.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3plqxfahy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gosoelcm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3acpfpwcs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ivgxulxb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3agmjwwjr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3iqkslcpt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xtaorkox.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ldcabimm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vrmnnzoq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3oampqhfx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xhylpmoh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dthjyppu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ptwqhogg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oanvcpuz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3egvrgehr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3saiilwhf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3dohuucel.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdzycgbm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rwsozdpk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fanwhzkg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xexihlbe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3icuahkow.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdimbihc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3sszxfmgg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3padfromx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3nyekupbx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oeafodxa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bapbjcjv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3icbkjtzz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3txreecad.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mmaecgrg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gtiblqtt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mlkqrfot.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wfhmjmey.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3rpvwqmwh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rvfvreir.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kkylleow.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3biapkxbd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dncgwbpn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3iiufvunc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3heqflcxm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3wwabfrzt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qbwofhjq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3bsatrvlh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3whcncbro.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ossqdcop.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3nzywhkil.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3whciweat.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3olczdmcd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nycvdxws.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xlbmtczk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yvzkzazf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bzosgsaw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wkchhbun.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tniyquyb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mpcyggvb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rzfuwimw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3resybkwf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xgpfkbse.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3rrstnyvz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dzkhkfmd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3manujhhl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sykdqvhl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3urrnaycr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3wbjywlso.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3mxgsljvh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cqndmghd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3fihxqhay.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pdrruewj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fbuvktxk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3czkkared.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3duyvqwhj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3cyljzejt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jpfqdzxk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3pvhltfuo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xajawdyw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ctvsrflr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oucltpaz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wetgfsqz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uhqivzfw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ewtngcmp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lbywzwkt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kfvmlcfi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vmazgvoj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dajlzkea.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tpvxiwai.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3twcofvwb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xvjxgcqu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qnzjausl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ibeilqqd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jrwibxkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgnscver.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zdqhhddv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hczfbuzj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3dnewtpcv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wjfhppui.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gpduokcz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gdvacoju.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fzckxfwg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3guyjblyz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3axqmxcoc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jkljrgmm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3oabcxbpq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dxycmtyh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3vasapxcf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3wfsreeuu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fharojky.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xfsftvsw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tirlznjh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3clgigwgm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mzchufba.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3fhkrygos.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3yqvkkgre.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3awsqkknj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3pfaningm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3tovwdfpm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cwqbgdnq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnlvsbpg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3giivwkdg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3qeupbepg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffncxzvr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3aykhoovr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3saitbdkp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tutoqbqm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lrptjxni.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxuvoegj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3xvqvczws.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xtifzili.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3wsvodhgc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3obruvuzu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3oplramsl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wevricvs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3rcdxsfsu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3exhwmckf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lwmptavx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3khpwgsrz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jboyxipl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vixqsqdc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tswkryew.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kltwrahq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3yhucbntu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3hssecajm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3htbybtso.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3koconxmm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pexjbfik.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ujnbjvjb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ogzbcwnl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3usrihbgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwlbbukc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3smvpvkxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skhfjxgm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3obtiheza.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hfahfixr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hzkkrrmh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yshoshut.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wnfflirs.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3plbvsbuk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ohtfixik.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hqaojwqm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3sdfoxovb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3llikmsct.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3rdxuklzi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zyamiknv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3yaoavmuh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pxqhuawr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cgmbsfgo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3pgxeuesh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3illhxttb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qquflawh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3unrimiua.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3alvuenie.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3afsgsfcf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wbukfufi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3npozakeb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3suzfkxie.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3sgxwdxll.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rwxyqyzg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3czrrcqih.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3tofihhjw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tacfsmzf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zxktctko.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rjknyzip.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hyjdogpy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qzdzzzzc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3luaeeltn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3xuazbbgy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bpmhmawt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3fvzrsmio.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3uktsbjga.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3gsvoqwsb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3pwealsdo.html


<!-- 参考信息 -->