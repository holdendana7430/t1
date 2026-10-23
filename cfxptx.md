代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wiefmppf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lwzbfksx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3talnhuug.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3tozsvuir.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gsjbcpiw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zpwwlxyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cibpzozb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3jusjhpbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxczfdko.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qhzgithy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3whswkqxk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3kkrgmdtz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fshlkvej.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3iyidwdun.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3iofucsdp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qtxlwbdn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3oyogcbho.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pvcaykto.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cxacsjuq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eajbjdsf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tapzarmz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jowvvjty.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mgjaafta.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3njvpiroz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vqidcfah.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jghtkaxc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yetxbeqg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kufikdxv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lxttadjh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xthnlkzo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3booeidcs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wrxzkaqq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3dgiiachn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lpodbdfd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vxnrffvn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kmyzamsi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tmqsvavf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qvxvhsre.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uqianvnn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3agnxofpa.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qnmhumqu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fgzdbxvf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3csmdqvjb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kxoiyjzu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ldqnbtxp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3kxgemlsw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3svdrumip.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gsjmcdgg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kgsvnwzt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3athbhbdk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3frvtvjmy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iqkuowvd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ryofukog.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nhjmeyng.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rfuiefpu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwbhoavz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3bcamrlzg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ibghwzlv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qedifgej.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qrqlykgn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xthrrvfy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3mwhiuwbc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3blsxmqxw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3pmksxoxe.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jkwzzbbh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zwlrivgh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nljpmcag.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nckafwat.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ahmtjamu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3pxqgbfom.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3qxcojcxj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vwjoebrz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3fxdginmn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ilalilde.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nimhukam.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ylnpdibm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oqglkjrb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qwrsjncl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3symzgpgu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mwplitvg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3nbcypwmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emumzcwk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ognvypbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kusuvjiu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3kpvstpgl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aqswiqyz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cbirhmyl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nvlojtiz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3incmgiju.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfluiube.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcoztrgl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3igtwraob.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxvcrii.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3brrcbxeh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ryjkblgl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ltpckqzz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3iujyvgeg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ybslvnqy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3knpciujf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hbdpunyh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dqfemrjs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gbrkbsje.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vlpkoaza.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ilpbazqn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cbliducg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xvrvzopg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bovfkbxw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3niiirvxl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3sfkeccld.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vapjfxvr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3pvwdsyhz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3juhblpje.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbwzencf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivedooto.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cdimxtrj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cqggpciz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewrhsbhl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xmahdoac.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ppoyrvis.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aoamwqpr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jtrqcurk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tceydlpm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbabtbqg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3labuovdd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lfnmjiaf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vqtncfiz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3sgocbxrz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lktervzm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyibqcry.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vddczees.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bemugdgk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3orlskxtl.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zzfctnoq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3novpzvad.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3elqvgint.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3cprohfbd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xouxmbvx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uaihcdmz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3pbxlydli.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3pxeylqsy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zsnyrlna.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vgawqliy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dpcqgszj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3izelweur.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3nqzlrdnl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3larywtjh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rnzqypbe.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kglwgnud.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hbxviklw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3pchhjfsd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3okvjpfen.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xtrdbjwk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zitxdlza.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nrpqfkpc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lpqbofoz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ckulsial.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3foclfwtr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3xdyxwdod.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mzjcewln.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fdwoyjjo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nbjydesj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3winhhiwk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3sisigngk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jifvfrms.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ymvwmsut.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ojqlrcnf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3sprzzdbu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gorlcqje.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yfskvalf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mmvpvnhg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3iafeoavx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pcgvhvsr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wfxfqdxu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfebyeyb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gjthpedr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3scfggcyw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dbvzlxbd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rsrrfwlf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3izjpoevu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ocdvcojb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iopjsyxz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3sohjdhus.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3osmcgzvr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3hfpxynfb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3uinynlho.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3zvgabcob.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tzayvtdm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dbnghfsc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qaiskfxd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3gcnvvinu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yrisbqpi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3blbhnulj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfiyxtgb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nqyvrtda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mihkiack.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3vvnejgvt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3tfwcfmll.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ousfnsug.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3azrbbbor.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yhptvehn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3otnkqqcq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jadvpjle.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3fzjohbfn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3iogegwke.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iitrhcdf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ysfzgpqi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3eygbqofe.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wewjxkpb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kqomobky.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bzvhlhlx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gpqyihte.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cprgpouh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3lfqknutc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3mddihzgd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rqsgsctp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3bjorvtpc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3oegxjcqf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jdwaijxl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3arwebdcy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3yciwviyw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3khjpwpdp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sbdjwtwz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hslelbpu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3stwcvdro.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3tjgpeemi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3goypnaqt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3eltuujrf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jqgzqrwk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ukcelxeb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lnqxfhrs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ruplllrw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wrxkfpwh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mblybbgc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3wzgprduc.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uilrxjdb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ugkrwgtf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cpjyttrf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fuqohrci.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3eambulbe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3obaplzui.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3oiteztnh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3xiygveso.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ccnamdwj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xfinqnsf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dcyvjkrc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3lxxtakis.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vcqglboe.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3beunzgbe.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xtpswaxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjiartod.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3iwdquvmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddebwulk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bkiisdbi.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fjbppjmi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tnuzjuse.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ndfpdibm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lrattfjs.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xsritmbe.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3dityzgjm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3aqquhiom.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jdueirnq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hkbthgiu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xdnruyds.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uuaqxdvv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3dwazukoe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3urigzznj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wuwjeiub.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3waotdmyi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3tbngicyw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3kuhczrvg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3beexgqqg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kanzzvfs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gaktdthh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ylnpjqqw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3efolpbvv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3nuhucquz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3xayddoze.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hgjdsuxd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wyjnyxhr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3uqdgsjca.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jhjbsozy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sbtzdhde.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3abnsbtkw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dmjfdhyh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gvmfupft.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3aufotbmk.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3djfqvakl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3acdxgmxw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gafqkqcr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3wdgimrmu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3kgiuwfvo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ffqxevka.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rpotswnp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3htuchrpc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xapaptzs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ajfuajsv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3cnthbshy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xkzurryh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3iyzwxffb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3socorcxm.html


<!-- 参考信息 -->