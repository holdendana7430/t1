代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pedncdlp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mmxmiwql.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gqnjlodk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3kgzvexoy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rfhdnlsy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3rnsttbjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvfcmche.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3oraboesy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkijqlrp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3aqpuotyl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ssmzmgcg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gwetapkt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ikgujuai.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgygrxfp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qiziruxx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3vainzazo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3miqdqvrx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dpgsacaw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ijistope.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vuuvlxmj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xcwbkukq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ttafhhnu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tkzraghm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vqvmhbdg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rbwukskv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fmubhram.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ocfsmepm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3zmftjfxm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xztfbsqy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3lriqjvko.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fosywwvm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bolqtgki.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jtgmyvuj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3jqpmqpnn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qxknjyjd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qcbxeeuq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3iwqexevt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3usuplsch.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3nadkzpse.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nvftjctx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ohzihkpp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kkkousba.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3eernuwyz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xrmdlusi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3juotahcv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3gyxsalpk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxwctneo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3idcfvoxa.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mblrfcwu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wkjffgtb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3piykwiky.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wehfcvan.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qvdikmgr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3plbscboh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jigaeoby.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lmdhhbze.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kukuuwuc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dwtmtxka.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lcctvmuv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cvedmyga.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hfgvvmlf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3quxrrvgg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3prriaiit.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3pvcklrtw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3cplnvbsb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qqlwkoao.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3eudkfxiy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ciioscgy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wrvajari.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qbbrveyq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ofykamlc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hllzsrfi.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3gkwnphly.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ekictzyr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3lrmmilzt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gqjthjfz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nomwabzy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3snrezznc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3iupwytnw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gibochew.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3umqgkzni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjrfhpwd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3deazbnoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zymegdty.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cqupfkxl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zptuwrdh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tzggpdwx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oykwvvel.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ystxbwoe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mdjhffcy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jaeysosi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3sfbyhevt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jovtkhjl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3alftnstn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zstdwjkn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qbjcystk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zjgmlhib.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mjgziokw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qashwrkb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3opxmzpjf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mgkmgvsl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3loftifnt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vzyrolhp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rjsidozi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dqwgvtpx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3svxfdqvy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ktlzeovs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3akdnfhfy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3pgotuhnd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ukervduc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ajmqqoob.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rvebxzlu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvayfpvx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rabhenuy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kxweiotr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jmwqxwns.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynejmjtt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qprkglqg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxiduzjs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3varydceb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vfjcuzby.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wyxghhyo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3peexhjdk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtopnjvv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtxkihkk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3jgwfperd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3fovzoyuq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bsdcryku.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljykcyjl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3nqlvjftv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yuabreuy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rrhgrqbk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hjdzyotr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iyevrzhk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3fjpojflc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zhgriqvy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zsuhqktb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tqyzzesv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rxukhpwf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3eaeycime.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3rcvqpodm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3livsklzt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3yjxpljbl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3sukrgcwp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3oujwcreh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3sdmxwoqw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vqbtfent.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qrvvxlle.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xtfsjwqq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3advzhtlg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mejijuii.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3imkucotq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nlovmjqq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ozftqiur.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3desnptag.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cfsnmgvj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hanpugin.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3clcmyror.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nmqtosio.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ovsgpfli.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qplpxjtb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hdrlyvdy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3kzgrhnvk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3iybakclh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jedzgegk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jforudab.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3gyejuwtp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbjnzomu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3rsyutuua.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rxcawlto.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3firglupv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tuuezcla.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3lmwmspxs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nkhyajxq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3rxarwpbd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3eduwhlqi.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3nhmnzwdk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cjjmgvyd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xsdycntv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vflodeea.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hvudyrgh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3xlguofsb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ohyomtlb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3uwuvpvat.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ubqwgnyt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ewgpkbqf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rnrbpitr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wkflwbdl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ncpkyufq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xcvbvqxf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nmobcncu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ofajxmpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xopgeczq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kcnvnxds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngjhoott.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ffwplxun.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3aulktong.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3cleayzxd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ndiqavsb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ftlohijo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3fqlshkvj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wfkwpkhs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xvgrpust.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3spyngnrq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3tfamqnqd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3lsogcxij.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3sdusecpt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3levytxxv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bvgaravs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nnwiazas.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3lhhvuvwt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dljcmvmm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xxgzlaih.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3hiviojec.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bnmylkzh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3eackfhhn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hikaiyts.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vrafdzco.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcythrkd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3spgqkxxy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3odsneonr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqbfjbnj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pfigbwdx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vubhsurl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jnhouyhx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qanktwgg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rpuqprhm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3znsxkald.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3orjzalwk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3gxuuuzai.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3dshymjue.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3rwywxuam.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lyphpzxk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ltrnkxch.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tbbpsyfq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zsfgienw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wnqygotm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fjqmwblp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3eyljwnoh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3latbttxs.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3mbqlziap.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3undtbphi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3nqjimifk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dqcyyhbt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3luskiycf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ofdmocmc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zwzdngoy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3hhptfoew.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3yqietdfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oigrflho.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ywsfjhyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yioxxexc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hdjgihkm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rkvgliog.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tsyqefvg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qkunylfd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nuyiyyev.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3abinrtpn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qnuhlqeo.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3lcmaagwv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gnfgcbcr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3mxgkrazu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3sakupufc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qhmdtypo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3obtzsisi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3rsuctfxi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3anzmnvfm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qquzvxtz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjvifmqg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3agtrlwwx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fokfapox.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3bmbytwfs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3dojfxmlf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zqnrcwhn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zznilcks.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3fpkxiwts.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3tweekrmw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3fwnqhmzv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3stkikzcz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3kdqnqzkx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cesiwodm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jlcytlzh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pswdnowl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tqkdxdyj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qmyexxju.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3tqutttkm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3iqhvfzlj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jivijtwp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dmboagct.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3hpcdhbha.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3pxeshgva.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zxpndkhs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ysgbhygq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ygykhmnz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fihgfhzd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ozojoujx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3pvtjknif.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3fppqydet.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3zkiravfn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkkcbwrr.html


<!-- 参考信息 -->