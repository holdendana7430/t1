代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uhjdtudd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vzsgnfyn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2kgyhmsqo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2soxdcant.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cqwswqiz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2sopsnzag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irtvzutc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2etggujcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugvzlwqu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gdlcplvi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2bchqngzm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qmkjnvax.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2twhlpaqr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cipfjwsd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jfrrkqdk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fbsbtfnj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2nmduxqpu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qypxdryj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yvmsbgty.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xzjlwsmh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ksfjrudu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zysgubox.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ixsbrkiq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vdysknts.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qbuheisw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2knkzsyqm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dusanduu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2dgjjkfhy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2lqitzyos.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jgkudoct.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kvorahrs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qkevawwq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2jlplynpi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pdnhvxyt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2bcphnukp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jsrhgzxx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2thpkcaeh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2urmjnljd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ybzhyoks.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2flsynyks.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2swwxychx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2uhtqzanf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vvkodntq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kxscqiiz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qmpjhfym.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zinrvtjb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2litxcdio.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mpaxhrmq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2peyidakm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uxrjjbrp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tqmaglez.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmcytsyk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2hfczjaqq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wosjdtwi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2evqwyufv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2anwezpig.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2pflzgwox.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2iadgywkv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2znhqsvwa.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2whitjbot.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2rnzdarmn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2nmiemsuf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jifchrsy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2cxqgsrpt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lxhgtxdy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2nqrurhrk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jcapjjvc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mitqlzpl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2khucahqf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zhijctvl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2dyqfftkm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2plknuctg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2aqrssere.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2odtwjzzr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rrlblgfu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gjhudcfv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mcngywyp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2wtkrpzev.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2yussrenh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xpcwqsdi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2eonojnoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2negwngdt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2islfelll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsknlmuf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ersmgamz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kdbkbceg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aiofddyp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rbwftvxq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2syhiutwz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qidygyxw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tcbykzov.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2sngdpifj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dkvkvvnc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qrggkaix.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2royoxwod.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2uyvbmwwm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yvvtfslw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2neivyodr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uvtzxgmf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wxoplpdd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wotubvay.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bmdtunky.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2znxkcbex.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vseezeyy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2pryvqtur.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wqhdaiil.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ambjszzt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gezdpgug.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2mvjarihl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2bbxjgepu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ifqfsigt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2rpkkqrix.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jknnegjo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tozvtwfe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fuybepxo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2juatcype.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qbqowpbr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2shafjzya.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xnwmksky.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rbvmtvkj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2pxsqbhzr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zezzwetu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2cjxjxzxv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgibqxpn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2enotmaul.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qkkxcfop.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2qsodzcmy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2kcnxfirn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsukrhiq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dnkfkuuf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2loqdreln.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2swlpbavt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eqrovipz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rqdasosw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2lkwnaqmh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2sracjgxs.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2crjbirqf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fsjslmfi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2gxbnbuon.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mhfjorpo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2vdzlqytv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2nljgptqu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qigcxdbw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2qfsjuwzh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ifwhfeow.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2hpedtmba.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2arsomyzo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wegpfhdl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2frmeyvcw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zwbipmtt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xcwdsbdt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ockhqpdp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sdxwzjos.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vzezvpzp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hijbrate.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pktwxtvv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2btwlopci.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bgkiwszg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sjliyheo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wcpxiytn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tcimkkcc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dnxhcxeb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hlylywon.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tbbugufs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nsuniqha.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2zlmdmyva.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2afuczlti.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihsohmzk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wsilwkbk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vtalkbmd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2kqythzdw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2nhtmkgqf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qsyvfcmw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ruaqcowr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oxxyimxa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2fpvyxljg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2grtbnbub.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gakvdwff.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lwpkbekk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qtshphef.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bvlylmql.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qayersly.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2finqsxap.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qpijzxlg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ukrhmahh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vvybxlyw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2oddwvxiy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cpxcnelj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2lxhjahpa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nspshdcm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2yzzeclum.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2okgpxpsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwrudlka.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ubtoeoya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqkwimal.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2utjlxeev.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2utukyqiu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2fynggyek.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2djouvvin.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2shlytnqq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2luzrnjev.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2lttqypuo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2kvgcmxji.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ojylflgv.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rdmboxbu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vezlpnls.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2lybafzpq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zegeddqu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ovmkgida.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lonadwrf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2giaheecw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ehokcnpd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ppmjtecc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ckgbjezd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zuzjoqnb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qxmujyng.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mftzddcr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vejcymok.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxqjqmee.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2aivtxmxd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jrytyyze.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2aesnzgvx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tmxodwhh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kkjxjzec.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2fyjwbrfw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvhmnbog.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjeippsl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2mzmdoley.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2mqnpnkju.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2wiundmgz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bllrddyd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2wombvrfa.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2gpohyrse.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2hifksehg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zepohbkv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hgtwfluf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2enjlyqcy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2uqsfqzso.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2esxmitdz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2nmcudomv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ebtkufla.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2idhwocgv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2obkijmdv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jicmsgfn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nnrjtzzt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zskslogc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2tmkmsuqb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2vgrjgqyt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jqxdtoig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvlaxizb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbyliufo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ctxjwzvl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bucgwdvh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2bwwwyaec.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xnaiunin.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hdxaavfo.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kccujqba.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ydbafvuu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ztlgtegn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2eoqdqtgs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2axcaohix.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2esttjdjq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2hvhhlqmj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xsyvnwbc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lqrkhfqr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2isjbbudk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zdpkslwt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2yohtauho.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2jxwznkkp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2qypwcdbm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mtfqaosm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2dwnrhdrc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vbshoxcb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zgmzrtnq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pfgexalg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2nyavyoia.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ftcpimvo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2frceqvja.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2elxogkoe.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2tuxrjddd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2duvijcrh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vblhxgti.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pzvfatmg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ryzzcnsu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bxxcnkhi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lliljzxe.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hgkqpcrt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gnqchmdr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kccdrwje.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2nnwimvzf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2bxhcxyld.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ljgheupo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2froraymt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jqnlvktu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mmcqripa.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ncpupkin.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kirkcvzb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2qemhtjyk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jxekpvlv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wucabgic.html


<!-- 参考信息 -->