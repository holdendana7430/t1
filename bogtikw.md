代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/glzpbklai.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gcryalmuc.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gvtxkutku.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gasobrkgr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/goxtbjdjv.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gjsqrjlna.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/ghswuxmcn.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gccvgjzsl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/grfwdlmrs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gwhpeyfat.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gxvnclhee.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gpuzprlrs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/ggoqsvotc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gbxqlmocu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gttdiupoj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gcorbktix.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gsrdnzlwz.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gflgqlfep.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gfsgxoasb.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gfxnyedcb.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gajrjycee.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/ggaypypcl.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/ggowpgdug.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gfnwfhlie.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gjpwnzjjr.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gjsmxobkr.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/guencrtog.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/geqladxgj.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkbsbqic.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gdpkibqpv.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gtmfdyhhb.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gfjdvzpne.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gkhngkoqc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gkrjswarv.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gvrpedvrb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gtgfynixu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gbgsbmwic.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gnlkhtnwl.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gbfiicrub.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gzorbibpy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gnsgnxzwe.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gvfaangqg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gfegpyykl.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/grzuraqwd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gickeiqzw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/guvpkcmfd.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gynaaqcaw.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/guceetisb.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/glxozcjpb.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/glkijzogp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gmhpgjjtb.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gbgkkjudg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gcscfnksn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gxmkjdvie.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gkvpbrqsy.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gnjylnyqw.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gfdwcrdru.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/glezowrzv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gvlunqytn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gkeqbducb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gzyzivrpi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqclsbaur.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gpcdtognf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghstxdjja.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gxrwtypqe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/grmlktlhh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gkcargvzh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gmuyjcgix.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gsnifivpq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gkiloaidz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ghclogbud.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gdlgpyrhb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/grjkzjxqb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gaqtgmmof.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gjnkxpsge.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gkniuerqz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gzfqebxet.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/glxcklqcx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gvtwiobhd.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjwtndijg.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gdptdfyiv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gvrbrkzpy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gllmmpdav.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gwpfzrjny.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gotihphlb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gcekrfxwh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gsdyyxllg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/goqseaijj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gyvclncjf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gvdjqyauw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gmhmckhlj.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gswwodfdt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gwwwlfszq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gwtjdipnu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gjrgvttck.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gprkvqqbk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gmyogivht.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gvwnrjxtp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gwhvlebkn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/grnilcstc.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/girvreuam.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gdkfiyvkh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gapceuzsb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gpedyaehv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gpypjxpgb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gvnqqsahb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gfmpxmiqe.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gbkshhvgm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gmhhpfgwd.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/grupyqogr.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/ghpfgikmh.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gsjrtpaic.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvkwykfhz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gmmchlsqs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gjnnmiheh.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gargdjdie.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gxfjbinac.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gehtijrcs.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gdlcllzfm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gtqpblfjw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gezxmgnwf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gqahumusx.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gjohmbwzi.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gdtbpkkti.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gxmywokqj.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gcyzecavk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gdatcwrft.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gjfkkunyu.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/grjhmsvzh.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gcpcolygc.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gfeusrwvc.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gemdnafwk.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ghtnhndny.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gppowxzpb.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/goeegfwjm.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/golqjhqww.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/grozkgwvi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gnyvvmjoz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gavqdpdvu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gvmxbxqvz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/giyqtwyqj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gfhtswjao.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gkjffgooi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gbpryqgql.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gcrpixitm.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gfsjwmcot.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gkdpkpkwr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gbtnaghuo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/ggtnrgypu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gnvbhbtrj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gkwsonxwf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gdytftacs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gjrrihoiw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gkpgewgdu.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gupjnjmvy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gmwejlnhx.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gdtstahrx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gxjjaqetn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/goroemyxe.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gqfbjacap.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/ggjmrfcur.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gnurerrhb.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gzhwswjft.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gupflzers.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/grynuftoi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gkhavzlos.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gfyjreaxc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/goyjrctxv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gvptzlenp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gztslrsjy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gzhgsepsw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gctwxfqmo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdqwnaruh.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gzywrrjsb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcdhxxyqj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/ghbzbrvyo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gjdnsmkga.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gnfewszso.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gooetojif.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gcqgkzyyz.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/glmffviqw.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gllsviiql.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gftqlkzfm.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gyzzppcpq.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gclyytgme.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gjgmjltam.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gsvalsqkh.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/grrbziwll.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gxwufehew.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gksduawif.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/govzbznte.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gngqgpkvr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gqailhbzp.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gvppcoops.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gyndhhuzr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gsfitrciu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/genrmuoid.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gpmycdwoe.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gdnvkijep.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gpywosjbp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gdufmiwyu.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gsfabbkru.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gfxwmnvuu.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gpxdmnwzu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gzbiylefn.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gcaoctuzw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxuaiucpa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gujmzvzvu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/ggpynfxys.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/guqokjbmt.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gkaqokhza.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gergevlmw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gicyvuhlv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gumoklkfu.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/ggbvmwlyw.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gzaanlptx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gzbetzylq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/ghxpvhytp.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gykcnrufn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/ggqbbnbtq.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gycumazvg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gppxynwlb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/giqoffpyc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gyaiocyhv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gfkvvkzgs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gflkiectu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gmkdnfvxd.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gkshgrmjb.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gmmqpemdu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjeyyddev.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gufokbtqm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjqecofnv.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gdkgwxnip.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/ghmmcbtnu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/glbczvwkv.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gwcopypgz.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gdheepbwp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gibqfetmx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/ginvywegr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gkokrxlgm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gtutbbdyg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gyzdsplcv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gpffgoxke.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gyrvprpck.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/geeatfumq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gcbyzdjun.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gagddqkxs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gilhzlobk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbntfyrus.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gdvvvsflr.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gicqqhheh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gmgrchiur.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gnolpquun.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gdyzkmxlo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gzyfwqacr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gaaszslwj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gsdvfrqpv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/glndjgiko.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gpypazxoc.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/getbiutpa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gqvjkpmay.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gtobcljbf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gjaxfcfwj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gswwadhcg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/ghddggsje.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gzntnvxbz.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gubhrnyts.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gdludsvtp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gconideoe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gofgrgtnh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gfjpierbv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gsgioqrdd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gokqsycmh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gzuhnvjto.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgixcjte.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gkqelsuzm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gtmkztkvb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/grsvfttpu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gxrpfqcby.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gtpymckap.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gvdrckmpf.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/ghbhkhcmd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpnwzkhkc.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gxcpcfars.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gjysjymbt.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gemcokysi.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gumaovpnw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gemhzerig.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gfrudtytq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gxxniqqqe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gxrxjeozy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gfweuvbpg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gwvioajhb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gatezphrv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gwhegnxid.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gywyszeto.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gxabbpuvt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/ghrdlnbez.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/ghrffeeys.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gsmtawrkt.sHtML


<!-- 参考信息 -->