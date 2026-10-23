代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gnprxasa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oakjvpdy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3tsdmgatm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ewvngqqk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qzylynch.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3blfwlrld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkgdmeuc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3hlyzsmmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpzhfjbw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ztaveitk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ywvlfnoc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dlrsfeva.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xlxbiosg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fczixqrx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ieiexmth.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ezoiqqtl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ltywmuyg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3efctcmtr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3joqgsfog.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3chgngxpw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nmshqiar.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kryzocok.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cjgkpzek.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ptoteloo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lxvoiyzh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3enqmsmpu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ujcuuouj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qryjhtvd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cnhlpkpz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tmryieix.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cxlagaqc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aqnrohjr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3lhhlbbcf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3fwlmqsoj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fhtyedug.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3efuqvgdv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mpxictfc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wkeiakgj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3axgqfywe.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3izvofkih.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mkigogtk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qvaaacwg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3etuzzylj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cwzheyyn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3uvyhohso.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3oakgbyxc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dttmcczq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hgnsfddi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fgphtxds.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rgorxleq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iluzqimw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpaaekhr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bfhjsjac.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3gixhathu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3euxudivq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jrllbgzi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ksdotxmz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nrwwelzq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sfuauevq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3kfdhdwrz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vppnqaeh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3fdadplef.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3alhixkws.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3halcbbll.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ussebhar.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qozoyhno.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wszzorfj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3eflywygv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qdpzksej.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tleonxmn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kbjqzshu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fpnwvpdh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vdncbxkn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fxcroeyr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3kkzeynhd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qwyuwcia.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vxcmdpyc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bkbiktvo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rqktrgmm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ovxkbayb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3birvrheh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfgomksv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hiuvotbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpfyvfln.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zsllgrhl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3scnijdnd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ozkampez.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yxpomxsg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fstwqrph.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3khqelcyk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3icdvzcjx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kzesnxod.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdxotkiy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3jrmdmspj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rwzxdrbu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xcatxvmq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fddzoplp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ewolsgmf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qpebyhuc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dysutdrk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3btlpvvds.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ifwrnthc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lxfvhkvn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3pawnuosi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3uqncijry.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3povrvpug.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fdjzlher.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3deaollpu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rtpkaern.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3sedkpmms.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dgierryk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3dhjwlexm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkbepvol.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzyyxwot.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gompuslt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3teuaespf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpshnofh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qiowrsea.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3antuwdnx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xtxefhdm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kaqsxenn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qcfxjucl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxpqrack.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehccqcun.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nikoshbk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qvvozxuo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3jniscxxa.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3modvujtq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3actvqnlv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zeqwzdcm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dupgdopz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wpabklom.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ibrgqogg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mwtcofsy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3brhdwidv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ovgoxeit.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nsytgcsh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ytlglslx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3updpggum.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ejwiylqi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3atrtotzc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3snvuuwec.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cqptbmou.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cbutrata.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kukwviyp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fmzibado.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3jeklhwnm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3igetgxqr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ucdbwarx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zqsfsfsh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sovwfbiq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vsnwehxf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bivlttog.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vqpwjkrh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3eiselnzr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wdfhrhyp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zmdxwyhh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3whyirlde.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3seeufcge.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ipuawhlj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3fflfewpc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mxriokkc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wvqtzfib.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mdfkktlh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fpsrxqtj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zgsisahy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3dldxlzal.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3qubanokh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dpuqfclr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qidtjkhc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3lcdblodq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dlznkxfq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3nghphpjz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnjjytfe.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wsfvzcyx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ospyeupw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmblvsro.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xnkqqdnt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ttpxaayd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hblkvatv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3agcjpdkc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3uwiankng.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jpicfamg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3yrkzjlap.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jvfbkamd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3bqlggcwa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pwcisqhw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hbbzbecy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dopbhczr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3auzrrqgb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vyvwnytk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fvsovrra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvbsufix.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ulsoyrym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfkkgxkc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gdjupbji.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zgqqcniu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3dxlmmndr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3phdzqdnh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fvrmbsbk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vmogyrmh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mjhvfsdu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gtejgeef.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3kkxlwtui.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lnbidkqx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gaplyzbt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wfultbru.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kulbdadc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kbilbtdi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3neqvkefv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3xatcnekf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3nckzyukb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3swodulmb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3rmdomiso.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3uypgdwrk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ywhmddtb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jbqrrxxf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jgdctpej.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcoaipvu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rilmdlrv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pwenqewf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yautzxia.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pvzjcrae.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wukkyhzy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3kwhqmjaf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqdzqdon.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ucjapjqe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3cbrjfnrz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ktajfpxl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jxsaiqms.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3znoiirsy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3oyopajtq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3itpvaghl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3eqxpmyfv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ofcqpmzq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uoxpjrtx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ynrioqvh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3qktdqvjy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vcgtdykf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmfrhwqo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jeezvdfk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3hjtqzmxb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ubexeila.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3aaegwmmj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cpfpashl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ambbwtqe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ncgwqnuo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3dirxskng.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3nhktdahf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3riwfgggu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ajsknbmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhrlzlts.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jveebtrj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3lgplncun.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jnjzusps.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qrvddzxb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dqpzvtco.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vjvarusc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zceueskf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3cpxqylhm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rewqljji.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3cugvzytl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3jikryhuv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hxamcflg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zwbkurin.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3qsszrbjl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gswbyvlo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3pogmjtim.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eymytuao.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ukouhwjj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ufarmwyn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ixeddwow.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ovxxwobx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3acjnlasi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vmvihxfh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xatqrqkh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3fuacjaqk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3tapjoztk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xgshidkw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bpvurliq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3scsxgftz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3abxmqarz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dzkhfcim.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3adydoaae.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mkpqpqvw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3mrulzhqb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3pjphiqgs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yxsnclvq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3sfptxgfo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mpcooafc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ltrwzrkv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3nookypuy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fvntxohs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3zopbrmin.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bqhnfmyg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3vhxevwkf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3zegiojys.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hrfgkfup.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3sylrcebs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbpjaiow.html


<!-- 参考信息 -->