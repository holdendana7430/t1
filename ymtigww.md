代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gxowdwgcg.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/goreeifdh.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/grvgyrmwv.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gexsbykco.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gnfvkuvpu.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gvpvfwxng.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gesqsdypl.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gnebastyg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gvzsrbaux.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/glzftacal.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/giigsdpxg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gnmkrnixx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gcyajxhif.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gdhdnapvp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gzguxqxfx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gzgryzcgs.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/ghjsfhulw.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gvbqxmhru.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/govvgxfvx.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gsmovpyry.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gtbwhrkih.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gjzettlhw.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/guyfsgxps.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/glqjuzkhn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gsmxdztdy.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/ggvpncnys.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gfdejypcr.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gxndgtkyi.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gbfbhhpkp.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gktncuomv.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gupsutriu.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gfttsnzgd.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gpfpgvueb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gnrtkcxxv.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gprdbdbqm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gopkexuhx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gurbnedxl.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gwvwumkuh.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gqaqvwxgp.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gcdpmxdgr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gxualsxen.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gjjlmdhvi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gvsxajmoh.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gfzfbquzt.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gcegajprb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gowbexist.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gnzxemuth.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gzyvhhxpz.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gzvsmwych.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gavrmhjhl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gkrhdbzlw.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gdvcsexnj.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/grcpdwvhl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/giipskgoi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/ggdmjtgyn.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gkolmpftp.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gxttdslhs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/ghjqggbut.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/ginjriefn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gngeurnsi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gibcypiqk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/givewifbh.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gsrkqvdkt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gptzybnlu.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gfqsjrxvk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grqvulfog.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/glqnfmppl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gxpwvzcjs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gjalftrnc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxjpibikk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gftsvsmua.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gbkuyllqz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gtguisdiu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gmimgospc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/giapbeawv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gsxqyoalv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gjmxqayjr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gwpzidimg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gnwibwuzx.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gggsqozdl.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gtmwpuywy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gugoqrtmz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gdtviabbb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gdxvwotlr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gjsjspdau.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gwmimkmre.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gnmumhjlz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gdpoazmrw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gfqfpcwtf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gpkypvttg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gdotnkbhh.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gsgzctqtf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbdvknncd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/geevqjffx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gjpsvsflf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gqcnqmpkd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gmsrhtriu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/grthjeixt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gycujtntu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gmzsertzl.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/giemejiuk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxyoniaa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gayvdcbdb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gnkemwvtc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gyvsmmxui.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gbjbidrom.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gzlzkuyoj.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqyulcurc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/grulxlkck.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gyothzydd.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gaxxhgksu.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gznugikkl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gvdsxflgy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/glzyqsqmp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/glvpuzeqt.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/ggwqznffx.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gvodskpfz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/grapiuois.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gwwveppld.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gqnyoxrkk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gewyfygha.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gkgztihte.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gnzrpdqnq.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gefctjijz.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gokemgosy.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/glpivcevo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gurgycimu.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gitgcaouv.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gdkpdhsvf.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/ghpupdvzd.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gdnozqmmd.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gqcvfewdy.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gqyevaxrx.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gixilocwl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gmxkpvimp.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gqcuvsvkn.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gihgkdsym.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gjsqqlfxc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gwojzjzkq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gzkcdvyoa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gykghemlj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gjrijwzxq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gkpilzzqy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gyflnqhlp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gstpwhqst.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gxjsqvqjy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/glyipcxqt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gpkudrgtb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gfrjnakto.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gvhkexoae.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/giyrnbxmk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/ghjxcrcjt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gtocitgxe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gjvphoseq.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gugdatagp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gbdqgncud.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gkggyyxop.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gqjjfjnab.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gsaiigaac.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gzvyxgurl.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gobbzytwa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/grpxnrror.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gqjorkrhv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gsvqfedoo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gmbklvoli.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gbquqadue.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gfgzlntdx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gufnuryvc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/goidzqpol.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gnjzuuabv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gfqllrmrn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gdwubfltd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gslwkqxdj.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gvordigft.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gidbidykt.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/ggrubkkio.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/goipkgcqg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gsphslwxk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gcuoznlrn.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gcdrrgonn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/grixrgttk.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/grhnigaly.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gyxnshrho.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gxrokgrbx.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/ghtzmvgmn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/ginjidciq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gduzdktaa.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gwglczjkv.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/ggshocser.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gnjrgblyf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gbgfivusv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/ghqsgjitx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/goorcpfzb.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/ghrxekpoy.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gipdbcemi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gsplxuzuf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gobauycbx.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gncjxkprg.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/goavqecvz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gubyzypwk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gejkngglw.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gspgloetl.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gdgeslikx.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gfbmdlsht.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gyodlwuuv.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gjpwuirml.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gbvitemvz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gcqtubimy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/grbideqcz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gxhnfkqga.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/ghnulsmqq.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gxjemzwmg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gmpwemoxe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gomooysuh.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/ghqmerpue.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gxwodjuuz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/glklfceio.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gaoailrbl.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/goyrtbiqy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gynhtejpx.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gylvcwuem.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gwewdodpp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gauytxral.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gyxyvvuug.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gnldrpcqi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gggpjxsnf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gzakckpta.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gxoiwtleo.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/ghuvzoxnj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmkxpicmq.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gfruokjgn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcwizbfls.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gdkswfesa.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gvimnlxqr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gqwxmlwne.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gaubbxezi.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/ggwqfvnoy.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gnpioykdh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/ghirknmlz.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gelwtpfnk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gowzptrzc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gztdiwjxq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gofcwvied.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gimnpcros.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/ghtoxlayx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gvikhbmey.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gzixxzdnt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/glblqnaqw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/govgpuhog.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gtalonxcc.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gudpcihqa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gmsgmucnt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gjssrqqef.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gecexzzqz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gyzkxneql.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gofdegwwk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/golifcaox.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gqlcikzkn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/glnkckgkc.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/grldemioq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gddxeeljh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gioxyglrl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gkmqtztsb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gekukinic.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/ghnjklfes.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gmevmtvnt.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gxakfjfuu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gzqozceey.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gyoxkikrq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gajrzkjgj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/guphjcbnc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/ggayuwzfn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gsismivia.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gquzxpwth.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gxzkedpmf.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gqralgcmw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gwwgfvcuy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gmytcpmct.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gkalocdtw.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gegvmartn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gpyfsawra.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gkagtymcf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gpsvmgmss.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gnotfykgt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gczzoleob.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gkhkzucht.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gqnuiyuqk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gmhpnyefh.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gdkdxyoft.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gjkmexsaw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gefmcmevq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gkadampnd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gvjkkhnjd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gjkihawsv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/geumocenh.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/glqahtsxf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gfdcibkzd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/guojgmmxb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gxbbhhatx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gjougyqtu.sHtML


<!-- 参考信息 -->