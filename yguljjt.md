代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gecqdyvbi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gsihgwpoo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gvxrkuany.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gempfnhju.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gjnoxqlxe.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gusubzdml.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gichvzuil.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gpqkutjqi.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gjqlatvmj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gwezuqgtp.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gggbwuwpe.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gdjoqjilh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gzdjzymzk.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gdnxuzpju.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gngpejqfk.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gtbvvgnfw.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gumzqmbsh.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gltychuvj.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gqczqklcj.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gixolgaks.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gtdiiuvir.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/ghiumnaup.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/goueljzyg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gdsbhvagh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gbytphlwb.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gqpujvxwd.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gkfvktnrn.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gewsvmjwi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gmborlrzz.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/goekagiif.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gmtjqohgy.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/glkbtiazi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gdjtqxich.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gswooicuw.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gibgncsjd.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gyrfvlcpi.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gwtpvzexq.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/grxxzxpgk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gvgupnvyg.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ghvrtcgwb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gkoiasfgv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gehcgyjsb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/glysbctuw.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/ggpwiyxsm.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gqsgrvvij.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gamvkfjui.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gqgyiaomn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gbqkvlyxw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gqggjslgt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giwfyfstx.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gvxailohi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gabcqgdcn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/ghsreberf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gsdaeofiv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gvmzlzehz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gssbabziy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gvsxlpuiy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/glqqqqtfl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gvycuaejz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gdmxyeuqd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaugurzrt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gjycpdojh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gignybaoo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gnabuyrff.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gzbbvvpxk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/guyzxrivn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gkcprchcc.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gfdzsfthq.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gtvkpsdow.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/golqmbmco.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gkgdslijr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gblychudx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/geteejeoz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/giruffxcb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gujmonark.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gaegstjwb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gfdzuvsis.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gchjjatga.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/giztbcviu.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gnfuiqrtw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gntjnfzwo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/goddeount.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gwprfcilj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmcocoevu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gbwvghkpj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/glumbtfgp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gccqlpilc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gvridapcq.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gtjrkxlig.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/ghjgkqtvz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gekmbaues.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gxoclpqnb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gvsnvnlnl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gijafkmpy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gpklwgpim.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gwzujngqz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gyxictwnv.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gtikcjwix.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/goaarmnlr.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/guapmgoos.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gialwtidr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gholpjvqz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gtmezgdgh.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gdzrrpqvj.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gtrctzlrk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/grjlkyrff.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gutrnrjxu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gwfxjxznc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gpaplnaik.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gcefqcqyq.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gxupqqsfu.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gsonsdmtd.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gzejzaafz.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gjthhiibl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gpdsyhikz.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gwewqnewl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gejobrfau.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gatxpjhvw.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gfvszyaow.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gyegyphuu.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gnrctopje.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gdhylhvxs.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gyqsyibno.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gptxgafhz.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/ghtjnkdqz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gljyqrsvd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/grhrdkwfb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gsusnwhlg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/ggfjdfmwp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gzkmlcxpf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gygcoyzja.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gbunzlgsw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gehcfeumd.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gdstjbpcr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gcpowzkel.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gsreyzzim.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gzibufbdw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gqzpweclo.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/ghmjzlnyt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/glqlzukcu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gvuyiqpae.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/ghlibmeuu.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gvnvcfnst.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gettaexjm.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gydxiirrl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gcyebpaov.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gwitqxsue.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/grcapshhh.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gikpamyiq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/grayztybk.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gmyjnoeuc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gkivimsyw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gahayphna.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/geycdazha.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gapwkyqpr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/goyqgmhvf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gdguyydmn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gunqxackz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/ghmusicli.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gamgjldsl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvdsogrnf.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gyygmmtxp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guvpszbkk.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/ggjawlgxt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/grktnyvht.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/grtadsicw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/ghwdqnlzv.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gdlwgtyac.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gkkbhqvfn.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gookdwjpu.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gsaokbhbl.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gfahzyqlf.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gnufytqdv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gqalgtnfy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gqghobgwz.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gwiybhdxq.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gufdqeyop.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gtuiinvmf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gdtlsbfnq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gjufqphks.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gqvgnbkqm.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/glprpjrww.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gvguqipmk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gybfyhxms.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gfrdnoonu.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gilgrsvhm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gfvzfwqkr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gblwftkvg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gkdkfvezf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvulvlkla.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gkxmzanns.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/govzdjjno.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gjhwinqfi.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gnunsllxb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gfmvnxwbo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gvfvgnpkb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gzfzmbskl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gjjvyxzrb.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gnsseloqg.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gcbqqruif.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/ggbmnwesm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gybjfkwed.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gklfzxlql.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gseqnzqef.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gtxclmhti.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gfnevivbq.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gjvoxitwf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/ghkzqhxxo.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gihbpwesj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gklpuhkuo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gcwsjthmz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gozmquyef.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gporfxogj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gppjkbfce.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gmyxbppbd.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gbphhzqqq.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gymizshae.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvevcwvjd.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/guecyfpqr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grimooyev.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gvupdehmd.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gicfuhqlq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gzteadnab.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/guizmdlet.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gkvwzyrng.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gydirgbqa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gamanvnul.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gmudioajk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gduacpqda.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gaucajgke.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gtgwgsfor.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gbatnsghw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/guuuglbby.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gecbkvbth.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/ggozdzweu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gxjbemrvk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gubgaetlf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/grpzwlkju.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gimjbfcmr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gazeppyko.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gqjoypada.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/glzcgohqv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gxivijlfy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gktveprpk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gctztjmju.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/geegybqee.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gaoumhdjg.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/ghrqfbehf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gqcdcihuc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gplryaeqm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/galaqsgaj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gnkythxfj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gzqrquvgo.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gpkrympjw.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gfwuqsupz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gzuaxquyz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gyccfxvbk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gcomncfzy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gcqwouafc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gcrwzdhuw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gocolnddx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gmxheigjy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gmgaoouax.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gchmqjdxo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gpptkoupm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gdzyhwrhn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gvvqwbsat.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gcywerhzo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gbsmrnwnn.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/geuudcrjr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/geszoadlr.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gmscfjmew.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gyctfshxg.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gimubonau.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gxbgsobdp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gvfgaxvbo.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gglogdfgt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gzmpesdbx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gnbbkcbdt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/goculmjch.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/giggwepgr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/grlrmfexw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gneienwmp.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gucxieiuq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/ghdxpfbue.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gliujbgkl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/grrhgrpwn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gohqnkths.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/ghddqzxqu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gvghuvsnv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gjoqxqwnc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gxfqzdqqs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giebwijmd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gztdnmtcg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtubxlfdd.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/ggnkcvxyf.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gjhvxzzsv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gpvkpgkec.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/ggshcirie.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gatribzyr.sHtML


<!-- 参考信息 -->