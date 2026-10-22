代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tlybawfr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nhvvtopj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xibcetpu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fnvbgdpu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tmlouaqr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2flxiiupt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glkqlpxt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2nkmgzagz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvbxyuyp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2alwjiztz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oqfdtbpy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zcpurxrx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yypxjnzu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2saurvdqt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ttbdutgx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fnozsgoh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2snrkzmff.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2stvtnmmd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mtpkfkdw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zgdmuwbh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qrzugqrr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xahezewq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2eormjinp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uenijvrl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wegpaznp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vqmndaok.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2drmdgmtu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2eelufmju.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2loqhstxm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2rfyouwhn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yvdswlyt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tzoisbkr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zqvxkzfb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2rqwgumdc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2myeschms.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lhtkrnwx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ydvxvamh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qaycpdrr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2abbtreyo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zudzsnja.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2stlmzktd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pqyncamg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lwdzszlq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2uxyikddj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2oxdoynad.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ddnxnbhp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvetlrff.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rmnjzqml.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuyokdxh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sageedkr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwpukrlf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qmdykycr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2uxohxsyl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ysnqhpny.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2wqkayvgx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2itqeadbq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2okvfugxu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2osxhbuhs.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rtexxugr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xjrrbjlx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ousfdqkk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kjlmlqua.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jyidampi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2zxtpmosv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nutrjtzt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2rdhjkfyh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hkiqovze.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uigdysdy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kyrojtfi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2trmejapq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ehwonfah.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2nlhwgkse.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uybhmgkd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2vibmdbiu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2paqvwrvc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cencihrj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2djkwzdvr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xwdzgkbm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2voixpkdt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ookzjhox.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qzpyrwab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byhbarvx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xxtmzkri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzudfifo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2prkytjqm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2navvgrxs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ogytjovd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pgtbnoyt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2myvayvmy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2khsqdukf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2usoaeyrl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ozhxgrgk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cunrmxxu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nzdrqryu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qaastpxc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nyoadiuw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pmpijfvd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xqakbqnh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hxyeblwt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tzksyspm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cknwfwpd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2yoyothze.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zmptlbwm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mvvmjffn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vlbbwhkz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gmujsske.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2haqebtna.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mfnyvtqg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ektlgmuw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uhagggyd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2eajymenu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kafdbkfl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2siuphtfx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hsbokyro.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2joahlxfc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fszhxjcz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xyhxyiro.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2oyppyxsx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hcoyncnt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nlayzexq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2chgvngtx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mkjmzdrb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2gnrdywwz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dayhkolq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvvhfszh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2jpxmqkua.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cfrkembb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vdqgzfjy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ovgixnyg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ldelhket.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2shsbpfxo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tugzpsjd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2idwizoqp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sfpeotrv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2eyavtdyx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2prkpmrak.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fbomwuce.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uoytifas.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ftsxchpc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2oozjqvhh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2hngqtzie.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2uuzyccnn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2bslmfkmg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ntjmavmr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2geuflmpr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nseobdgy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2oydimmmn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kpsdgptp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2waoajnfw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2gqndnhmi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jsckxqvo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lifbsnon.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ulewyxau.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jkmzimea.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rjqlyjpy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fnrpssnj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2eulctksl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sjjtyzqq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mlnlcylg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ewklvtfc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2vjzsrswq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2swcgpido.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2xmuyfeig.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hspaacoq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lqabspit.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lyeiwifm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2mhevffuj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ybhwglzr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2rtsvfhro.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vscftruw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2pcstuomi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ewfyltyi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2bbqghcno.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kieagzsv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qfbnhjwd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2reotvwfv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggwrkmue.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wkpijvdw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qecghjms.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tojmeggx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2drhzwcon.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wxrxxozb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2irnprmln.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jieftady.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2pgxzvnha.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ussfiffo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mfahwbco.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zgsrapyw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uvqcxifn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jqqmmekn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jiamkncy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tmcgpuak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owtupqsr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2cfrsctgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuuhwuao.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tiidyuho.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jgbdtnha.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xflkoiqj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hzdgbxnk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gpxgdkcw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2klrhgycs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2oceibmgc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rfrtmqxs.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2maioduvg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yiklbkuo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dhsypdns.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2elbhexnl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2aipnuhbm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mridbqal.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lhqzpvon.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qruzodwr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2bvohnhxq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2axznjnsj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ljpyeugd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2nirootne.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2psplzzru.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dcrwgpyy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gcripfqo.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2eahkpruh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2huaihqlu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jmzqxonl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzqdyyoe.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vuuwezcd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2vmcqckkg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jffxwtht.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kkfviwwv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rcsodufe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2posygmlx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ptyxqvka.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ftxfmsbs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2szkomvqe.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dobjyfvp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ciilvaaa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2oxckswpr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gwnhwiff.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ogyrdijy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ckqorggo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2tgicoqnc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jkrfliie.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2scfxcpnz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2xkbnjoic.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2mmowafzl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2agltfpgt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lgcglmrm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2abzunqzl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fiwkftqq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2olufxvip.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2cgoltmgf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2snjickuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnmycsyq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2frxbnboe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvuazfax.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kbitkmde.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2prmdeqqu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vfkovfxj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ipickdoc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rtdfgzxi.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jwlewruo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2gzxcggdn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2psvqiqqp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gnyhottb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2vqhyfbhs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2nogdvwmd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ooeftuxf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2pnornikm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2tjhiceiv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yzrsphgl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2wotrjshx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2foqoulhm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jnbjqwac.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mzywigff.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vbhhrpde.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hkceqvmw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vwrahnqn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kptrncfm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dysbssfj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rxpnhlnm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2oewhbghh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2eqtixwti.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2gzubtpej.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fsyokagy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gbgfnbqy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lmurwkxp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bsjwbebi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2whqcyndi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2vtdvwmbj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ipnwyoif.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dzpxrfnp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2iwgnlpte.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wmjngpbk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2wmnhyzol.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qooupvmq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zwhmbiha.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mpgujrbw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rxwqjaft.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ebwfimzb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2yfmfospj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rvjzucdn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2wmpdebth.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bpqdkwbk.html


<!-- 参考信息 -->