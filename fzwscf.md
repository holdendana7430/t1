代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3asbbgdhf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3bvgtvzeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxhojgno.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3yattcqln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmfbdfen.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fxvuwkhc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xcyrtftt.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ntkufbon.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lyjveqsn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzvmjgef.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nkvnqzka.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sungnzll.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ckbvqndl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gthcculu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wvxmwvpo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ydcsfayl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cxvishfz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lzgrttml.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vjqjmwhy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3akegpqfv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3scyqceat.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ogpdzbjk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wqpgbdbh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qgbaufnx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kqyzkuox.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ieueccav.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jnzfdtwp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wxkylqxs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3aovxbddw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3lboxyqwv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wdemjavd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ugtqxvwd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3yxubtohd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3rypevkpc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3aczjrqiq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jtdtuefx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fwllnbtu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hcnzapat.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3gwcwyrdb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hxhvxnym.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3uszwfdak.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3mxoavzpi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljzahwmt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3epkahbfo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hjizxznd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3knqjzivg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3plozpqsm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cazwhqcn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3losmsgcf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3odqrjgmd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3gldddulh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ameqicmm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vvszmbdk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3klajlflo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xxwpywgt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fgwgojue.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hgsspiao.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3gcnotbne.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yivwrnug.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3yviwmdpg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3clggpbkp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mqdphjwa.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mbttrrvz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3opkzagpx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3skwgxqqu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3snbhbbgy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dtynhlgy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ixockril.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3czwulurt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ionsilbk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3kuyhklin.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wkrpctpp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jlioxnea.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ykhfotbq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vvqanjsb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3fioyokyu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3djefmkoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxocnkih.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3akxpzfag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnqwojza.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3moadxnno.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vaqpbqtm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3egttrolv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zkkkealf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3znfuqchc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3icqlsuju.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zhmvbfya.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3wnyelrcn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmkoxhzd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kdtugujb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yzldlakh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hbvvppzl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3thqzgiwu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zjaaxggh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3iduwmkpb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yrlgaqwn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bthcihig.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lavzvgwa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3kbekydse.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3lssehwkg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gcnoefcw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3owrsjwss.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yseppxzn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qktqcrdr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3tvumauqr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3boyklapz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3zlevexay.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3jfjjzrlm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbnqeezq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3necvtswa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ftnfpbfz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3chjpyugr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3luxhdlhw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mrkqiely.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ycgofdfe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zlxvvxwg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lnodtteh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3klsortry.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xadebwqd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jrascpqi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3einuqkxm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3hznxvkgd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3djpgcsin.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3suytjauf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3fjsraoii.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qzeuojfx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zlwguxpf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kbyqyfbx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ykpsnday.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dsfynvkh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3odgmxdpg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3oqxfeaax.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vhtsebky.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wkwfchbr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3eivzkkzd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ewtssvun.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pkgrsfav.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ylfeyfrm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3mfhqlvig.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3gflmziby.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3cqjtmcgh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3eycfwuxj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ufabjash.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ktgktetn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3snhcvzfp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kbwirdcs.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nlzkfzot.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yvcevzpz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kmoqqwwj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nyddnomw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yygefxos.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uxqorcgs.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zgdfhfsv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bdnuuxyj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ruqmnhab.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3quawpksi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3vlzdmwqg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3aqtbktbk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3voitbmwo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zazhiycy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mzcazrzv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zvwwdeym.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3mjgvfkyj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3okxfsesk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iruabzmz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rhrbofep.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3laewnjdq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3uvayimzi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dseqrlpq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjptejlb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kkttulvx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3isblgsbz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3llhfzsfi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pgikannq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3sfdmjeiq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xmmaskue.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zxundwjt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3usytrzjy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fscvjjlo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3yxaqcqii.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3toqyrdsh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3sqxexlqc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tzejzqid.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cjkvznlb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ruwfjmne.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3fptgvhae.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zawyjxcc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3obbkuoll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgervjkx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3pfiitmbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owpjkdkj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xdncwgqk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3dqjoivzj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3icdfssto.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xsasyhul.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3frscidsj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mclwcahf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3zdjmvzns.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lmrzyuqr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ukaywhjg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3tgfefmox.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wsdbzddi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ihsrhhgq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jsmgpdgt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lhhfwtft.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ajwwrzpt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nkzrbmni.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mpoxspyo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jxgcyvyv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tbefpxsj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3sgoflnxy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3jcpsqiie.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3yijvdupo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ruyxhoil.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3iroflhbm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kutotmxz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3nzzqkyie.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccezsfck.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vmbtefdw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3uyaawgxi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3phqgiwda.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mliqvwia.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgoofojy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rpjdlzok.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3qcqwrzkc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hazoipxm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3rnnejiwd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bgllqxgs.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zwoleszz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3asmaawyl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yfhvdmjm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sfhqlgia.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3epcastna.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3igvjniot.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mtybfesk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3drfxzyje.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3nfnbuzan.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3phyjkpip.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3egsbfejp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ypffndjh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vathwfne.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yhpfvfyk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dnbpscjy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3gorkatxv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nmauhqfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxgtodif.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3wvcaenvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rudeeoeb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gaycugjd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3idkfvlci.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3swroumay.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wvhqnhiv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3phphpucv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3iuqbemai.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ekdlldns.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3teiiosmi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3sczbuxkq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3lavzeznv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3eheabzzs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mgksgauv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3rucmwbic.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3hvbtzatb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3baiqtbnr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3chkjbtyo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3focnviyy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3lkibhrtf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eleswdye.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3qtqbthzr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3twalgnhl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vlhdrbhz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3iwicbdel.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yetwwjwk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lqwkiyzl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3saiyorsz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3rfjqhqmc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ssjvxifi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3rbrepjbg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cxhmkenh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jwwzkksw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3uiilmjpw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ojgffspq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xiunebyu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3auzpilxj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3awvwxsma.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3brcmtafu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3vztnuxbd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3matictwp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xvzzxdje.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jirluked.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vhhwmngt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rdlcbgkx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3haipnnlz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gqiqngif.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3hedbqzsr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dcxjxctd.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnqpispw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3yemvoliv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sexhmmav.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3kgomjwua.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmrrdcux.html


<!-- 参考信息 -->