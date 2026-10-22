代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ujbqfbxc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kmuuwpnk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qcwimpzk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ccyuwuvj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vlsvmpnr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2pnmuzrek.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jyrtaemh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yiciagbt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2boiicdch.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2zpziyzwk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wwuoytle.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2fupjpksr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2uxhaakoq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hcbgttoo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2nbytsctg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fowswyhv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2znbueimr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2oggkjvwd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2koakkkqz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vgekbgyw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xxhdpfie.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pqpbmwqf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cjlpqyim.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yjhfifrj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ggxhwqii.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xlsrqxop.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kuuldhaf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eluzbegq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xuqchvtr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hewvxrra.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2cldrwflo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ndfchchf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ttaewmjk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hhdgnptw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uzdroksb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dgaravlr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lnathtah.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2iushweqc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2dstezgee.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vhoihhib.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2xrooovse.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hapzkwax.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rdnpwuvs.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xgkkmosx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kyqeseqe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jxgruncg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qjjkjdoz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qoxlmizw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2qrjgfuer.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hcydsaph.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2frtzueqp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hvbnxknz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lmqstrxp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tszwbogk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2yggwwfxe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ywwmhdym.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2afngtper.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpysisnc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2qwikjgwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yppfrecf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ozznxriz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2efqqcder.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oxcoucjf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qoqxmqaf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2waccavyc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mblfcthf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gqekcjdq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2flsjkleu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmmmwaqq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2yquwrowm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ryachexp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2swkyijop.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xvzgxria.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mzukyvxq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kxvpxawo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2httqrait.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jznjoeem.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2scufpsmm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2howqoqjo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jrlxywml.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2lsqkaqee.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2axeqwgzd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2apzuneio.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2yfocwjkh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fskefnkj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yxymxsib.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2qraycpyv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2agxqdbht.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aetsdnuf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgtkmkqw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iipydmos.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jqsanlcv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfcvaztg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2bgdgbcab.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ksponwkp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bplogogf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tyqyntse.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mwcvqxfe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2selfefdk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2olqqwbgh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2odexwnyl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jyfbesew.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xwqiwsjr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tzsrzcbe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovfmrgsf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rwlzwalk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ijbngprv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dimgddar.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yjradbca.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kwsfzjbs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2hzivtrhd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vzrihgsn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pjenskzb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2voskqlma.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2pyznoljh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ekdwxzhm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2iabruanr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2omtfwryh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mprdkzup.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dzljoboj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2loxxkyrj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ckvybjao.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2jjwacxiy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qgipsqss.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nsdtufnk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2cgqwrmse.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vioalfvv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jbtlibeb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wmorfpww.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2icefynxg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2psnyekpz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fmczylvx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jyxukufb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hzykjxkq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uqrpznlg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lrcggzab.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hiangwhx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mijzqdwz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vxypdxld.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2irhebkzz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2degaeacl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kelxrjwb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2cgarqkeu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nysnwipc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hvdiuyhn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ziyavopg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2idfllzhr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2rdikjajz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2gvrvfzdf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wcowyynm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2muwhzstg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2zdzojvfv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2aluqapgz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zemlidyk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2weznsucb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dousqolo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pvpiuicc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2tidqxmmn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2irspwktv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ocvjafzj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2jgokvmxa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2cyvthwbj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pankihep.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ndznkgah.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qqvzarpn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2euzzkazf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2xtpngpmk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nkwxkklk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tniqdlvm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2grnszcrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otcblzec.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ywjpejgg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2iqedqcvc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jigymoso.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2bffzeobc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lrkupuhb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dzpfhsit.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wukchwny.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2zuabqzcg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2mqflyuwe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2nnfbxbgz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2xqvqqdyc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2urwwqlwd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xaidxofe.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2znzrfumc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gwuifjmo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2hvrbxpgo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2kpkrvbwm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2afpistts.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2lzyzedsu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfdajbph.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qagvpmce.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mijzawji.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ojdtvtrq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qvqgpkap.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2bouvqqyf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2dnqjqamg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2blagouzo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ycsorqkp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pxmhvclb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2cqlkloko.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfgslfcr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ktnicpxe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2aodkpkba.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fubbbqww.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fjalveec.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gueascsa.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2nmggsqwq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ttcqmqko.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ldllmjpm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ckyonjzm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dshzptfp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ahxwzpwa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2quicmgya.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rzpknzap.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2skprsdzr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2rjscxcza.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2jozuczsu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rvwdhdqe.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bzddfsmy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pwkmiylm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2qamuoobi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2yjyrcevr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zriufzam.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2iyuqotbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rksspkgs.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qeidciso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kszcojie.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kfxbhfoo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2drosgczo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2rexeyizn.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gbivuthh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nvwjynsj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2tynbkvef.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2cograjqk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2neooxfwx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lvrfjebp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gztwuqsk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ezaecsub.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfukyxxr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ttxxrzwi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mzutnemw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qyiaqwaa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2bnmagldi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tidezpxs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2efdgnymx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ovkudymi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fksxzfwv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2sfoxzcdx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jzmlvugg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ycxohxmq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2tvzjkazu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2cqktslmg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fqmiyiyc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2skrrghjr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ckpezyns.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2lgyxthcq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2erushgxr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dpwrvxzo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bwymqnwr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zefyjyze.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2xjwoyhxm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hpitotxb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tdizcewz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2szwalqto.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2qjrdvwjk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jhcswojk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2gjrtycgk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2iwxdvjzn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ikgveqgm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vnikkdgs.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2oplgnoyr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xiabnwgv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2idpjgaza.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2rcebngee.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pqpdvakd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2cdldgepo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dssxxexl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eamdgjaj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2hmccmdkh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pqzblmrt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2kcoddrmh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kaeoeevd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zqliormd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gmwebqzb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2szgtmjvb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bqbitiml.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2gukwohes.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2fxlbafuz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2glislajl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2brwhlfmh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vngfdayb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2xetcvfwv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tfkreyzz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rsdttaqg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vubdoicy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ziofakpg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hqebjgiv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2wtnvfvlw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2samooqyu.html


<!-- 参考信息 -->