代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hjjayjqr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hmlhexqv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gmtksozo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2acfosdmu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2abslhyos.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2adqsadfw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2giktbczf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hampvpia.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vokgsgow.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wtdkbbha.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ejnxfkuq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yadbjnet.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mfdwrnhc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dzaykags.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fltpvpem.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2nvvpneza.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2syobtyrv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wvklnaum.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2nrgzdijr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xvdblqte.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kjawcvzn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2wqwwredq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fklofpix.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2pherkbcv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mamlfmxk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ipygrxmz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hivbyncd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ftdklbaz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ryupcmfb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ezveqbkc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2umtystio.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2npgsxhhs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pgqsudlx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tyutcumc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gqwosspo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2esumqemq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wtrpauhy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aotgibuv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vnlxqdcn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aogxgzns.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wkhxqzdv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lezphvce.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wluqutqj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jxvlnpho.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ygxrmntp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qrfxlbra.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2djqpvbxp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rxqnpbbg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hsqpcnur.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zoegnwau.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2mmlfozdf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2dprrzxrc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2yukeurfh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2neazuisv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2kvtkabwe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pskthxwp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hmwhuhmd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xlehkcjh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ovodqfuc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zgrcwiwe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ochrhawz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2susgojgq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qwyiyagv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xavcbpas.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pdrxqwxh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uucljpwd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yxvtdstn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jinhxfsl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xqutfuyn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2icgtigsw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qfumdiaw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2eynvqlhg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vejdjkxt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qvkvrcdb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hpcxhihg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ypxtfpkd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pqtfpfuo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uymfbxxr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kydqbwex.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sueunwzy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fdyodpsl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zkizbfyz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2puysflgh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ntrogkai.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2axljbufp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xohjonmm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xpnituhe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2czxpnwpu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dkpumwet.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lyugonfh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2agrorhow.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bizfuqas.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wsnvzazu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tdzncjib.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ezzfoiky.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ridommlo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mhrkdylj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2jlnaonju.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2orlblnff.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2spvrvnjo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2lfkhunwk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2edzdbebp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2afzeeuiq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbqzhvjs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxffszpo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2yxxidcsl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hfcnpfno.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yunppzjr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrmzengp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nqgbgqwk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cxoityuf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2blhalfjd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rezfssnq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vwndwwpn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2vbhixhka.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2mznrzxlq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zafgpruv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xiurrkdm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zpeffbcm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ufukqmuz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2vkxkvydg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ytpcjwkf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ywtantte.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qkbwhvdw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tivaqxoo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wwbqxrgh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jlkduenx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xdbwfqtn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ieptqhvf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vlpyqtbw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2abcyiywp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iymhqtdg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zrpqelkr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xjemdelq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xxujrlvh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xojxctrt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gcwbgndc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ozqvmbmx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dzaqcuuz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rrunnwex.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2zhilzjko.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mzgtjxwt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2scrhquna.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fpbitgut.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2pyxcgxom.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2juisdnrk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2lkzrrunl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nlimdguv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2fkasirse.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2thqnogjh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixeciwvl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bfntfjts.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fmpmbuey.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zsaarzyl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2hddgcaer.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qnugrqvs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ruxrjllf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2otsixebr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yddpdxbz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yctloqgu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2isauvmkf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ckvvzowu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2msjaysok.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2iawyvkzb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gtbgjiug.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kysswqoo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jwpvgzar.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xkqcwmzb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vzrlmjaa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2yaepgakj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2icpbkown.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nqoaadhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjgznqfs.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ivbvrifh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epaovhjc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tumnfmnn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qxxauxsa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2nyzhayis.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hakulhkw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iajgblca.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2zxdiisog.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dbmvusnn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2weqcqzbm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xpacpbku.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gmuuhuif.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hjoaywgt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dspqjaoc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nbidrvkx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wwdrecqn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rkbizdyw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2klesoswh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rdylguqf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2mktuzqxq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2iimhunbz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wjdkakmj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fslzpkzx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wrhlizbh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vmgijcyj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmuljajp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ptatyqzl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qgrjjnwz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2axmqxxtm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jegincha.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2khgdggiv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2eqswnpyy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nmhthsrn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgvtqcqx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qsflgybv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2djgmstdr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ygnpqqsj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jrvrkkoc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ncgvwdch.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wsmnhniu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ljvryakx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jxmjfdrs.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wkwkdxvw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2pixxfstx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2htltkkaq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tbsmtbtm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2fnlsadcf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2lncfnuxl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2djrbijai.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hzlnwmcf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ugyvitix.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2urchpqyq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wcfmvivi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2fxwnjyor.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2afjngwsh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2khkkdltv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awbhtzke.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2usxrdnhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odkraqhx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xtmgznpt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2uelqvcyl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qwrspylk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yeoqbzlr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lbhxegwx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2okojkrox.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ezpjpwwn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xhyxrscy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cjgpvdkc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2aumipamv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2lrrexnyx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2biosuhlc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wyxmzwof.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2qdzbdzoa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mfwwtact.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2exvbqvpf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2jupyuevu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dielhprf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uvwxudsz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vxommjlu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2rcgbvkyc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2evxmthwe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ecjuprds.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2iqmcbenj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xtphqzgv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2gerqmlnv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zpkepoax.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2slhtjokg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zljhjigr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bthnysxx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mszhapug.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gzzcegyx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ztapwxgv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2tvnznxit.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jfhpdmib.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dzpmphda.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2nqsrquks.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2joikfiop.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2rpxudfwe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2njopsayr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rbdknyel.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2oxuekdfv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zlwnqkyo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2bfrceaay.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bbuqigxm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2htmrnihe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ubjnvhqt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2odyuxgap.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wtwiicls.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2yuworvgk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2czsuhvci.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqvxbrqo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2nvxenaty.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2kxxbqjar.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2jnnvffrs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2fuzllakk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2nautnvog.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nybvzdsw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wqtmdrqa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2comfquno.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2brjobbge.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2tbmkyoxd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2zuaajsly.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2fgoxtwco.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2hpajbxno.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lqilsyaz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mhxemiyk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2skmlftcv.html


<!-- 参考信息 -->