代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bdxmadwb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kxzeizao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fggdmwlb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qjcsbabu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhcwokwq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rwpvilld.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bqlccxdl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3cfigvnek.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvvqdyxu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ghdesiei.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dpvxneqj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3sngstiuk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lenawcyj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zpesgwfm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qvafotvc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3obhbhmse.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jikptjqh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3eceitsil.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3waxymxcp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sysjdttm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ouqmorqm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3wfpukfof.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3omabpugn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bjkondgb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fsrztxev.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3wtmhilip.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kqjiquly.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ieptylbi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dqfdtzda.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3mntdwaye.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3rcnyzicd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fzsqptin.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3btdmqouj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vqeipcli.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ybkkynql.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vpfpfgcr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hnlulyie.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wekuzimx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3anxqqexq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gvfydxyv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3iuehpygo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pzjaufsk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gslnffer.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ldzgzeop.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wbsggcqp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cymvpbgl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzmjqznc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3swkfasyx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3yfatfqzw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3inrjszwg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rubrbkqw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zgmegvob.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gdcvmnjl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fadrizqj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yrswgxxg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jmwwckuv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3wpedywsn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3akoetnau.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ufqirwou.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kgxovaec.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nxmhclju.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3iufxxozo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xejjyrqt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3oxwxbavl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pfydxkoh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nbnuwyvw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3uevvjydg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fziubhqr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3okutxpvk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3pmblshgi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rbxmfzuo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qhzrawvz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hbnzkern.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3aqbybujq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3szmcsvuh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gmebnfuz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3bsepjbhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vykkploy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qflbkdyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cebsvyaf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3zwqqvegf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mvekfcqi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aetdqgsq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hjeeqoap.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3viahcutr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbuasinu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3loweymhy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3uqlviqer.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iialgtyu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3etbfoiox.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3taxcjgrf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dqxudllv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3urvkdwxr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3duxckfxc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3metandba.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fvjafixg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dzjhmqmh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3chiayhqp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vvwhfmvk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tymuclva.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vcryomzw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ljolhjra.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wmfbpupw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ktibeexq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3urntbqrl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3yyxpvjcp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vxiiohvk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dhgkoqmv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3euwxgyxe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tjooifyt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zcoqqgfl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jqpdgjae.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3shnjekmu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dvlffgvs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihwrsbgz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vtsrsoqb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nbrcxplu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xqxqrehc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yurcnrve.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3agmzzfnj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tioffuuk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xnjopeaw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mhstttva.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pxlhghya.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hkvjjssz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3pwzsczqj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rkajfngo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ranpqtgv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aipouhoi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eaahymnj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qmsafdsw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3oheocgxp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3psurblkw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3avscscbl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wimkqywi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3pizolktd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3oguuswsb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lwulacls.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dfoynpvq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3erbrwrbq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3izfzrvlr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3crqmadwc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rvmuhrij.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ipwtffbd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhmzrzgu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ryvbnykr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hfwgvdlm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pvtpfuiw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lcaqmhxh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wcufqsip.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3wwzmbeev.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dkioguqk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nncuomds.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3mkhbaykb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vwlcxsjh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bfzaksxj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xbspqghj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vpbbmbsp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3tpvfstoh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qhehlrce.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zbvhkxum.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lwmhdyzg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3mmyabmqo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3utoslvuv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3urnrdcnm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3tamvdtbg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfroashz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jgzkyljv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3fuguwpcu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3juzbnljg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3avijkjuu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3daipkykx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3zguaswzr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hrjwxrlh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cmhgbatm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3epjielxt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uoggxjvy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zpdnemtp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cihfjbhd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3tnslxcod.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rgeuoddt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3frchdytc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ggkmnxyb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hvyvfvuu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ufclloum.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3hyhmwutg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3gkawuvgq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nfoxahyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkfgiwdv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zzkayudt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dndxcdqd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3pbtojqxo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mttrzrbh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rhabfdrw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3yrkkovfx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ayndlrrt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gylgfbok.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hnmctewb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3quuicghh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3cjhxnzvl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3dcoymfcv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kyrbwppv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3sskdigsf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qxpogwuk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xztuutxl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qkphghfb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3pxlraybg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3uusmjote.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3chjpezjj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3eielxzvp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bhcjqhkr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3yeiwsvjd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cuepgbqy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lnkktghj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3poqmcfno.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ehgdxzru.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jsgvhouo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwyzydsv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kqbpkchs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ivaybyzg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3pwrvhnag.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3izkcmddh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kwfubyuf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ytalwhcl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3zivfclyz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3uiizloao.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcrklhkb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3twqapfaf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3fahxivzs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ftpsjjpi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uvsjvdho.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uekumhrf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3kmncrnsh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3robwekrt.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bcjapgvq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3msgygyqm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3esekmvxb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cgggaoap.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3bjniipqx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pbgsljcg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3scjemhok.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3mapwvlui.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wbitknyd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gzqboirp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3naeewrat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3inonmnqw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3eyqlyqha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbqxnsbf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kamnvcxa.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3cdkcgxlm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3exdnuazx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qiwirpxn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3khilnldr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ismihuxt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tnaxqecb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3iehizsvn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jzpeuads.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pepdcpvb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3bwadakvj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3yjhnyleb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ybcassfn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ykgikrhh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sidnsamr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3fgbpojmu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3qafemgqh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ndvzcyxl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3umkinwnl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3dqyezlki.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3miwjyqnp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nzlqwnqj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tflxyxrp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aryttspy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jbmkxlmz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xocmsjyz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ksktngti.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fbszsifl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3bvikzwsx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rokyuzyw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cjwoafga.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fetbmxzd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3joiybzgz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vhxcjjqc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3stbirutb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ymkablio.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bmbpmqtm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3sgpyjjpp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3veyyjxah.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3jrlknzti.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vhfbjgsy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3cwfprraq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ijxvefta.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jwmoejly.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gbkmsgbu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ewgtpntp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3belgqqax.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ftlmpnme.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3dakvwddg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vwuykhez.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcpxtlrk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3popybetp.html


<!-- 参考信息 -->