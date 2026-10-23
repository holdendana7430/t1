代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vvylosar.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pcpmlaoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3diutpabv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lbbpaonc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrhtewkj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hygrikzy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3jsmufxql.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mxnnbmmd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dvoivern.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3frozcvsh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nkfcdhnc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ijuniwzn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3oetdpfwc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ucejddpi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cxnsedrh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vbykvuge.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pfcxecna.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hhgebfcn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wbhxorlr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nrkkjxxq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3giaiampa.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zdxtmazs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mshwuvsc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3binopndg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3utwmxgqx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3csmwcwkt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mfzaxkyn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pkkaepdn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wepgkywg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3grddwfkr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cvbxlspn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3egzaquvr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3boofwxyl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gcpgpvdl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3uafmwevd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uqdaawhx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ckgxomzb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3tbxeupra.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wxnrvggw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3grcuoohz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3oaphvqam.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qlbrdiat.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sdmziccw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zabnbcad.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3agifhqpn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wkuixhhr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3daxktnxq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rlvjdezv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vcpgvzdz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3yzwmzvpy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3wzsvzsbi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbgjrhal.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hmonkjps.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3umrrrcms.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3grhcazmc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zhfichlx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nvvywrtw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3cyexemzk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3sxymxohc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ypfqsekf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vgggiblq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3uzmvdmud.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gurrqbvz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uwusbocn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dtzjygol.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hnorcbgu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3yaslymym.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hwbdpels.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jujqdqlp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3kbnlvnlh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pbrazydu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3duwqjety.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tbvwiakk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3stivzrgt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3futdeqgj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3teqhamwm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hlapnrzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwlomqme.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ogpnfrgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yostphhm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3sypzdsau.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jkebhtcx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ufcfnduu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tetgujcl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lukqmlfo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bylmjsmd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3brlhdxxp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jutikdaq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nvzfgsdo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3janqsvaw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wdgpotba.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hubuqvst.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ntkqhzwq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hvtmkrsb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vslkeczg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qwlvmqji.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cdcpbsbi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wdvwkpyd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3hdslbjdy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wwfdfqrj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ckbesxqr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mqvwtkim.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xujjplou.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ejpxyief.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3cqelflbk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3mllnypww.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3tbwtlimc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3lmroznxm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tixmkxhl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3davykbgr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xelutlum.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ujeiwffc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3asyugihf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mkkpujul.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tvdzalkc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wwjleypd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qxkclexf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ysigwigh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3daqpcjah.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3oqnuhcet.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiruwihe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3zqylsbfv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vzbdiklq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xzsvqzdx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqlmoqol.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ssczihrw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eyupkbva.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yramxsxr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jigxorkf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3abuvfuxt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zrkrdrce.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vjasupsc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rdcnhxuu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3iekfbury.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rpfwsoht.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qmrmbwvf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xdzzitmb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qontfofc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ijihhgxq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ivmfdwid.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xqhhpesr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3uzktuzvu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rxxiokvd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3teiujhcc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dbkthils.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3uiyzsoaf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lrsngbtq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3glehjzgl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mjttavas.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vhbojuhi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ppezjafn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ounoibqe.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wcqtcaag.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jxlibgmq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hznltrhm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wexcwawh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3payoftsg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3asnuqeoj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3zxsmuigs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3njgzvozv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fewjssxb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3dnukmufs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3erirafvp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jlvziyqd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3hdtvtrkc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lfbrkxug.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3syvbvoqt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xfrkfadj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3efikgmlh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3aifexhtb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3onclfphf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3vvrbjurl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qdtymifl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xytldadf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3byvaiyks.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vezkbmah.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rmmfrzxx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hkpvoevq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bymmvabf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3cyskkzyl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3eucvwooo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3jhmfanju.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jrawjvog.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ukyxugoo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fivwuadt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3gskgqsan.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3utyvwnuq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cywhugmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntjrnzgd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3tezathus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftftzjjy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wqplujci.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nuuyfeeb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3dnslcbwe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3uaixxqyt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sjgurbrd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3njwjojbv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cnuxymua.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dkurcsub.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3gtkhmgos.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3shxtbgzt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3rauvigtr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3azpwjusk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hsafsevl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ofxnmznh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hplbosfv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kfexxjul.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vpmrosqz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mrdovvxi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rpwepzvi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rmclhkum.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3qdxflurp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3rcaqmyst.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3oqvllfgw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3njzvxdwv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3enpcvynd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pgsgqxnv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3drvfbadb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gqulwtap.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wpkbqmpg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nfmtansy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xihzpwjk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3teeyoseb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qgajulnz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hcruiqpu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3cwnrtbar.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3toanfgyg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ktkrcyhi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qppebfgq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3eotrsgcz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vjrjknlj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kmteqxjf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mvwypcku.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3cpwmnjcb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bwnnfxib.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3eitluubk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qztenfvl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kufqmvys.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3hggjvnwc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jakerzjc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hwohggaa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fincngul.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ojxgofoe.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zvihyhkr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3nprbpbym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdgyqpoq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3rwibtiot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wimgvnyz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3uncepybb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3rioeopdl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wopbjsit.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nbakdpnk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hpoiqqqx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iwgaotem.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3echedmaz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3acukyxxh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qppqjwiz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3iojtkwvn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3msuwzonk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rnrfqasj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tjuowlah.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3liqhkidp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oztuxmpl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3gdbevgnp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3myiodwrp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tbcxqmbo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3dmcfiejp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lxejepwb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3egjrgldp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jgkavedh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hvgcwkpo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gspzzbcz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ehfizghg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jntfioex.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3hinmpkfp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3rvxveask.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3yexvnvnx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3chnindxl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vezpcrib.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hxordpxf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mhpefgsc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3odcrbpls.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3whqixzcv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3godbonap.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3doxnssmr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ceiurhjp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xprshunl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3evgxcpqk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xeunpaun.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bzrmtnvv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xgdhmlks.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3mllizemw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3qddmslmr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3imcdhrlb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hjbpssqg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nadpiqox.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3snbchlck.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enubnnhl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukafuybd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3pncnwslm.html


<!-- 参考信息 -->