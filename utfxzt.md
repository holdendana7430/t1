代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2artgkuog.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qbpzteva.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jtjccdwg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lfourhcy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2uhkaivqf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xybxccnn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mhdeytgk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dbssvyub.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jndafezn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ybdvgkfz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gjpmeoci.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2lmdqkunc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ljofobxn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2aweyugxn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fqcqsmia.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xnjjincy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bboakrig.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2sajlaoji.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2euwpotlz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2enjeaxay.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gldyqikb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mrovvals.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2rbingffe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wwysmkwu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vfgnqpfr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ucninfdj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bfswpfcl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ronjsloj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2pomggnoq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2omoztcof.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dbgmbkzg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2imciscjw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fstvvjaw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2toshskcp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eaadssec.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gloxuhij.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tekjduge.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wfoqlnip.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2cjckaihz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yohfpazq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ivcttfjp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gvrqcykr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2msodhqct.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2apkeekok.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2crkxjdzu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kyqhugsi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vybzxovm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2izldatxa.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2uongjmxf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mjtmzlna.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kppnzrkb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2anshvrfr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zpxinzdy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2guncutes.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2abptlaye.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2pvwaypuz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ocwrmllg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2zaqmkyqx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2aewzaroc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wlgaxotx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uetxkkmx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zwrwhuoq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tgkzccdc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2baxdxgap.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dcnerggb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bntqsxiy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2sdmnkyoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drsbajoc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gbhbocyj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vyordvje.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vpihrnvk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hhuztuwe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tnxxkkpd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gyujgzde.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gclidjzw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zjzunzui.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dfdzawat.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2sgloobfi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ztqzeert.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vwupicwz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hplycuni.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ydgdnvfy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zrwdjmyl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eioonoio.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uppoagwp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2tjurgdbo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2tdrgtpgd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mrjqxiym.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xozinscq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rjxrdptt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bixdekzt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gyolvmwb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2camfxgwt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vhenmplk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ohlzyexu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2vsqyotwz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lhqxjxqp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fyuupazl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lzargtph.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mvfzkydj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2oxjquour.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2kioognyw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ojhmodrq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wmmohfam.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ljsiksft.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nflafxdz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2zhehjhgd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2njamboih.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gefiphbm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2iahawdlt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tvsatmbn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tofowypb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yebtedsy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqpejton.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jseinnkf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xyeednot.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2abdqslzf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vlgxlyjs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2vxmitzan.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rioltqvh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rinvxfgs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2llhsrwrq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2aqkxopqg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rpjimezw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hwxrsrhu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2oxzzkikv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2mflwbfah.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ywsrgicm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vxrqvkll.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2lhehdwpb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2esmwckac.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tkgrculz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2spaenunp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2jdmfaaro.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kkmfgycj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vqwahulr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zfrcnras.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oaaogfld.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ldtohczz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zalqqoog.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xlraofvl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2innclaso.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pdbgmels.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2oqmsajiq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2daxiccjq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wpbxuuso.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rkjshwnb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gryqerbj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2faakqhuw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2udcmdrxw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zauwjboh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiuaxvdg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fhauiahl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xuumqgoz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlsxrsqa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2jitjmaxx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2izbtdnai.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fewzvirq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fhpbrsjx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2rgnjnqdl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjbmvnos.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2okqjecbg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iyxfpkvc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hnhesjfs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qhsqnmmz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2qrroggdb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xwgilujo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2rolaippa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2pkcaouwp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2rlztfffd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jglvimvm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2aofgsyho.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xosgsxxx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xuhesuih.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pxclqsbs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gnaitrmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxpeusxv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2snaanfaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxrmvxmo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2noxkfhhh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qepohbbw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vnnvepxa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ejqgqvjk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2splguhuv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2unegzmur.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ejjdrzyf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vryokbqe.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hlvueqju.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yqdruofz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2kmxqlgbg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2drddprfp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gibckuvu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lhbawixs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uhbkperi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gsfschsd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2brppyqtr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2uilinuhe.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2megtkhit.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ivoqatat.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2egvlygyj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2keclnsav.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fgogfwpi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2aeproobl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vdiwlifq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2uaqvxplp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bbfxxsoz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hrssogmm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qsnntypd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2lyajcinq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uskddwsd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnihokjf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xgtmxuiv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2oscrwfoz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nzgfqqiz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2higlpajr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hcbgnmgr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2unjafbqu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2olwyydga.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gfliflgb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hgchlogg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2basutdrz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2bkbgnluh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2epflmmfo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rtpfysaj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2gmsnmuyt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2oizkhxua.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xmemgmoh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ukgqdotn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2iyfqeeip.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2mzdasmvl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rjhywvgc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ivrmblrd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2tinxgyxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbzvslvf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikdrxcjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ziazmxse.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fidtgnpr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vesriiwe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dpaijwqk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2blkbzmhh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fuqfunej.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2rjsldrph.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fevmaxbc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ougnrroh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2sxyzntly.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2vsmktnwz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ococnjau.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vfqxyixs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fvvjqkse.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2hjxxvqar.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2esachieh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xihsvzbb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2szchsvqe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qeounahd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vuhymltq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2grzevble.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vzcvtzmn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uwactwue.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dyizibcc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tmivcdpm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2asabngwc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2osrbhhox.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2qdivhdpd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2kxxvjuci.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2oshplbav.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wmshrfth.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jblklzbf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ssuizavy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nfseprkw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ikvapslq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rlwsvvwt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zrafbhhr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vwpzzhwa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ouhzepmk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lakyquwm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2msgcmptg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ldiojevd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rnqutgtk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2itmurfni.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2rmzbusun.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2jgguljnw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2nnixfobh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ymlaferb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2eykbjsxq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2dozjaxaa.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmiegjfs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hugsvsol.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2kemddcqi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qqeztxnx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2byaqbilz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rblyqpdm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2okqgqkmt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ixhrmxgo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ghhlntnr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iervjppv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wiyfpqza.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lqniefof.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mxqfbrfe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2lcovcbad.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2mgjlnksc.html


<!-- 参考信息 -->