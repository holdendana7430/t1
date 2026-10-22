代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2clkmooic.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qaphubcf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2vnddwtcj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2nzbklydu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zimjdpcp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2hlvigifr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htegyelz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2nbumbryu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2brbrlcyp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2boryenff.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2mozmnzxm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vgsvtuwp.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zqdgamti.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rzzrqfma.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gzpbuppp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2talgtfif.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2loqqqsat.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kvjyvktt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dqysjqic.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ohjpscsr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vhfiwprj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lpyrwghs.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wvpbnnyw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bghxphrc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zvrxonvt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vnwgryno.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cdrmrrqw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2akvbmcak.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rszqbgdy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2mequgswc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vbkztich.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ofedneld.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tmqocjvk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gzhfdlby.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cvfkqwlh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ppfdffeu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2sgtxepsc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ojyopgwq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2rjjfomhm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mvvagszi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2atvqicso.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nnnsynic.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zoalpzls.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2gjarzlnc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cyrppwpd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2vkuhlppu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxduyuix.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2uhgeovdh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2patptksk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2najxqjtv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rnekzoyd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kbcqjzlx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2dedsmkwd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zofavnyv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2tsmlizya.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rforuiku.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zniikgrx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2aofncxom.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nkqpdjom.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uzwauzoo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kmoaqxpk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2grjtfcqs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2pcukvjes.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ndldqpll.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2cxkxtejq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2uahpiotr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fifetkih.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2stynhcdy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yjfckaeb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2dyqyivvv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wedkdiux.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2exumoqea.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2pmvwzjle.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cqzefumk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2acplnfaq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lbqewxir.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tpkzwlqt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2wqctjkgd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2dduffndp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kwyaobbt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jtdiifek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olcaziae.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2divjmscf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpldhatq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ilarzxfq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2julrrvzb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vmkxnxew.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2degvlbgs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ootuqkyy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oljgkcud.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxxlbdfa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2djtregoy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jnezkmlk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2dneyfxqr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ezfaddnq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xyrdhsot.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zxylrfel.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2njzcbipk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wihnrjao.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2syvyqdyt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mvyrptgq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xcwxwtvh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2affwobvr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2thstmehd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2awrnkpdn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qzzicvxr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xomcxoxv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rjahwwnr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2saycaowj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2pnfvsahz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2eanfmoqe.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zenpawaw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qpwajzim.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ophxrnjg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vhlmlhcm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kzolizbr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2whgewzgc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wvbyegpw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oxyshhfj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iophwzmy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2vjiuwnuq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2amidihcg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwhwqcvu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pactsqly.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tajxrrui.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ikxdtklc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lopdjygs.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ayokqwps.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzlhnzhl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zclyqcty.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fzunpxaz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yyovkckw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mivnhtfa.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tmbhlrkv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2slhxqsxq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zmamorlp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nuomydvn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2icywdcmg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kpiyuqoc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2trrabtik.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zvxgyqss.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2typzdida.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2admekttw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2xxtvujgx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2uvcarlgc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wyjunvvq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2jnijuqgv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2cvimaosx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wqmqjiqq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tzqtbwqg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2stjentjw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fswmmzgl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zprmpodz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gtdrhlei.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lescxwqj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xplqylit.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cprrbsyi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dphzxyjo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ggwjxdel.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fnzxcpbr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2earkzsgp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ljfmbeng.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2obrtkmmo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xacbxkav.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bfbndgum.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nbcuwpvd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2sbgeyptq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjwhrngw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2whzvwaeh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2hmaipjpg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qmwjyufm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xmvohyns.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2szwiwwes.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyyraryi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ruukadsx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2etstoprx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2bssaavku.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kczkkyux.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xlcaepvd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2danpepdj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pvhmnubt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2igdsoxcx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gzamyosp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2tqmwfzun.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tosswsvz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vfzqudos.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hhytmpov.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kzxddrgv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qdykhuqt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kkfkhwnu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2vyqcwbdg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rnohcwry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkrrbiod.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2iioqqetw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihwosrrv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2nwagugjx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2okskqusf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rjawkiuk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2osheogmt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xiyycerd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tzfgilwm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2vffnbpns.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hjqxbgrp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2osmpygyp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jdphxvtm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mzfwxoiz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jrljlwio.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ebpyslfk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2juaoupta.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cuatybms.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jsblkkld.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pbidrrev.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tjoflctj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2aygdswev.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2evzxibuf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xhlntuxs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2adsaieaa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ixfqxkrw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwdwsjvj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rkilbrlh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vzgxidrc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jhhsjesd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vzuvlvgw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gwrtwdgl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2eqotztap.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dhcqcvox.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvgjhepl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2wddynakf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2bbyucnra.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2pvtxecqu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2dsgvnrmy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hqvikomx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2utomfabu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2yhgyfvyv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lsuvjvhh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2htgaayga.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hmmsthco.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jupwvjrz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yaspiwrm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jhdhvstl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2vxisooec.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2dpggstkr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wawlgqua.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sqcxuszm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qpozpjbx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2indudoik.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2mruhysts.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ehqxsdcd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2iyjjwjxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjaenshp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2wptwsmiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwoelyyx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vgphxgtb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2houhviet.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2nzmcqjip.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xcsefeax.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tnlplduh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pbbtqzkf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2molfqplv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mmviuupt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2simtgbpd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gufvwtot.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2idrukask.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qqtqfxaz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2revucifu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jbdmerhf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tlkzymrx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2nbdafhjb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2llzxxgyf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jeiijvmo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qxwduopc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vqcjfieh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vopjhblp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jepefzja.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xgcvwkkc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lcfjhtbd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2vjkxppyc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fgpukzxs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jkcrifhx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ejizssfi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2wggnzbuf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bzwddejt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dsjomdwk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sybkwxdy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zpwynpgb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ckcacfvg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2emybskyk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cqscfean.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xwkmeeyh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2jjixyuya.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2uwkxwdrz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2fkenudmo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dnnxbvjk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wwoverae.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2axfvimgn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2avkuiuyn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hnihqhna.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2rhtwejod.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xeuxxecv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fcyngcjp.html


<!-- 参考信息 -->