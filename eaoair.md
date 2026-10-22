代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhhbpspn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sddmcpdw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2acozmpkk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ajctncch.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvydkweg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zxcjflyr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2olgthhvk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2uxjjrrgt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2itszcxja.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nowgjgkj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qcspbtei.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wzsxwkzx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vocwzlek.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bxcxwnff.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cmkclutq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oeurgjdm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mgyqduvh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qymkilqr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dmjizurh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2bdenujpo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2rpuhhghw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2njuodotu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2shyjsumq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2trsszboq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cqtkbnce.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vveuahjh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ubnfttho.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ekxqdjgo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2yhqvtizg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zztbctep.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2charrtzt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hklnytkn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hvlegdpt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2mcecojqd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2iqwirdlk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vrhkhhjl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2cpgnbbfc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2vemtaiqr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sygxlukx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gxqbsszz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ioyujlif.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rhrrmvlt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ammerfjd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fexwbkww.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2dzhytnej.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rxzmfrlr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2gfmlztnz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dzjugatr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2gwviexli.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vjdgoxbt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2forbrpdn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jneyckqy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2uxhgsmdv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2owcivrnl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fqetvzwj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ftmooxlx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vsnnknuw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jofpsqds.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2pcgwnxwf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2stibqsak.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mtbsoqty.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2lgtsmabi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2tbdhpxgy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xglrvfrw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2vwmwonyu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ldbkbflp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2dhssnzrk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2aofdutan.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2iqjcqilz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2madoqxfd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ebepqiku.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nycvgnay.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2fyaudoup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrupkmjp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2olpokjgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qaqlfiku.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kketwvdv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmxjhrpq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vhylihkg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2prqflvwk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iyexnkqv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xubfyqop.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tprmgieu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2waepdzyg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjenukky.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lofadifa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2syzrdxuc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hcliccgk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yoyjofxc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dszenvct.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2koyciqrl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ysyyhxep.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lpvdvscj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oxcyqwyh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2askdfkxs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bxneavxd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2tazeuiaj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yugruxzx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hxpqgwfl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2orqunadu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qunrhbzi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2aegtqgey.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2cguoxvlu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2omvhgvif.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tddqqqam.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttpiehsr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ivlnfadv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cdshuexn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vsmrueyd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2kyhmcufr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nmrzymdw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2crhevibq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ysgvyzlr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zgybphso.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2hcjfgmeh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtsijxge.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mavbdijy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2uqudjqjc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2itvsjkmm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zofzouve.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2rtcpmxar.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mtrolovw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xvjucqja.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fghymrrp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tezntpdc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mjpcaxrn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2zbgiabza.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2jixyovse.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ilntohmc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vpqwnvgk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2nrrsjxpz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jnyqvkwh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2oleuchsz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2udzugjpc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2nfcwzruc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lqvxxhxz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ahwlnsti.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2faamduvw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wlayetel.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2mxunvgsm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uamdlgzl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2fnlitmtj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ytahivgx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tkuwwwhv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hosmhtfb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kpffyrjy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2deggvlll.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ufcdialo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vqqkdinz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uunpejzx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2isnzvugg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2abimbahg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2bvncvedi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lnuovugz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2wsgrgnpu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vrbgdtfw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qeuhsadb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ijzfkzyx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2iuwwtrfi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2leqzfppy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mzypbpmr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ouqlhmam.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2aslbeskg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ywiohfsb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2okkwzawi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2abowfybo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qiinivul.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fkxgdvjy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2iswqwiez.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xkbtruaf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2opdcxqhg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lyheovtm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sqfxbqjp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2krqtimva.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bkrchntq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2qppudcwt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mwpawcjc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2syrbpeog.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nlxgvstb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uohbkete.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hfprxooe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2cvwmvlwm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2sjnhjfln.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lqgqwfqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghxsakok.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2usuhumya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcawfebc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2dxwyfkyn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2mjgkgfqg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2oazegmru.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2grubywmf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2juflpvut.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vrsiwllb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gkbfmujq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bvocnnht.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2odxglgtd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nkhiczya.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2cexlrypb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ywjkvmvc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ysajetso.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ispuzfol.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2zyiloqiq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ahnzhcjk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tnbahvyn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2kiaqkpen.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hilkoxfh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwwvqlpq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fhcibypc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2yhxaffou.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vehklhmb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vihcwlal.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qrtxrnhs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2hdkfxrel.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsywuphv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2mkdzflil.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vzjynyfa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2cidklzzp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2etxadfyx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqviienm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2colxacdy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rytictcu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2uvpedxhf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyjjxhyc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2zlkxxgpj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xtnzpnlb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2zuxmahsq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ydxwdjns.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nogtbkkl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2icfdgftw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2iwkqdkon.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ltpmfozq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2dcptjqot.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2kfjcnxcm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2tkkbiufe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2qygndawo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bzwfuoqb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qhhlfpxa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fmbrhdhh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2kbzxvrmh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xaendfoe.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ftpeqvqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xihbhtou.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zjxtckpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mprjnhnt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ouzzrcxu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lqsjjwub.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2aiircpge.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bigvfigc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yhjspjqk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2nlwyccas.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gjesewfz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2rtqgvpes.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2tmiitghm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xtjgvmep.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2kyituvvi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2rwaupjem.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yoywsebn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2xlhpmick.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rifouwiq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2awyjivaf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bvywqoyd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zhufmlmz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2peicsceb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2wadjhqdi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ctzphgpn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xqdfmlgg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jtrfaiyl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2hfvlccow.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2uctultvd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wsnkbsgp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vzljioqu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2soqkqwka.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2yiwqyzzt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tzeroqiw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jjklmffi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mdyztjfk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cuifcpjb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2znyyoodr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2hpjaegyj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nsxetrdj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2sfzviscu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2aqwzhnal.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2uwmqmtzm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2brjecehk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ewgpkpma.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ywrywfmk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ldqzwkzd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2eerkwsph.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2jrnixjfa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2uatjnyux.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2odsnytbt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qknuqxth.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ejiqliaj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqfcbyjx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkhgwtlb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnjyypde.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2zyhcblru.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2itbqppcd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2yvfhrhke.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ujijkqls.html


<!-- 参考信息 -->