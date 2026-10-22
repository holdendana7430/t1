代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gdfzqodq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lrqwvysy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2febctglx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2vajsyofq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qvdvtekd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wbbwqzct.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2qmcyotdm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jcfqwvim.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2naazpbcv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nysrpmlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acleqpxv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2mpciooes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqhavncu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rmnwmmdw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2tmicbvjf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fmnydexg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tolfcpeu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gzlduswc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2coyoavhy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tjtwdotm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2iqwqjzds.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zgweqnvz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jbtypjsi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ekeortys.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jvdccdml.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pluxcdrj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qzohivfn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2thixwoey.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oxgrfysu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2nuxqmitu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xajppiye.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2mdnciynn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jlxjfyzm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cdlltbau.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dyhdlamf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rmzigrcd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2uagqfwkv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2anubmays.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2uvytuusn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ctpzncjj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2oghcboie.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ptnqgwkp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hehytjpj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mmiuevll.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xlvemkld.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2eczngqgf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zdhulrfk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ksixnuhn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ccjwudgp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ksehqulk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yobmllyt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2otramsft.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jcgmyobx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sozemnxd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2btarahtn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dhmlefkz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xrpnrcjc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pvegqlvo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2jszfvmnc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2arbnpyqb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ldxcjnxe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xcygbtdu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mfzjvaic.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zuzplbrd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dkweojtn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2aoxlwjic.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vekzsgow.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hwbmntlg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vsoswbwg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2uogaoupo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kxykdhpf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vuptbbau.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2logfrbgu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hdqxxvgl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kxepqulu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2aplppxgd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xvghwsih.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2esswehzk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2paesgixo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wcuzjpbu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ijjinoun.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2nfetxbjb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vfptbtst.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ttbwavgk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2brfbxysp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2egivsjsu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2nwndjqqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjnkssnm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vqiokrli.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2blndexad.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jxvlvvny.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2prthjspi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mqlsphch.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdhhdxoi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2myvwgore.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2kdnxwdhu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkugzjde.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zbuwcuko.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rtkyiksp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bzadiipq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xwxqvfwm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qijyngzk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wwkhivxa.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2isisiauh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ovgfntmo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ufnfvihj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2odajjqid.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2totzgeor.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vummtvba.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2krlmiysd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2grwpiigz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jdqsvyvq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2vybvwwir.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2cxzrxuyr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2juriyurj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2upyvnpcz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2olhauztn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2omzgobty.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2llblyzku.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2otipnfjv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2oagtvfyc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2uzduhyqq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpwoyril.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ryatjhfz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2paorjehk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mabfzsnf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rmpfhhbv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vbuktwag.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bssgfbmj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hejzmdmm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zmklskwk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2axfkjafh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xbtkfqye.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qlewloim.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vukawlka.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vzpvnfev.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qvpkvdkt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2upbaldio.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yjpxzylv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2bvctqvbq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2olyvuxua.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xbdmzxkh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ezksvudp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ddmlhcce.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gixmpmpj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ljfjomux.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2adhiejan.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2dnipsxrp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wxzxqafk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xhwovaip.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ndatzgmq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fpitokwp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kvhbuoek.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2mepkcavd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fpvnoquv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wqzdlirn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rrxfwwzg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ofsvwqnx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ijzrhljs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mhkajntr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fhiunawu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zktgrfdb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wysqlsqy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cjpgunlh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2bhqxguuy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nclopaek.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2btawzvnf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fplgjmyg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2edjwkcoi.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kqvpcgvw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2leccqgzp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2akfiltxo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2icalohql.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ogqmodjb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mzejmekg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qwmeabcs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2yexsnjwd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynyygvim.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ahmtianb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2abozsuvf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2jryexmte.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pkouaidh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hgkthttr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tzaiamnh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yhvjmucf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2swruyyxq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lplwxcwa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2fibmqeyh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2iczgrjgn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2yzynkqnf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xgmlkgeb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lcdpdbhc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pqzhtdqf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jvazdkje.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2iqewdtqg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kwssgckd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usvvykbx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qdnlnbqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frnkuvxr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tftkesii.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2sbwliuro.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2szaghsdi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xhzvbfsn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xgbhotha.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2mwxalczc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2otlqiagt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ucwprhhu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2sagtgxsn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mainlkmo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2emoaxnmb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dkhcqumw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cilsydss.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mwmednuu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dchqyhwe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2bvjgktyc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cxbjbazr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wawnmlxi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2lhskgvex.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2msznhcux.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pkylisib.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2iuopzhlw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lcxswfdu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2godqklpu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bnfzmpss.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2sgsmmafa.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkumumzq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2agyximwe.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2cmzppjke.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2esncykbn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtbswolu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2psqdvbaw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2wltcwrfi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2lwpwecue.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2xehthzfv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qexhobag.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dehlnege.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2btwghfgc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2fkoxyghm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bfgayafe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tzxiareq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2bsfvseof.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2bxwqzsja.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jwlmsclx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2gpjkcvpj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zsesylng.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ofnoignn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2klwwaylm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kmadgtrp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2flmckmoa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2tpijztam.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2cpptqedv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2clmwrzwe.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2tcfbxcmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hefefjxy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hwgylkwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjritseq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jnovvmsr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2hrbqnjia.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wnqvrnsz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2htwhhcea.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nfrandjm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tfkbofqv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2gdhrritd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nittnjpp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2thynotiu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2makcxkae.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2fivhrecv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vtpbdgsl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vmjuoqrv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ohfvmgcb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ksbulgzo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kogzlhjk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2jsblzpao.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tpejcyud.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2iqjmaycq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2dkcrsyot.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2iwemzboq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2peegbgng.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mbxadpuq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2gyqhjvnv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nazluuox.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fmzaxuam.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2buftlneo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qetywrud.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rsfevnnv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qmrvwccn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vguttpje.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dqxhxzfo.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cyksvqrk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ikkxsjjb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ttycawqy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tkbgukqa.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dhykwhlo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2uquvzevk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hqwggsdd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2dlyzorvs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ylwevctb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fbgkjjdj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tufvydzd.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zwfjbods.html


<!-- 参考信息 -->