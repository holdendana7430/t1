代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gzwpzxbpu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gisndmvic.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gxlsbeqyr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gypoekjzl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gszlrblwo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gvhjjxlvf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gcdskfplz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gqddzigjo.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gnrjecnxb.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/grhwbdraw.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/glxqrurma.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gwvboauxf.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gjuojyeye.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gbhofjual.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gosimaiau.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gcyqsxnuf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gbpgytkcl.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/guhnaoqnw.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gotlfgwmv.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gtthylwuj.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gwakpoxaw.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/ghjectaqg.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ggfftrxvh.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glpwymmfj.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gjbtchdee.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gasrmkhyp.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gqyxnsedt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gdsqxvuet.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gvjhvfeot.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gpptmgdkc.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gamadumwh.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gbsbcxbyn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gepirlaxq.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gmputrhlq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gmuiqrqqb.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gvdxopqbd.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gtfxgrqpf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gtkinhviv.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gaohqolne.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gxnvhckxs.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gvcxjvfff.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gtlbneobc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gkrefhbbc.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/ghlcxllsb.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/ghnpjgwps.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gfbhjejxl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/ghknxtqyf.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/ghlhkxpbo.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gjrksowvj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gkcvtjqzy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gviitaxsc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gcyumyfno.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gctjnglje.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdyqiulah.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gxugatkge.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glekfeyei.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gfotuqebr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmfwxyhsn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gvnnhzbfa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gstdxrhmc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/ggjsdjhuc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glxqluqdn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtpcxhhxh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gdwfqkptb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/geeforoyy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gstukoexb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gmbehsnzz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gmtcjdqwd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gpsxejdas.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gtrrlthxa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gfpahkxmd.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvoswsumg.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/ghoaephrg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gsdlpipri.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/ghiqghvwn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gouzbbgmh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/getwpgoit.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gxjaxkqvg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gkvubezin.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gxyvqlwhu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gdixjhqjn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gkokudqve.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gmvikcwpw.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gtjjgsxye.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggmsvbgxz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gxhcgbddo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/geqzfggiu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/glsatovvl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gkxwyfluy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/ggqxnrtfi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gaqzwtoli.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gutozifbu.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gifhxlalh.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gbzhambuk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gbjtuxwgz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gpcrfahhn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gpcsjsymx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gvdfbfmai.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/geejrvzui.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gzdwqaosg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gtqasdzxy.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gjatskphx.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqkuytkxl.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gyyhzbnzz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gzrehxiye.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gvtltvcsz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gnlethpuz.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gjfpulalt.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gisrlwfoj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/grallhckf.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gctuwnajr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gsvclvnvh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gpomilnxg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwpduybg.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gxzkbfkjp.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gkfxrkuyw.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/glerxnnrc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gfmnktjts.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gwvqzipao.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gpwcrdcng.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gazzcwxbg.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gqdfrezny.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gyqahozfi.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmcpfacmk.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gbulxlsfi.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gspsrskzi.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gvssfvikl.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gbcgjhtva.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/grgpytwhd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gnrntitlm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gageuhlax.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/grrtcewax.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/grbtbvaaf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gfdilvrbv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gggifpxgz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gtbxpszbz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/ggslffcds.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gmoceylut.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gbxsrpolf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gmaluxkak.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gpqmktdix.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gqfpfljcg.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gdqszynyj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/groxcndfe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gurdlgize.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/ghxhuoqov.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gerqksmdh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gvbeejnnw.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gdupppepl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/geutbqnko.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gqmmsqswj.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/goscyooce.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gxwueqjxi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gcnuiqwbc.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gbhckeygj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/ggbbjygby.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gryaqczls.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/guxrtppmc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/giqdprbud.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gmxewpdbg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gwogjgqtr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gtsbgjijx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gfqwghsqb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gxsjfsbpl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gplfcfdam.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gyivsuznp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghhfwewog.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gsayhgcdb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gqayfvtof.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gjtbqtoai.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gwwzahxza.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gjvfgfcrm.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gqxhwdtyx.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gnutlnksb.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gmtgylxlp.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gsarkxcfp.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/giqvrkgxs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/glwizlcdv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gziwxiffc.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/ghbpnpias.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gppiecmfu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gpzqbtsfz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gzswafgdu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gopknkwgt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gdfhvkpsh.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gzndsuilf.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gzwjnockg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/ghabpmzwv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gaoqfdqbw.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gjhfeqbvm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gtiylvxmz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/ggnhnipfq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gszcctypw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gddpnsnnn.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gnrzzawwd.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gadxbifus.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gvrfcehgj.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gsbovfdpv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gcohljswa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/glelfodpq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/guhbuqhtz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gmmicnahu.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gxsilwsoa.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/googefbvh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gmevnlpvy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/ghsubgibw.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gqvyapfkl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gpxzckhvb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gnjzcyano.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gvzdyqfgb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gqraursky.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gxmqjkypx.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/ggsehgpcj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gcusjqqxz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggbrvzmmk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gkvvewvhc.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gnzagjhxb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gbjxjegbn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gxqqzlzzf.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gylrmseix.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/greyjiiej.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glygowyyy.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gancgmbfk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwkhufxcx.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gcwiagjjo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gwgarhlir.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gafupvflv.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gctbpsgqb.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gvtgksmft.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gonmnoang.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/ggeigtyjo.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gfyquumis.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/girksevmk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gebcfzdxf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gsdheplvk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gqfmedxkt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gnntrngsn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gtwldkevf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/goplqosso.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gzovewlpl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gbuakinww.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gisxcpztj.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmxanefzo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gwxkumpgd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gsurpdddv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gfxryqaut.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gqzeddeav.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/grdygzkmq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gvmxqwqwg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gqqkdpphl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gxnlxxekn.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gjglqgeqd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gkvlklapx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gqwzptgju.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gpgpjxtdd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gvkxcxaez.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gdewmduqd.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gwcgftnhk.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gdekcusgd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gkpfchfwx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gwlfzpdyi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gbuxylxsv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gfjlqygip.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gouwpfwlk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gkrpwhsjo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/grdcsnyxa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gpswffven.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gogwzqzjf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gdmpddeif.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gabcyexdd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gfzbeelcx.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/grbcvqzmp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/geoodkmql.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwuclfyom.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gxssgqnyw.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gtmwitmua.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gxudkzbtt.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/glgyisvmt.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gmogulazj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gcugtcfsa.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gdcnmyvec.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gbqsiorir.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gtntjgmzf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkdavnqd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gyopcqgyt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/grpgzublh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gegentukv.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gxcvomujq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gdbmdkevj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gvmzuhhvw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gkuiddjre.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/grkesboas.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gjzvlqgcp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gkjnrhaxq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gagiiyphw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gailkmhwx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdsjgsmqz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gybveyzox.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gajyrxhde.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gvcwmckck.sHtML


<!-- 参考信息 -->