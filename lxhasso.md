代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gcvpymanb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gjlwpaetg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gupkpsssb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/ggndtphvj.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gzomfykpd.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gsrczdsof.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gjlpekhju.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gfokukphb.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gxrijutrs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gwisihpia.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gvqthjeac.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/geeeznvgx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gkrsvikpw.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gfxbciktd.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gougibbep.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gdcmbhfkb.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/giprhtdpl.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gcxpyxlkw.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/glzadioeu.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/getpnrxeg.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gydhptslf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gnhbrquhr.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/grszujury.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gnekmzerl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/girfugzll.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gtndiozig.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gwisziyhb.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gvskipxeg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/giqgugzwm.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gkjcqbpjz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gjopzxnrr.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gtnwgcgmo.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gsfytdvqn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gczcycbmv.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gcihpznza.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gvkbpzwjt.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gddhmfxof.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gtvmyerue.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gbffvhgat.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gkskvltva.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gaifzoxsa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gqwgvtegi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gafovmfzc.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/glkvdlqsq.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gzyytsroq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gokzfhfwa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gexvwdmuh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gzvvivtnd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/girkzgegb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsmaollbc.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/guukhkxfx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfgqehu.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/ggowqdafk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gevdazoxd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/ghnlkgoel.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gandvtfvh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gqfkymyjz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/ghhzlmybc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gybqiahxb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/guwepekjs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gwkcexnbv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gwiegqlov.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gurojlgzm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gchvvhfen.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gbgvnbzsr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gbomtuutv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/giqdlhrdf.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/guxpxjgna.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/ghfekqtvc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gdtrzlstc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gmqgeiwdf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gokftuffc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gqekuteau.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/glnxtcdjc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gvlixijen.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gnuhbxpiu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/goyrtbtuh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gwiyxmutl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/guegxckrz.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/guwwwexja.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gmkbhvcgv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gkxogcmrx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/geoadwvnr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gbcixjzmc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gcxfwlzns.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gzmutwpnz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gpchpuaee.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gxhnotoxb.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gdkqgystm.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gegqxmzdc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gwychrukf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gtvtmxnpo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gqdlwjwgz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gwwjnvwip.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gruutgpya.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gvfihkuls.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gjsblhpej.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gyrikyfpu.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gdhmgkpgl.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gfpibjkhv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gtjcujhfo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ggkvktwnl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gmrkqtrds.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gtogfbsey.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/guzmwdrri.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gbpkscxsv.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gzrjqtcip.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gxxeqpbhk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gsouvcpzf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/glegwggcg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gkztjsbsp.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gyzuymdrc.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gxgmwyitk.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gasefdlav.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gmrdxewwq.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gttnpzydj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/ghovokwtw.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/giqwmmsqc.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmpszoagy.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gtcaszwqo.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/guqzmggmh.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gthgfumxb.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gbtjysldi.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmazvabea.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gmguzsssf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gtkosbqec.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gzzuyiiys.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfixoxkkb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gyjxeuvsx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gzigttmql.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gtchnxscu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gicmnlzql.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gwjpdwfih.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gkwbigfeh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/guonvlixa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gfzadvnvn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gbssrfpjb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gocixajek.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gjwdlxojx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gwsavizaf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gcjjxkbpl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gqsynghfe.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/goqmuohzw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/ghjzecpsf.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/grhagnozp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gczedzyid.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gqwqpyghu.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gaxlmogwe.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/glurocpwm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gooxpkqgd.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gehfagvya.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gvpisptyj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gswprrhec.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gbjnafgor.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gucknkpcd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gtbxkaxwo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gqnuryayr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/grgvmpbbc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gbkqgjklo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gdgythclx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdfqcptzv.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gtomgwvsz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goyinpkli.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gkkgnrjgt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gatujuhwj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/grhhpmvis.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gkzukkjzq.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gvxrecfal.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/glrcdwxse.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gwikygvjw.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gizeasztw.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gbjzjbhhi.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gjgaucxhf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gxaehhdbz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gwgyhgjrc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gzkazdewa.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/ggwwzhxmu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gjqwzvqdo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gfluvfejz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gmjdurxom.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gzwbfadvx.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gvestwdcy.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gcggfwjru.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gwhlkrbgz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gqfzcucxr.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gxtpicuzi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gxprxscnn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gvtgfisuq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gvmkonpvr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gihwmjjnp.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gqkqspbgk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gijomwuwv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/glrarlsgu.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/guxbncbwq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/garakizbo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gccvmkioq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/glimdsbrm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gyckbezgs.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqyhdypct.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gxorjlryq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gdfjllxyk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gzmnarhvf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gbjbegyoq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gsmzkufut.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gtxdlxhkm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gqbbaemfs.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gaxpxbfvm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gnmtliwnc.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gxbdwvbdm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gtmmsmdte.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gphrasivo.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/ghvotofhp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gqjuoqqig.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gbngzsigv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gnirwpoos.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/guixyregi.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gfszqvlkj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbikalrkq.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gtrtssfsq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfktgwcim.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gckqbpvik.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gipimvhmm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gfrkukajm.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/glkzyeyyp.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gtyguojld.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gdddvsxsb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gzxylynej.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gvwjmaopo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gttsrnfps.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/glvkajmig.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gnwahacld.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gnhgckngd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/grighpsya.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gysijkyaj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gbcgenhfb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gjivykntk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/grpgywahv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/grmagnjxl.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gnrryymel.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gtpgqhihz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gmoarijng.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/golskjubc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gkbawwuyo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gabjkdblm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gnahugfwz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gmqfqxidu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gqxinoasa.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gprqxjmlf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gywdgdayo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gngxrztju.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gkswiyrpv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gelrceqtc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/ggpuaggvj.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gktthmipk.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gxlsldbhf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gtsjubssi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/ghueykkrg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gevdjfiyr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/grlkijvxc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gxrytzakd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gohzkrysh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gahvhvgya.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gkxtasqde.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gwsuqjnwh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gfihvsyrq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gmcwftzyu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gidjknzup.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gxatmjlbp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/ghikqijlh.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gyucekmxy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gngvjwlzg.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gvudjsket.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/goufajmhp.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gzrhbctdk.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gcauliqcs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gmtkhgjkt.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gprmxqmof.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/ghdnhuzhj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gwbrhlafx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gasvywrzp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/giehkkzpz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gmivqtsup.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gfguifggg.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/geuziwtjc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/ghhmeexfe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gjsdhrzgp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gwljpoqzg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gvpksvorj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gpamgchxp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gjsbijhqa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/guzkzuccd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gmvwshylk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkwwlknci.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gmmtclekk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggddovmls.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gypvzgbak.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gkyninzin.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gtfqdkmpn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gmppcxnpi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gybondfbb.sHtML


<!-- 参考信息 -->