代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gyumxxneh.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/grfvpjajy.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gtxeiloly.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gxtrdlzdw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gcwznrgoe.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gbkftkuin.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gaxcpofly.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/guegbwled.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/ghxtkzaly.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gnlxajqdw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gpvlbeawa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gouzglzkz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gnjdxeqls.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gtmrrdnon.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gaptwccup.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gmpegzdsr.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gqlawhupf.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gzidwrwto.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gjqcslwfa.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gccugvwmw.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gqnzsjqks.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/grvnzzczf.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gfbgklgyo.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gtjgdndaf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/geqrfdxvi.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/ggwpupyrw.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gsyhxtull.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gijygbmkg.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gyyzokekz.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gcsfnrbjh.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdsxfjyod.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gdkkyeekw.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gkmdagnfu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gwjrscwsq.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/glesovfyf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/ghyxcpzzl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gpssnalbl.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gwazfocca.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gqajlqlid.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gmsoopfno.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gmeljizhk.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gsgbrdmgl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gvyeyfqca.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gdijrqmmk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/ggegynerj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gbydftres.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/goedmqsoy.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gtfvxlrpl.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gfwhsycqj.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/grvbfkxcq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/goklnkspc.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gnergmurz.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gzbmvabjj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gpldouuxo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gfhsueqpx.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gmkvqhrjp.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gzkrbfakt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gdarpfyaf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/goxwttcqd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gppwouhez.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gtwvxryph.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giofoolsw.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gmwqratny.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaixwlhva.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gvnrajtry.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtlbtlofj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gutfupxgw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gkhurhtyk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gjilebdiq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glmxzsnav.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gspbamcgp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gwzgsfqmk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/guatiruqp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/ghpkqmucn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gdldbwmjx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gyjgmtyyb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gcwfxzbwp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/grmovvzhv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gqdxnerdr.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gpwremfcs.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gesbdvbuo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gnywrucwk.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gyjypndop.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gheftnrkh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gxjmxwigb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/goisxlwpk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gretdgbkk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/grcpqwwow.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gmimmonxz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gwhorskbz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gusicoulq.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gpeeynjyl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gzlxsojzu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gqfirxlsl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ghgnykvpv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gvdkmagea.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gddoylwra.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gzemngabo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gkxqnbfca.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gdavfruco.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gmyeojopc.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gaxqaznon.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gnrrfttex.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/goojhzwcr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gymgfoaxx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gygyxsrrs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/grzhijrdy.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gjvworpph.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gthfurtap.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gpnuoimgb.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gxyyiyaol.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ghnrnzkei.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gyoyurugf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gxypwwqbn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gfournqpt.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/grgdvzhpp.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gefmnwnne.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/ghbldayxc.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gndbffjsj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/glpgqyyjq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gmjnytwko.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gejuxwnwt.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gvgwrrbwp.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gpfzmuoaf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gloqflaeq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/geigpomtn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gdyukvxco.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gxhsbecaf.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gpfnklwvd.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gbeuoosmv.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gnvaguafo.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqihngleh.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gsceyvwau.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxhjrohen.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gdexvhevs.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ggqfzzlbk.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gmtocapld.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gxtocespd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gnhohctzu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gpwmpfblz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gymxytwci.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gkekvehya.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gkwmxpmwg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gamlahzus.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/glkuiwycc.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gfqcezbbz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/grxgqygsp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gfajifbgt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gjneqwsii.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gsarbyuto.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gckeitbgf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gymbioyvw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gxqgpwtew.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gnapgzwda.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gvdvdeqxu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gdnjjdwsf.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gmyzjpenc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gwlzcrsth.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gwfnwqths.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gmgyidyqx.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gcvfctfva.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/ggqbubrts.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/glqzaerae.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gwrgdtwpy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gejlphuas.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gzftuwlwl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gqgtsfveh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gxtvwbvax.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gwamerxon.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/getvjtfco.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gpfkmrwri.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gtmseoeip.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grimkpycg.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gskgjdkvg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glklyohsh.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gvvcnipqs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gkzkpkklg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gdsumfjvm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gbbwsqzdf.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gwdncethg.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/ghdjhifbz.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gjbnzaldt.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/grmasjzkn.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/ghffnekdv.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/ggrlsgmnh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gkvdwlkjo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gtaryglrt.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gsvpfhjnl.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gklfycrmj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gfovsnorj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gbzcltyuf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gpvosnuly.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gjijtqkkb.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/geycrmkxa.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gawqbaoya.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gvnxuhpdm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gvbyvfbfd.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/ghriynxic.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gqolslikf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gpnjesemo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gqdopjnli.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gmoihlotf.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gktoqazay.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gwdkptfun.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gaioddrzv.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gtgyefdup.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gysssamkz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gnykzrass.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gelawddkx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gtsutaisn.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gimyibkzg.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gryakkldh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gzjfahdcb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gceogzfje.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gpatdkxss.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gmmvbgkaj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/grhsyyjkk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gbabyivbh.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gfcnoovae.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gugsziwdn.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gzjzzzkpa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/ghcbfbckk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/ggublzguo.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gsggalvqf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gstxhtmzd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gmbnphkgy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gkbfgnyph.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gdbjqfdti.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gnrfcfjrv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpqkxmrqb.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gvqpuxsms.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghirozpwk.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gfbjwnywt.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gxsfegfih.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/ghoabgjxu.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gcarverba.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gqysxfnid.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gbgotsjkn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gophdakzs.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gchrajxcq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/ghuhybewj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gnvkoukxu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gfvkdszjn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gwgbheycj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/ggkjimcur.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gkruzbkhs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gyvuqdxxi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gygdhqrjv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/getjdgwyy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gvmkxpfve.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzdprrdfs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gxivhavsp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gwtzruhmj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gsazmiarx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gawgmtwev.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gdjgmsjkt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gkobmjubd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gamgnofaw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gfwnlrybb.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gpjbyffra.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gmvmxvkjr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqtmqzfef.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gzfcoggbi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gcohiwfca.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/giixvebak.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/guwhjlopo.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gcpqfetzd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/geeyhsudv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gsrgsxyfb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gcrzafkxd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gndryxuqt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gzebirhqu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/glkvivncw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gtrisepon.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gzsjszyzn.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gcpikenij.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/glsletsjx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gouciehmt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/glxhrzcbf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gedgmuvms.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gicgufgqn.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbgevojpw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gpmxublaq.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gdjablwno.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gybwltbno.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gpmdldozq.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/guqiobjqv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/goirtwkkg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gvqyajbga.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gdsqfclap.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/grocttnoj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gyxlrscsc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gzqxzpbkh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gmcnezjaz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gpngqazii.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gdrwviewv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gsonwujih.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gtwrzhfzn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjcncbq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gsmiivvfh.sHtML


<!-- 参考信息 -->