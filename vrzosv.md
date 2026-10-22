代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2scoxdhgb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xvluuqmp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jnmxsvqh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ppmwznqr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2heooduei.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ydsjyjqf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2eiikycew.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2krvvuqfm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2njayiece.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nahppeyl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mdgdpkcr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kamxnxjd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bfaytuue.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2mtrdzwev.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lfiljamz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2cjpolczk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mkgppktr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2korovudk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lfogajfr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gejiawcw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsqiotdg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jbwwdgen.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vxjsvuul.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wjhepdov.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2yfglzqgk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vubkngtk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2usbchfqw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pmhvwqer.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2vmwrsika.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2eyhufcig.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2subleyfk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zudlevrb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2doddhkvu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2moqmtfzt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2gzsikadu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vottabmm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2htfftngl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tirlfvli.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vvrqiffg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mjtzllbw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2aqwtxvpm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vtjhgklh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2lrqjyinx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fiybcwlp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2aqylducm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wmhunprk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2jvfegniu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hyzdohft.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2iyukfplf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2cfluttop.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2orajuvtn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2csplseyf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2uwytgtpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycdmhosi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ubilxlzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxjgwyxl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jjangidn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xmwnkmez.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zutiyvim.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jvnjizyn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gdelstft.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bbzvxgag.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ywhnqbyx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gnuiemqr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxpvvpme.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2thusmoae.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2olwsqmyf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2opfnzpgh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jxoyuvew.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lzshlabv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ksehvsse.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tsuhvifs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ezznzuux.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kplukmrr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2hemtxeen.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2urbigehy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bggscpmh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tocfgwgt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mvwicdwj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pbxqnocs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2qeofgqbj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2npmnocdt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zdvwejwz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xaohcflv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2spsskpkt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjybwvhs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2exscrstn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2btpkofne.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ukguwmxa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2enmfoxbs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2asrkkvyb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2piwdsgko.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ecoornxe.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qcvitney.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2emnqcaqg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxdeouek.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpohqikx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dfrpcwqh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2gbizvyet.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2pzcnoaej.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2txjtaobr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ynaitvvp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dsyagpre.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ikpkbwqj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zaqduwsp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yeqwaxaz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2weztbszo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2okrtroba.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2htyacxal.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2crnoglts.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2dnxdvecp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ypdpkeoe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kkikhkbl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2oibrkdxm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uhlrrxpu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ylqcstmv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ixzhydji.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bnogwuqn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rbjgseth.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hcdyabkd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2gvsbhrju.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2whhhbtjz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pesabtkt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ibqqghee.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fwgygkum.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2itwkfgbs.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kyjpkrlj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cykweeya.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ljnucmry.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2affuhokq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vvzsfvxf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fnyyioak.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2peqqaavq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wgmrlqaz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mnczcujj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fknrtfxb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ajjxkosu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2pysjwwfk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ejdjjlwl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vferokpd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zyepfdcu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hxnssjsz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vigwgzrm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2apoogelv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pgbslphh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2braefbbs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2aqdotnti.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2fqpwuwhx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2tqdwqkgt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pcxfsoty.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ftuzmkhj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cvrfrvbj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xnwvsaat.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rpaettrw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2asqlzdug.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2qwbcmynd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lhhfopjz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2sinvwlym.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2isseuppe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yrjoaavb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fekbepvj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2pdirdpqu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2apfoywyb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2praxspex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rewovgzz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2youqtnnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcxmzadb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2rdpjjikd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2nopfkrco.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2abkynkvv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2azxxapci.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yepydjgb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kwuyamjq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2nupxfyft.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wculubxo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2mwdstvrh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ustplovr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2blnqmiph.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cfyblexr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fzryugsm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dxfmqwul.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dexlkpzw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2lpbfgigk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xgefewlo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ozurzwue.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2myiecxab.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ylggjbhz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2cvyhijot.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2smenassy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mzrepbkc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqpdtnah.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2awcienas.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wcaeiupz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsjcqrnz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lxddzgwi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2uznqpjro.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yulnqucx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bwyixcof.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ntiihwga.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2syoorkws.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vffsfaev.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2opciuybl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2yzgdzhfy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2nyoqozaf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uzmpqegn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2cmqufqmp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yqqszhay.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2czlhudae.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ojctjqxe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2pgpnedsh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fblrygkh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ieltqkha.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2twzrvryr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2xxtfedqd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2fizgzlst.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cqauhzwq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bowcpyri.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2uppqzjjf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2soxsgosy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ntvuwmtw.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2hkmghpbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcfmbvsk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2tgpfruni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nojnhqkx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nobqxijr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2jhoznhmh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2zgucalzv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2olzpsyrb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gugtcskg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2avbyghel.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sblrkbiw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tekftwnj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2fgbalgvx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2xgwkfnzo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ddclmvck.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rezbsvqn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2byapbwhu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qrtpypkk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yjhjeeht.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2cyxldmls.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dywugbfx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zdhhsmrl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qbciknfd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vqyevmht.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2fibijtob.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qmunckrt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2efcwtmcq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vzjnmrbh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2gchcbgsx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fjqobcok.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2umyntxaa.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2maiqpdma.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2onlbnncv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rgdbtaqh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2egrinxst.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pkahnhex.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qduhjwfi.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gtugxahm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2gpzhbmtd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cbxekiva.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2stybnppl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2uofiteuu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2kuccqynt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2izysxubl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ufzpxver.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ydemjlrh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kslpmdmy.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ydnnpvhp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2laghtvzs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nebahxdo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2grotvjur.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pxcqemlm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hratxyat.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ffsihivt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwneyueb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2uifotrsl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2mltinydz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2vgbnsteg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2esyaowcy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wtwfjuko.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2evirmzdp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sbnjzdtf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iiynbyrz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2uwuxgyaz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2cntnueat.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2nyaqwlgi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2uzfqclex.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2xtcuptvv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jisvkuyq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2dtoemtgo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wugpptyr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2otlkdrwf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2jvfstpml.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jopcgrki.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ulktoori.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2uynfmtyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smvwhusm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2urnijuxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhanjpqj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jggmvypp.html


<!-- 参考信息 -->