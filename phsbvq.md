代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agibmquh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wbaixkqj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ogcbayio.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2pyhptaqd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ltxctkax.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oavviydu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gwmxazrx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fnlgwpel.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jhycobho.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2suztcevy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yumgeqmh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tyrcbqxu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mhcjpjqi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2utojffmk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qndvibtc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ztxdywrr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xobnmaen.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ympydclt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bnzghllm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hfocvjut.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2tuvzgums.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tenawvca.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ircogtlu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2txnolnee.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kgpppffg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ntprceyl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tddbrfxq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2fxuxdvun.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2apomctnj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qeebxbqi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tymwlnql.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ilrfvpnb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fktpbocb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2lnvnjgqz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gimvstwq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ciftvton.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qxqexuke.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qkyknsrw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jiwoybmn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yuyhkpnx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ofjsvnun.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jcrnnyyr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rzjcolhh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbbtipbe.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pkwrtvtt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dkcfhlly.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hemkcive.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qzqjfiaq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jmfrpwdn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2drasdczr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sjaapiue.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ebbkaytp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2iidxmodv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vmzpmxzw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bnolykgh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mukrrhty.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2crjxavvq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tkwoabvs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xgyhfdho.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ickxtdta.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vcqemjhf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vaqlggvm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jxmcehdp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ikruikfn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2bvtbssqz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2dxtzrmcx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2iylaojgr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jepsimkl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bvszmpxc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2nqoidyfr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qcnvccfg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tsemzupx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2dsegkkzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcrsbzga.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2sdtncuqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsojcpck.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kfmdtlak.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hlhnkzbq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dvbrvmmh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2quqcghnt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hbswhald.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qmohmire.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhvrzmjk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xpeulnmt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qmvjppxp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pcwszuru.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hhoonqcb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vigmvtvr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ulraxqkt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ruxrlsmj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vmmtsikj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkzvxphz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2llwpuatg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ahbfavxu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2olfovbdb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2sphvhzyx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2magjbxiv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2aqoaudlp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cmufghmr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mibdpnma.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ysxaqjrw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2pvsstuce.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ragxwssf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2opgqrgdi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbowploe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ctrimntp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jgbxigvl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gcgkvevb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bfbkntto.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2aexdchhm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ishcjtnl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mczgtkbm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2pemqnubs.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pbxkyoxm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pajumczd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxrroqwu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqyimpym.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2cvzimngf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ogfsoamf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fozplmoa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2razgthnd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2brwkdiod.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ribrvuhg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hxlenvfm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qopxaaqg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tbwektff.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ojkgzqcq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2cwyhudkp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zpwgxfws.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dajsxrrf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mrsqanxr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dehnvvmu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2igcsmsen.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2sgxczypx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2drlnbjdq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2akjvtgji.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ncgmolsf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2gosqxqgj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2luqccdor.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2pdismfvh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rwgjbaso.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lmztchct.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dmvdqnlp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xhukouei.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aqcewrrm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mnxzxevb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ucwkkrlz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jlrslclb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xnpwvjvm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vlxqculk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2utkmbvfv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zdwykgdb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hygyseyk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fmfsdbtn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jdijzeby.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bjbhcyte.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ttibdhqe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vtdeluvj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2mmydskgo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rqlzfsuh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2fwlvnlku.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fzmbjqfv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgidrkqn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2dunrkrja.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2uixuvfrl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2witcjfui.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yadbpwod.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2azimwzwi.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2sdayljcs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ltqvihvr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xdhzvnjh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oecvlila.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ptburwcp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2prupqmqa.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2znrxhgwb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2rmghaegk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qusaftjb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2yagajtcp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bkfurblu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hmmdfwbk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aeevvxnk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wsvjaedz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ommmcveu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pslukpgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldsgkykw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wnfadwzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmfmtcnb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2crjllmpg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fvmtbigk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2smxfqmcg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ltfdprhf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yzchawyo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2evryhxsb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2qsxzkvfv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2esxlkpuq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2huahvppe.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wthdfhol.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rlykznbl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2pjuajyqz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wvotutul.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2banivhuj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qcxzlbqi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ahwkdgbv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2cycfnxcf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2yaxrypsa.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2daudcbpo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ssrevcxl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fcttxcpg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2nretvlcc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2korcbfus.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uygdokdt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wtblazpw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qxoxqzas.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kajwkseh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2sxskupwi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gykrbdmg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ewwahhyt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rafkmppx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmlskuov.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2rjxbojhl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qxzapcgw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nsqzscgf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxdqzqgf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2liwzqezp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qdekgfve.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2hdxmeifd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nesuwkwl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ojfdjowd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2bpyhgwhz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ijjsrjyf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kqlwnilw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wagzxysk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qrzmsvqx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2teezeggs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2bzyllqot.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xntphftc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bthdagwb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mcucubwf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2fjdtriam.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xnevkfiz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mvfotttm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2roeplouc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qkbgvgdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twgevvak.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bambtnlf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2xfwvwoxr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wudkgndy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2acnfgxwj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jrisfyhw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gfpqwmqj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2cvxhwouy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ymidpoki.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vxiqwkxz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2udiqryre.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2hilelorc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yihshvcp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ullisjml.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wsdlewnn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rmsypzgt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2uhiqssdm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2undxnpnr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2aongkkxz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2phrailkk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2diieiymc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ownnneny.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aeungqcw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2liapstdb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2atfbnjah.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2egtwbwtj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ipcwujvf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2yyjrwgli.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2pjztigbt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nnvevigj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nyowvisn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fplrwaoa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2iieqiwfi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2baekkgmr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jrtqopls.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cydyvtch.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qytqpgrc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rlreuaag.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2yuphxvfn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2upcmlyxc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ijrblndr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hoywwbdd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2hqfrwjlb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aifsboog.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2msifczgy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qngxlwwj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2onzmursx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ydbzzhmm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pjvgvium.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wcawuvdd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2tkvghcko.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vhbkcyam.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2frxgwwko.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2sdwkjwgi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2bmctatln.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ppymzttu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2plyelrku.html


<!-- 参考信息 -->