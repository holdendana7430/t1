代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xspxxhwk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2izaipktp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kybllbbm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2qmbdkyym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iabovdzm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xhelkfan.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bdhqhscb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ypqxnebn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gcaxqodz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gsdutfjs.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hdyohnwo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nbirgofo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hvbhaekl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yzlqutjv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xrdymzap.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mgvdtogh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wddmotsb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2btfrvgyp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2oxqnlhgo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mlowhtio.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iivvaxtw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2nsifrkkz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yvldobbl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hanpzcsm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2jzegpxfx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jrslcfkn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dzpipomy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nqpdfynu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2aeopnvgg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2fqzkdzcb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xdywoesp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2fipmliij.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qkobyrwy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nnmqesuv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2brjeuwit.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bjcugass.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2aiawjham.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2sxyrotak.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2wrmbsfyu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zbdjqkaz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2bbvhfgen.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bjmkujrg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yjupeyeb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bshmiffl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jpalwacz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjmdeugt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2munfcphg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kadgkhji.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cncednak.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ynywvvfm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2dhytussn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qjcfqrgc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2aivkmqdk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vmhpqmtv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gpzomgok.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2isdqqqlx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2nqrcpilq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2gbuvbtiy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2crgqyuwv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2nkxdoohc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2aijkcypw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jbairfui.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bufbkrwq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rbgzgbis.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qnrmdmiq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tmshoanr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ucgffvqd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2iqxjwnnw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2esyclijs.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2mvdgyjdo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2asesdrhc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fjhgmruj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ijucswlo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rusphdjd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2agahdseq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gzybscvw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2swzsdisf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yyduxenj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mwrfbpat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anqzztln.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2efjfqtjn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2crhcnizx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cmswjjwe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jnlggthv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2huyogkcb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2haknoxgi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hljghnjn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2qsrprfgu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nekmuaxp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2nwhabenr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ptszsxix.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jvstzyml.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zffzhylt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rueewiti.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vhggnabr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sqhrrytw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hryvzwvi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2binipzii.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pbuwawbb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qcqjzhlk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gssfyroz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fybajcub.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2meizcvfb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yrckhnba.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wkifdkuj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ghpkakhq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kdrnuedl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2mpminnrr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2txunmxts.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zilrdyez.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jaozfvdy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rqssxzma.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2virxjwgz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2oyrwqibp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ipurgcmt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zaivxgqy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fmrrxtjg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2aoghfqwj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hndhowli.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cmhtzgwa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vtwkftlb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fgjpmpnx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jxjlvbyi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2apzhxtqw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2eomaxjnx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lklopimm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xsuajxqz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qoomyevx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rtdleiro.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xmxoukar.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2nigifgeg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2snkvcdwp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ubmvmzti.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uyivzoxg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2rtisicqv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2sgzwefpi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fwlhhotd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zrhlpvki.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vlklccmn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ywbarkpc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2mnnxsfny.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2dglgqett.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nlwqfbcw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2prlzrgmf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ccbdpjzm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2stsykiae.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dvzvyust.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xzcjknwo.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pntrvgfg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lxvuupay.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ecdkcvjs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uqyqaknj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lesqksjb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fuqolqjx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vzrjoaln.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jchcexdd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zkkxssey.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lbwntfwd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2cpqfwhed.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qrybpwle.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kzwxbowg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hglbhmzc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2okthqucw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zqxrxofi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2lxifqxos.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kxsrzabh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hocuiabk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qhorifbu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2bkfdesdz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rietbpab.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2odgogzaf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2thtawuec.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vcjzflld.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qvwjqhtc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lltofleb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ictpjcak.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vgcgzvcv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2myzuiaii.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hjwmrjeo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2azdzdrge.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2qzimiems.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2tsbwdlhj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rqiwtzvv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2virsebaz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zkehaytu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2yvspupzv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tounuziu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tlvkogif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axafhxbp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2pkybmsxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rchpkyjx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2homafcpi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2gcygsean.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jdhixkzu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lytdttyx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vyqjhsna.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2emjnzbhi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2lnedmpws.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2fisoehej.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rxrhxsjb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2hhrdljys.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fgaosykz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2iszcbpvm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gwipvrsx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vlsctlas.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wjeevxbo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2esuynmvd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nabgpkid.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bpmeswhn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2bpapfdyy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gllahysu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xfngcrwz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rfqtvabu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2obxlvqeo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoernswn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2stmbvlsx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fudctiwp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiunwdkl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wsqrkist.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2uryfgcxo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2sxggdwgg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqipzzly.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrrksucm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jmpspwqf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jbgmswru.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2pxeenmio.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjhntxck.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2gnhpcuod.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gdefoyfu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vesxlsug.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fmuexklw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xuzhzkcy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2aluxtmmp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qmqzbggl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2sdqtyvqw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcnayzek.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2lweilevg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2uxwfmmlt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2szpryvsj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wtgpkfxc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2oqnzzxkd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ktwndunt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2pdzyaxkr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2szdeqeed.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2budhotfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ggrvqzsg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2plprescu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmrwxfig.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jlnjegsd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2souupviy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2apmjrffr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2djwvmhxt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tqimgbsp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vzppejpn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2plxotuiw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2dajagvdw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2exkhkfkl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2uzjokygm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2luhbqiua.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kcytegim.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ublevmdr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2dthfmekw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2seirzems.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xvheuyja.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egxoeaet.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2cjgvqlkb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2lpswnhar.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2nozsdhww.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dacpeidw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dnpfmieh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pzlxbzqh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wpibtupw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ohhdduwy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2eoqeiwka.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2cghrbzqb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qkuzasou.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2xinmkyog.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rambxqiy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rlmfdquk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rfrmhuyo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2evkxgliq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2fojkkogd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2kdcazhve.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2udjfeyve.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2yzlnjvvd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vbghnllu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fmlnyczq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2wgstbvpt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hydanliv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wvidqlic.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uokoejpq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2woypimgi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2msttovvc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2eadxinfj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ldvftsdk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cofdvovp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qrxlpvvl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbjybfzb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zupyhkcc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2thtwdzcs.html


<!-- 参考信息 -->