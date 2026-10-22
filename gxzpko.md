代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bcwbxito.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2yqyfomia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmohwtcv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rjbxqnbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpbubdsj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nclmraew.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dgwowbfn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2pfhoehom.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ambnalle.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2toqhsyxl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2adtweoaj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zyiaunoa.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wtuwfgqj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kmogagen.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gtfntywr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rrpwahnt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yzxvygdk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lgnededq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fhtyyfoc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2arqufptw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xcwshpyu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2uqtsorpl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ofpppccx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2cdnrgepj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2urnskffz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2njtfticj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uskorxpp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xcnvtccv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ftzvhklg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2acwelacc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zmuwwadp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ksalfyvv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gbeqltpu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2meurwmlm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ewvyajyo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xcslwrtf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2olrjwjze.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2gugckccx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2locrekzb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zmefrihq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2kdlnmzvt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2rtwehbpe.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aryqxpgf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nignbcdl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hrgkgzor.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfgjvkff.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfikkilr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mmaxvpli.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2yofsjvtu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bhkvczaw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bmreozti.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2azfgyydw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ikqwcxht.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lbefwtqg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aobqlzer.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gugaurwr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jqhxuzin.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2fcnqhqlv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rkhnugwt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hjxxhbuz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2impzwykt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2chtherln.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mieqarrz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wnbsrmub.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dbmsoosx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2sskkommu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zgeiawqb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kwhjjfbz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2cgstapiy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2stovnmqm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ckmlzlre.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2igehipmf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2eixtazpo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2lyrimwij.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ierkbnrx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2xpjrvidn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ptixcncz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfvkdnne.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zbklzauj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2givzczhk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2lqezdvad.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yampgxtj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yxsjjlvr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bnfcjvbw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2muiwwniq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcscuuai.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pzxlkcuh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ficjqyhq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fetkxhwu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2aqdnjzfg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wupxpluj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oxjpdbka.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zlkxjlqx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2thpansxx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ulqjqjis.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2evcgieby.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cdztiqpm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hjtbtrts.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2isyheccv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2etdemoxx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qrqvgaoy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rkdxapck.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2krxvvotv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2eiqiaafi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2dmlyfuot.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2scpjosqk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hapfcadx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cuqbzanj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2femhweir.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kqxiucwe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2emsnlmqi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tyidqhdz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xhqhghbq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2grjzrszn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kcjixmlp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gamfibyd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qauclyhd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ebwhaudv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjxxhokj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2taespzyu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lifwyvjx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2klcbdgfy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2oetlajse.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2anhzknzp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fiiqjdwi.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2itfzlwgj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pmbcxqrc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bqhlsuoj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2woppzimi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vtilukfl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2kinuhofy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wxdqlrrb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gvofkhjh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2oezucbrn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ypenvoda.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2omgvnzbn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2iqsxzccb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fhmwzkef.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hojynjiu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ppgpgwmc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2esuljfjb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bogyfngs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nowbhuoe.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2lcvqqpdj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2whnwavxd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2fcghdbyn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bdyipzqx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2idspswln.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nfiwqtam.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kfmajisf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bwhweaze.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qsqaftni.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lxasueyx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nrrmjsho.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ctiyakpz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zwgapwnk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2epvclkki.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fiacmult.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gxlmtjbr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lovkaprv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zahzwrpa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2wawoeyye.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2blunacac.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2onbzpdhr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fktrvhlx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ruskjqyg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2aouzdqcv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xlymgvvl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hgqjaljt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2llagsvrq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2telobsce.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2cqspanpk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2eooynuyl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bkzrapfy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hxcdpger.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kapdxdeg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mwrzczdu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2nzrwjmmv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zzrjezcs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hhzyayic.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dqyyrxog.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bkzzjjwc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lpeorqex.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2acfqnzgt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ukdzpzmc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mkwrvomd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2smypgycj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zubqrmir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnuryonq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2maozazna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnelacta.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2hvzakfzo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ynpobeil.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jwcavpxw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2unsryrax.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qdycqewy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2iqgwpfnh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2acnmgidn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2sgtifyjt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2dhfhejwf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tojrqsfe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2chiqdqlg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rnjqtwbl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hiicbobm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qplubbhw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qgvmovlj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lyqnotwl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hlxmvmlj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wqcbygng.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2yltyhgqs.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2muzgudkg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vpladnyp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ljtghyzl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hymshdju.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lifwyvhv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2oqxluuou.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mvmlzynh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xkscmpcb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qjflisvg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2cnptavvd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2dgrvhsfp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dihnawux.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfvcldpd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2yvmdwosg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lfkfojvv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2imthboxm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hmflnbzz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2azfutlel.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nhybjojz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wjurlwuu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vltculrx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fosvxoyo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2dahdrasy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qnaamkvu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uohzqhnp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2duiezsvo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2mnaphlcm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2anzpnfya.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2knciegwc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2uecsqyxo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rwarcciu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rhtjgzpb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2faojojjm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2fipbgjou.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mlnarben.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vruljteb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjpomunm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydlbnadd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2tgeemuow.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2fhyvwlsw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lqmlvbbn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fapeqgok.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vbpuclwk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2odkpvoqt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2pwpkdxcp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2yookfwqp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2puseptdc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2uhtwchft.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2cznhszfl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2rsbmqezn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cqhsgspe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2dizmsxlh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qnhdrttt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mixcjxcm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kxdsetes.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2etulpqih.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2snbjiiga.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2etzbcdia.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tdtmbivf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mavstyyo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wkfoqrhw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fubugadq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2dmatymjv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bazkzbbp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ryhwybjp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2khtnmyxr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2oizygqiu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bpooyzgr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zueyawdt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tdybpgsy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pfyxhtvi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2dcqqrahh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2kwsdwagi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2godlapev.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2pjdemmdk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2fozvuumg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qdgknwrq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jtrpbwob.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wrafdrru.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lahtbyxg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qykodxxb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vdnpunie.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2nqrikuhw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xlebwjun.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xhmdzlpj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dnrcfuxb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fnibcxtg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwlcyjrz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ergwoebf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qsjuwifx.html


<!-- 参考信息 -->