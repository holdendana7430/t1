代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3anpvmuio.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wcyqkoeo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pvvwqviu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3evcbrwhn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wdncqorm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ihizklsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxzmndre.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3iqvqrtmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cotffxhu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wobdiavf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pyexijyj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3bjapkoeu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3isvbymmb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3igfwvujr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vimuyjnr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hbfxhvem.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zuqgukrq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nkhiozxp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3czpcsxqn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ltfziqoy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3srjllhek.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ymwygkbo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xjhvzpas.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oqgpjeda.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qilxdztd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vwuodpld.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ltrixrdf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3akmysypl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3umvjhbre.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3bfbuxiws.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3eeojnunz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3womedyib.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ppmixgox.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qoyxtorj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3zrzoxuwj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qpjhbzua.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3izbvbfir.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3edmeoxme.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wihagfkl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gxttbdbl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eixuinnp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3slspknvq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3iesizcot.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zyjasgag.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3izmdmufl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qvnqmeke.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxfviqqi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gpqfnxxq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3skvthnkp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkqmnarx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hbnaislo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lpxzriwg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3njptftwj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ihlonfmv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qiqofjsx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ookennmj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3iqxtsbje.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hakeeeod.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3eigszygf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3krdeuvwp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3tcuqpvyr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3xxmxnzob.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3iwzprubh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3otfzhyfe.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3laqtewux.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ffjmojmc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xmsivrpi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3sxzsmltt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3rngkicrr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rhjopell.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jvnomgho.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3sovnuoho.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3bvguwbig.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3drzxhron.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wtxdnabw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wliihiez.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rsrmfpah.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ofhimlks.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wwwoyjdb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rlchpves.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ywvupdze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycibuhrh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ibocebit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hynymust.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3axowswwz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwsdwwwi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3siyskcrd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uaupyqia.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yeixgbpr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tloenrjz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3prvkaqwy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3uuzeiqsc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsddwocd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lpmsuiim.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gsrqgqyn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bvtyeslm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mbiawkgx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3werwravx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tnhnjymz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3beldknvi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rvgfjgxr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zcfipajq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gsykuxpr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3iqwrpkyi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tcgyyhvt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mudnaeei.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ujwqjdoz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3hofzfigm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xfvcweec.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ildbrylk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3qjcioqfi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3myvxzmqk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ahgtybat.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jwjybigy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mrfyzvuq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rhslyijg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3oouuymdm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hyzcetlp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3heuobnue.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dfxgbnym.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rzwjxwxh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fjbysjio.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kbzrfyvr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wrfmjfkp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbqlbfye.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gthlhdoa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fgmebtld.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qfottyne.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3flsrzcnj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lkpgxgoc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wtutnwfw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hoswlqpl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bvluofko.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oyspqrqm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dlqaqqnd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3arrcxmeq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ujjtebxc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ncmvtatl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jgclsnfo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ztnxgmml.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3iflsxhlj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kntxrehv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tcgbmsvl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3uqlalgmu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3renoftts.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3wwnrblig.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xnzjrvfo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3nkmkbrlf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ctyuonvk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xrjkcepp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iovrczap.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pkdsysqw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3woezrepz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lxzqfvaa.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zyjqupqw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wodrdbkt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3aerauysk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3xxipxayy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3avrbrjtr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tjnstgbb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ofpnqohh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jvnmfjry.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fuizjoal.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xzwazzsd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3whmsvgxe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ptidptog.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3gkidbcdf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3glfrisnj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qlalcojc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3goowooeh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qcaiqxqn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tlrxywpk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3attgrlld.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sseuymyr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kwnszzvi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xpgwrawa.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dgugnyex.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xtrtnucr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xkrnfoeh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ewhaugzn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wbyivpxn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dokmbzlt.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dlqvdfbu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3hswhnich.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3yiwecgmy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kdbiktzo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xcrplatr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qcthhisk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3roowmthh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3iobmevzs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tdzvdens.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rspbyyaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pngqjwke.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zxdyjtsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3culckakd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3pdfmehjo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zmwvwomd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gtfoutul.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ujnftwgg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3arvlwuct.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ujfaujvo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3csvzxyrq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3cnkdvnwi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ebsvljem.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hbfotvls.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3yfksrcqk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3nuigrfug.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3adlzlaqp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3apbnmolq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3yhqnezoq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3tumjxssd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3uhqrfzqs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qamhypbx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bgvyquvk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3wcwxcgxi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3fkvuvwgc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fmxtjdie.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ietbmqam.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zawkhtgy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3oztmxcms.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3swiauora.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpxjdrix.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3umutxdci.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3movhcrer.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ovqbooin.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3arylhmln.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcvorxsh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3wgrofyix.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3dhxtyoho.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ogaiduji.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3yzubftbk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3evvfejkd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3idfuxbda.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3buopqhdk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mlujntsc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3srkqhrwo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3hhnpaxwn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ehjstfan.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kzotavkn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vlyagiuh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3czcnrdic.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3hbzcjqnx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3yvxnxxpz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zofvzwcy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wgbrfmbv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3voriokbh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3blgwwfju.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3twlehnzo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3fpblnyex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efvxyybz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zaqzsxdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukajospa.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zeoitlzh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3gqbqkgbe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3qwfmddzp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xtdtyler.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ojrjkrig.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3koaclylc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uvnnjqem.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3irmkngwv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jeuwioih.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3mjgzzlfq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3illlrnkk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nnbhbrfc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3eofhjiap.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pakgmbne.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cncongib.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qghadwzc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nkkaeggn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rzhmyinb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jtnmcjbz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3njdyellr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3mqkhwieq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mysrpcie.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tfaudesx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uaxzqavu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3kblfiyjv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ljkdwddg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xzugsuvs.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ltaxlcuq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ydgtqhxf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wzqfbgjs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gqacvsph.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3sjnuxkli.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3azmvafgw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3aywhntjg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3lzgrwjkz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3iowtgzyi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dxkbeopr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xsuzjqyo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fqqxevlo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ehrxdvrr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lhduheag.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3pgynhsau.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bdloocvn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3zlhgeuot.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3tvnvaeit.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ppbfwyfg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rbtzzfwo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rafemylp.html


<!-- 参考信息 -->