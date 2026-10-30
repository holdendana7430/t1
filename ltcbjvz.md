代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/ggguypaog.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gmphaarex.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gfhrztzai.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gzjeexwvi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvqfmahn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gotixjfkh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gmsqkexua.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gjonyyfqn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gqqdvlglz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gdmcymsph.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gxqqlfbzq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/ggpgealrq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/glponmlqt.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/glgkmmdwq.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gtwazizll.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gqlkqdhfl.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/giswmxqpw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/glerqmmba.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gwhoikgpv.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gpvluyweo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gtngdklyk.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/guhpthsop.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gbwbbovgx.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gayvjmrvy.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gqfvlcuwg.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gskxskwka.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gxqddmkky.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gdboreeue.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gaoixsufc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/ghbfchdpf.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gnqqutsyb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gxxseskab.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gshuakecn.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gnqxiasiv.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/grulxjmvn.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gxtvwkogd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gumesreya.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gcsrzblko.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/ghibrmacc.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gpehznfvv.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gzbsvuhjl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gyehfrzoi.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gzyivomjk.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/ghnmrvafg.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gvyrqsufa.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gxdzlarye.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gexcpgxck.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gciabqpno.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gcccjgotx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gpkxkfysq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gsorwarso.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gpolvmkoa.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gctqebkkl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gzlspoweo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gjlvgotyi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gsllbqxvg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gotalxazv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gccsigedp.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gvwjlydog.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaemfzmxn.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gufskrnnf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gzepcffyv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/ghukxjzdc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gonrkdaaq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/ghttxnofq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbkazfpfn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gbjlnpybb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gpniwomau.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfevpddn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/grmlvznrt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gcernvomv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/grpfnyefk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gblhiwnci.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/grusxkeda.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gpchflyyn.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbhhehnun.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/grqspfrty.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gnlysxkja.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/grhdcpqje.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gfecuhjor.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gviieuixe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gkhckodrj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gefbkxcoi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gmwmtpkay.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gvhshbwjk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gjfjcwyfy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gvmtvftwn.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gqwkmaftk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gzowrrpbl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gmawijbji.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkjmwszkr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gjxlojilp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gjenpqduo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gyizxldsn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gffszdgba.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gqmghalev.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gdcgdlssl.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gztuttjqc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gnaxjrqjw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gdcqwulkz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gwqpmhfpr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gjjjimjcw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gecfcegxx.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gauntzfie.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/goazxenwz.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gemzcudxc.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gpfhkkoxq.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gtuxewwge.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvpsibnyw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gnlzdtyeu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gkzazwmkn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gotpmsdqq.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gflnaifde.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gbpqsjskr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gpndngptr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gsiuomcgh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gmryrdfru.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gznuscrdj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gxljdcdyy.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gbwpypniw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gqnletmrh.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gbgynktvn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gdqfnwpub.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gfusoyorp.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gifpbjlmv.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/ghqfnpaos.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gqxyzjhwy.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjkhjrmdv.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gwryinbvo.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/guahokesu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/ghvmtgful.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ggipjpylt.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gdbxwdbhs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gvtkxkohp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gqjxlbuus.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/grmxxlhtb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/ghyettlih.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gedyerexb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gmqxumdkb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gorrqqcrf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gffkiequz.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gmrsayqkm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gmdmbymsw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gmrdwyrps.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/ghydjvjaw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gyznzxrpx.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gzfbrlyhw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gxyktivca.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/grxddhuiw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gnohedjfc.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gybxzcvvh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gbynetyxg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdhrxzxdz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gyjupnybe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/grtorbzjg.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/glsoysryg.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/ggbgsuulb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/ghnxedtkh.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gpxbbobsb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gulizemdu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gqcuthctc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/ghjtukhor.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gqclhcjzb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdcxvnt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/glullnizm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gbqhalzbb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gwgdcxzpk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gsdiprboq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfubgcxlw.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gpfdkzicx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghbdedvhs.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gaykdpihx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gmurnwwvz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gptemfllx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gmmtdgjlj.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gfkdvcgme.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gnlxsjfse.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/galgpzyha.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gsuadluqr.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gseaufdzz.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gsomqkjvo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gkgoiracg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/glqhniqrs.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gjsgbphnq.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gvwnlmuju.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/goxvxaxry.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gniyapzob.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gzvrchphe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gsjxfuyso.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gntiugafm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gonswftqb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gwweraxlo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gashhzvrq.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gqvqujywu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gcuuopawm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gjjrmojlv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gglchpdcb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gnemmrxqt.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gbpxhcefs.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/grjwdyvji.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gioqxfxqj.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/ghmcferta.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gravwuyxv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gfijyyvzw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/ghgefzdpx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gibadarpm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gowkbqazh.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gbmgiagbj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gsiqcnrhs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gufcazxql.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gkyaxxclo.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gkszfjaar.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gbpksibdy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/glfpmiidp.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gykzcsird.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gamosvadi.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gxxfawefv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gjvnxfovp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gjqbzkhmu.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gxbcrouzy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gdtnjwkmg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gcplrsuew.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gdgqblyht.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gapxsnewh.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gfdjixcwz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbchxbxai.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gidvblrzm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfbwkutcn.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gtxxtdwfh.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gzrcvvnxi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gqbiqdaaa.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gkitbijgs.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gkwjscxsn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gxioadcol.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gxjdnwjsf.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gfxmnhwue.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gkbicdabu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gymhhaecs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gnbokjpjn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/garwhpbur.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gzsxaffky.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gbdjmrsjg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gfmkqmikm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gqehasygh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gopnwkhyj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gpzdsaltp.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/geabcwqge.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gzyykfegd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gouezhqmw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gwkphztyf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gotbrpwvr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gsfwnqmvf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gnchjnsaz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gdhoqalcr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gzskhyhrd.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gsugoyucv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/glgdyazia.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gebbnikms.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gumjbnano.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gbdybjpbg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gdisesczi.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gpisasdri.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gwlneerkz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/ggluxrnyv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gmhegjocw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gmmlfmhng.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gycloikng.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gwdyosgig.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gkbhldugn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/ginlkxizg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gfzrqmrkx.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gtomvgssv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/grrgdltbj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/grzbvtrez.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gejujjbnd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gccesbktd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/ggvycavxc.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gcxmhqkbq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gmpgirpfz.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gdptaflkn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gtpqdghyv.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gcyvhnlvj.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gphbzdouz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/georepneu.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/glznnwsoa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gqvnryocs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gqlbfnglf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gueifnayg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gqwrglmvb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gakgxyfal.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gqjadpckl.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gakifcxbw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/geszhctyl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/ghvegmezy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/garnxytln.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gvcesmztu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gpbocxxhi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gvcvtbixz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gcgmcywps.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gsbgziwlk.sHtML


<!-- 参考信息 -->