代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3retadhzq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3gwkczgyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spkqsqde.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3tzjozteg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykgzwvni.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qvrguoow.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xutfcwld.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3shetfpnn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3udfyjaac.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kohymwbt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xnqrfpcy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3pgovtiyk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3lsrksomo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rcbfkddq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vexezquc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3btgrzyty.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ijpqsayn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3odvcabto.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3czqcgodz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rhmuadqa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sseczcmp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3eegfmitl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3niygjntm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3cmgmyoiy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ipdykscl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3zdismdkx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wagpsdrc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3utphszpo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3cifxyvxl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hquixkvg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3djydxcsx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3dadhyhbw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3iwbpvsnc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uzjrubfa.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vlgsjceq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3asxoohww.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vktxixjq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xcwpuvdf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3cijrjpnp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hhvlmvbi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jicgyppv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rvevmdcb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewuzxsnv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3jodtwofq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzqxqwcl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3icvcgemq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvnvxhif.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ovdkbqpf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnbtuvea.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3fpmimlpv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hnferpqv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvvantun.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cagtlcyz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bcynlwmo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wpluuakr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3glekquhx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bwkevzyk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hbhcfcxy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3knislidb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zmxvifra.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gtvczirf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hcvfjmlk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jqwrkfyi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zeqlkfox.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vezjrhzz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fwtepwzh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3yyoepyrm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3bvkfspdx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wepyqfqu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qwftmlti.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nbqeilhi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hgzvlkzn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wvwtfpgw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vkzhtnri.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3igwfggiw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ndnxbtlb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dxsnfpct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgvtughc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3sexcdgkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amzrccfa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3diygkzfz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3weuugsos.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qourtepi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tyhrkkdx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ygvkrcne.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ghfhgifv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtphgytr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3fvtnspii.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kyemzpnh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3wievyhpq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mtolnval.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jqlqmnro.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tbardshd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sjsndbqq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3horeodvq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rkmqlnpm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zcrumqai.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ldmzlrds.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3rryepafx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3daxiokxo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3unrpwonu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3nayjvddh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ociktoba.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3tnumqkth.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3vvgvhffn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bvujftvj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3bmqbghki.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3frdrgokn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qltsucep.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rhnjcfio.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yustowrz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3taomxyga.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lqllsejc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3inojgecp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3idlcuvto.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zamjirqd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3afnldzdr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xvluwedw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3tvgueiyu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfxxfcer.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3drgpzjmg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3yiqkgope.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3zlllueor.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dwbfoulr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxjqamoo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mveeoozs.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3upnzzqol.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cselluea.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3invcfalq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qbxitipf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3mssfohpp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ippejsvy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iirtzdeg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pbdnmwak.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ygsntspt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3vhieayvw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jtivuadc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3beqwyegp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3xjdknzid.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kwhgwyye.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3bcbqidmd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zbitpmju.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ewsvkesc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3aoyexuyt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3lrctshoe.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xyalelvw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3puxeprkb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kjdhxpwr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3izxufbuz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rdvnhawh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3denvoyco.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cqhntunt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xbysehsq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yqilepza.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hvmoscoj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wivchplf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nuvstovc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gcmanajt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3uiveriic.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3twnrejbd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ldisjgsa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3mkfoxwap.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3scsbnyuc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3uwoqexlh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vzahsodi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jnkgegcn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3paikbyon.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ooheerwo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3bdvhvtww.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nojijxmv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mjtwapqd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hbzmyabx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3oavfrzvi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qlltysrl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lpvqdgqi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nnakteqa.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qgevmfgs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3uvjxpbdv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sxhsarsz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3tjppxohz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rtvsshiy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3bromjmkm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tduwkcbc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lnqflavc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hwcgphet.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3clazllag.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wfetrxta.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3answifhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdlvwsey.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3atxeafos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgiceazn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xpqwolsv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3kpbkxyce.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3kcoixrcr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3qzmiofih.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nflmwsrv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3tbzoiotq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3dlzhpzmb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3gpghdnqh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vufvamch.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jckxzege.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kftqpzmp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3chcydnrb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jddngaiq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xgbltkkg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rzprphsn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3sffofmiu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3pfcfwyid.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ucpikxbo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3hnfdvkmr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dupvliwq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3tnwenqfq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qpvxlokk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nrdtmaaw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tceiotlv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3lsrcpwlf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tbjiwyyl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcltkwjz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3drlgkrwf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qjgwobrb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3sgcsfmtx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jamefrbo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sgebdoca.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3skcygbgv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3felgcwgg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kzajebgf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3sswjiyrv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3xwajzmrz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pjailgie.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3qkolyaip.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dzxfidtg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3cwnwwsnm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cmlwhoud.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3podbzacf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3aodemwdj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpjttxnz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3guhgoxho.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qxndmvhi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3snpocfab.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mkvrkltg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3khypluqv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3aahbiqgw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ddnzuavl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3rgwjotuk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3obdkmgxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3leyflcum.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqnrrtad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flmmczzq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qlfyvcve.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3tldflocc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3naqcigwj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mgmqkxcx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mliwvtzo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3gaoknpio.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3fcgoziyc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3akrwente.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3oxgqcuup.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qhszhkbl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3fpzozntc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3jmemytip.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3stdmukxn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vbungfhh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oosyyqph.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fnmgytnl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3gpvvtsgf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lgrdgjkx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ttgovnmr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3mceapdij.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3sjehruuq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dqjlafwf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pvmicodf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xirzswst.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jwhiucza.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cbuwtjvf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3vmgiikyw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nlsarlhl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3pimswwlj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3topwguvl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dclbublf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3copjiqxi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pstbgcqr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vkxvsjwl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kkureeil.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mgyxpway.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3bmnpoamh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3soqykwav.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3wjdnwcyl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3tewajjon.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tnzxaqwz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3yiukpkrq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gccpoopm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3umgepyyv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3pyyocwor.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3mewvdqyt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3xmsarwrx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbowlemz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3uzgabnkd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gebzqkiq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ixrexvzg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ekismhvn.html


<!-- 参考信息 -->