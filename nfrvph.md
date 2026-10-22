代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vyqpjxjz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xjjogbff.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2aebajdsq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ymnussbo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kofesmvd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bibehwpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtdeyyil.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kxgjnfma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrnjrnnu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cmbvyxll.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hiwuqhzf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2rfrlublp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkderrqb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xptgrgky.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2uucmjouf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jazdrlwa.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jopomkrk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ahlpqhcu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tysgnvjq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sccoqdkm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gzgpcscl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ymgeclel.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2slkudwnm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2csiuyfyd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fmvmlvaa.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2njbsnzix.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2evpttdkx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2mvvtyrjq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tpjpauwe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gtgfsdyb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vwhjiupr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kkfrdeai.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2oanmqvau.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2bjtqirqw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ohbalrkc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2upxgjetz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ihuzxdmz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2niehuinz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2oalhnsot.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cejnnmak.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2unpmxwom.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dwskkvfm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2shmuwfoh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2psalllpa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lksqfhit.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zeaacfjn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pjtxcbtm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mrvtadxc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rysgujdo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2octsqjzi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iryieiof.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zkgwfbjp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cboskxmo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dajklgpz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2luswoyts.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ksrdlgwx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2peuuixlc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ujqoxwry.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sguxhoqp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ikkdamhc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2dbvrphgp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2gibhdwsd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fcmzdxfv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tzofdfio.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ftbvrnil.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2cfjfvgpc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tabhlbxi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wrzmgnnh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cwottqkv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2pqtghhnx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2bawlmyjr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2raprkfus.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2njhsoklj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2tzbqyfov.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2jimkwbgn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dhqlubjv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2swjmwwou.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2kvuyvsni.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2xmdcxdaw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zfzphpov.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2akisnsis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjchimki.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2hxpjvfvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzqvaqri.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2woklwvgy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2didagazx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dgargxzy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2irqybooc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2skoutsot.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bawzekwj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkgpgrif.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2arsmivoh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2guxbnovm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2txaueaox.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wbfwfenr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ldjvncun.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xrcckwmu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2eekchgna.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2efnajjnl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kmfworry.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vxgdzoar.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2eppxfbxq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2iovnzzwh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ujtudfge.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2osqtddum.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wgwcmdqr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dzyngnqa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2kllsjhdw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gupnurdi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qoqhaokh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2milivygx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2lcshfznx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dsvuiriz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmgxvjhz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gzgxbkgz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2moohxqtp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpnwlyzv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2azceofyl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2krcounwz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lhpcmgfe.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2gcvzwkwm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2icmxrrlu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cconrblp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2eearjszi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnbkooyh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yxjtqqoc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ecmksxvy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vpujwqjb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2iefljpzq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2methmzgf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2asooiimv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nvqlhwvj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xjjinuxr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nqgdizuq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jmdypjvq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2hsypffzd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kvtwtqzb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cetqwddy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2xgrbldzr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2lvivxltf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jovrznzh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hykqhbjq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qifoqdsx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2pbhfgmcv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gjcnvrce.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2grtalcbr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tqgfkppe.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2riwyvjcg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pfcrzncp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pfvzqscu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hcgetlpb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xtzuofap.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vloyvcth.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mawahbec.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ozigbzog.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zfuhedwk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cifujqxi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ugjiczlv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dsnksxoj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jrsnrstg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ckjdwych.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ckvkcqsi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gkvpizmj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rmqtdvfe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2gltsbkcc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ydqokzte.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2agxolcpy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnwetrfk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dlkwoaxk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2aenjpxxf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqibpuwf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2nvisvoov.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ljaxfvpr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqgljuku.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2tlrebcyn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2zyuygoxb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjovufii.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2whrcvopi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ezicnfwn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2acgneqmr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2urcsffex.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wxfqfxjo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ywgkbnkv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2iybvktxc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qbcclsql.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2taibrmoy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lzqrfmqc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bduoxuuo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2euwkpfsh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ueviolqf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gqqvfbwe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2aexwxxny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eafgsaip.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2lohfvows.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqiyxtun.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2kacemdxa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ltmnvtav.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2horkyuyv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ewpqmfyy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wspyzhdb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2uvtyhokd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2qjrvqpcq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2kngisxvz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xgayvttg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cyjnduue.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dovcordc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dcuqmxbi.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2elexyrbe.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tcgwriwr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iytbjbzp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2dnepjgsr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dbvqgacw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vgvdbvos.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dnrudvjk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2nrcvnint.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2aatppbrt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dgiseogi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2akvztkba.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubvjarut.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ffyrdrzj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2shivbymf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2umnesfrc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2joffkqyx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2sizjrlci.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zojfhxwh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lequiivp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqjgvtpb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ttvljhhz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2aiyupgbw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2jksxnbfo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cjgqmfeq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2eafwebfb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kiakeyss.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2azngvear.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fojhqjcf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rdpjzggg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qtgcrbme.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2prvoigzr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vqgyxkzu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2lchefupr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zqkgpssx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2dekaoqim.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2dqhwbknw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2stjlhnqh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jtxdihiw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tlgdejml.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2pxshmzef.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2uhjuatat.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2nlapltit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkponwdb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2itckideu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzttojbt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kuqiujld.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pozvqmhq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dhefzrbs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xcfzgqts.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gxejuqkb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gyuqddnv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nvbzdvve.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2iurlwyzt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fgzzduzh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2fkxmmihj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2otynemis.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ktllvinu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xbiyyyrz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zoqxvlzr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rvaueepq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rwiyqiag.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2iddmpmya.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bbupeswz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2tmplsezp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jibajdgh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tpfrgaso.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nktnvszh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kerlpgbk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pqicmrmy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2onbvzajq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2qcgqjsip.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ajrurqyl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zmndibot.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ckyaejtf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zxmdsyvo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lafpuxkm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2klbdixtz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jxzjpfui.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2vmcxmdmy.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2pynqkwtd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2asinaltz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mbxojmnr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vckcnmlu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xpzawvph.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2psblhyhi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zgwtysax.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2alvcslmd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zvbrnbwl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2yfvogiud.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2chcscsmx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2akohetxx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2vetnbyda.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgndmkyz.html


<!-- 参考信息 -->