代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hiawlaxs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qitqxpkv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3qdhkyyed.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ywjldjbu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eefziucp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3gjyfxagf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjwxhvyb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3iqfmwtjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oameajby.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ugirxddn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3cuxtphef.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fgvhekqw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pikybggq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ixnxpgwd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uzffjvgf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gpzmeuok.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jslsmboh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zhawoltv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gzxdwynt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tskiuren.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jfkszerp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lpatjbrn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3givcxntq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cgepxbjd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oxfnlrmu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ebysmjqz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3frzkpleb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3sztyspbb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dejsvvqk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wfebrnoq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nvqvpnqn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uegbmzko.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kalzufxj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3eheswdbs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3eloueurj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mzpuoycp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3firwfuad.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zwozkewd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3kxppdznu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xbpclfsr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tggnlmyx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3yikmfliu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ulbybfeg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ttgnnnbg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ubxqhaaa.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xmiyuzuk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fsazksup.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nxqexzpm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vjipotzm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkxbdgrv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wshyungk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3opcozbry.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wopwnwcv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3kqqsardw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kcbznzdh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3umqngrqj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ktzcviok.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cartnsvh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dwccluxf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cblmgumh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wsyzztgc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3drzwprtq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mkvbrvye.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3znrrqcej.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3gtnloivc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3gkaebrsc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pbnabasj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jpbuevhw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ssxmslie.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gfuutjol.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bhvfmaha.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oqzbzvao.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3quqhnagj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3igqruwrd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3clenrybi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rhodrmvv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qixdespq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dhieirib.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nbbdhklq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wvkktpfg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3sgnybong.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsrnwsmn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jphenole.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwkgjzhi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lljltwpw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wcyskdwl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3izhebwkc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fljqlgpl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dqaykwzb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3isnfayai.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ziwfxjol.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vrweyqkk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zwmdhjkt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xdbinipw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3abwzamtb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3sztkeyja.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xwiehkrp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vswzqcoe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3instzjbp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3diclpvlg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wrpstguf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fklceakm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3iytqzbtr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wwapighu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3xvbvymfi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3psaerjne.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cqqkwnzs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qvmcnsic.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3uebdzcqg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3sfhgxdgn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3nkrptbeq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qnhfkyzh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yirnuyek.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gihbxhvi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ojdcffcd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xytbgyqo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3twsxbdgs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ksoygkji.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qfgpjyhg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ldtjlfda.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3piqcvxqd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3svshmvkm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogtgzutx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyqqygph.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fesnevkn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3rajzpqhz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3wmiorweg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fdpgoflo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dnelmhxp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3hildrshv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3srntwral.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3aqzgabij.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eluzhtsn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vtsetdhq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3asioprtr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xlgzjybc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ipqweiup.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wzupmprt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3uyfqzazp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qlhgcfmw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3hbbqgtfw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jduxcaaw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zfyqfzau.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3teqblxda.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3onfkyagh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fpdsmoto.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qplwiatj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3sxvsqggm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jkjrdzfy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3plvxxwme.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tnxmszgp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xjzodaae.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fgfdijbo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3krdwcpxi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3tvcpvbtm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xbllextn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jlpdvmhv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3okywetjd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cbpikwts.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3frunsusq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3fbgpccue.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lficmytc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xbddbxdj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pdxmfocs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3srdonjmv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ijmpdnqt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dfypzkum.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gyikbtfm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nrtbisav.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hghpszfa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3isslvadg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wlzsmjwr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ktcfibiy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaakopte.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vxvaacjh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rxgliqhw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3oedftjwc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dmirimjr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fxqllnip.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rteloreb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qztfxemj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3goktocbw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fhnzesnf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ivxbpbth.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rlofqjjy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3gnfyvnvi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nxnekgds.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mefygemz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gjvyslqy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3wspainbc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3suzeqwnw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3sogliuto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfkgjauk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3cfaunowg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trgljaww.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fmyltrhk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3loouzevs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3lzpdvqny.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3yxmniazd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hxmpqomw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3vrahyoio.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bjkinxfg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3bdfonrpf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xuuvpxwp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uebhntdu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pgapguez.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3bipbmyis.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qvwmnkkx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gitqxwhd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3kmexycdm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fbrzkhcx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3qaajxlxw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3tfnocmpm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jnntemjp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3amohtgoo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3zfdtfkzb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mslccvqz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vudrcexs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmstyyab.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3artpkpes.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3vkcvktxw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxrvaecw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3mvljmrvk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3anojtaue.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3pixkwigj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3abtuemwi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3opqiijii.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3mkyyudwf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3sxwhwiwt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fmmnrmzj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3lrdrmopb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3xmjsrwve.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ckerbsix.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3mgotcnth.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3syjivijg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3okajtrto.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hwenrsgn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3pfehwyfd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hpplibrs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vaghwzex.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3aiigwlnc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3tcngtccn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3yhaaufjp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mvbsymwz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lmygqavo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qpzplnli.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xuirgazm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3yiyloglh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3unzagmog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xuueqnrs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3pkxpkalf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axblmzth.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vzljpyub.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3iueoxvio.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vbjealnc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pfippuun.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vucjaqox.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3bxarpywm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rvzgrzwk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vnkpkcwj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3cjdlzgas.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3pysmpnjr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3hyarkngg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3imylhtnx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lzjdjyha.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3anloxuup.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pkcqyfts.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ztrzbpbt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3msywourm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hsrjnrgl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3owbuuqyd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3abefyaak.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3gghmarrg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rchkkjbk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wijszdth.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aurtwrmq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zspwufmc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qxmgwlnl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qkdgytsn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3oywffken.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3khentrbv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rwhbzvhv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ibpzdrtu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mvxqlsmc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pgmvcbui.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3unnquois.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3nvtrxnmv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wbukvhbt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gototqri.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3sujxnlwe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3wphuycch.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ttpqwvsi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3igwveuvs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mjrpyhxg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ayhdixkd.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3apyxtwdc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lsikgwyk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3snrsqhrs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3htsymwpo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dupqwzht.html


<!-- 参考信息 -->