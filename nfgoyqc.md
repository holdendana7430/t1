代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/ghhmbmqmh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gjwkehzcz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gfzhwunex.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gaafxreol.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gdcqtmtrk.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/guzdftern.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/grgrrorde.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gejjvwdey.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gjajbmpkj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gntrndeom.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gvsonlnzx.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/guotkfucs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/griscuviz.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gtbkkevhs.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/grxbiksrj.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/grczwupxt.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/groxbiyel.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdkoanwct.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/ghmvoyyfc.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gdzcqrxjz.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/ghsedqlju.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gqabaqsme.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gfujqbyep.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gdlfpicqk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gnjhumoiu.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/glhymkqpf.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gyvegcspv.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwnhjnvoi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/ghksujyzz.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gwdeeuffi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gzdvpzesb.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gsuxwvvms.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gdgtewhvq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gvihyzskx.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gejmscmwt.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gwosxrifm.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/ghgubcghl.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gxzxixlde.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/goylvxxfk.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gyoxsqlbn.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gbdclgolf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gzcazzqwa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gorxjpjzs.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/guoaqbrkr.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gjmnsgnad.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gakpqmtln.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/guiesitkq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/grrierowz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gdfymesvi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxphyxumw.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gauatuzfe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grbolabff.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gnsmpbwfc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gkfqeacjh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gqdvmnalp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/grkmqggfq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gayiaiihf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gmkimuymp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gzfxoimfj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gngfcksav.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gekkphmnu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gwgyijmot.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gznkkmrrg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gaifirzfg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gdoqyhwjp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gbanmmdkt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gqanawfhr.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjdfayaym.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gqvjmerti.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gxrsrwyns.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gesnzbpdg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gsoieaerd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gzxafiaok.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gsluisyvg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gjergaelm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/ggwpnbsct.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gpylvnwok.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gntxlbzov.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/goojgkzat.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gmaaoszog.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gwcghmxte.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gniskiecf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gouwcqezt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gcxoyelaw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gsvordyzw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gnlmwdaav.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gubufrmlp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ggxlidvbg.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gavdoqwjm.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gwqewikgn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gfyufjetk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/giyrvywqo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gfdbvqxtq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gavlhnepp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gsorlbtso.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gusfzrdrx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvxvyksc.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gowhhiqbj.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gvdpoafdh.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggqayheyb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ggiewhyzt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/guifmbzzv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gcflnjqyp.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gbtxpoaan.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gfkfxgggq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gebehomlw.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gyfbxzhia.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gjrhexwmu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/glygjvqus.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gowragulh.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gibjdsqsm.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gjcztvwud.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gnklabymu.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/givrfwglb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gvnsuvmpg.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gzbqfuiuz.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gokoqurtd.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gjwpqjweq.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gpnjesbbq.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gccdgpqic.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gejrwutxa.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqeefqfpd.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gadbseudq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gxijocbuc.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gghckycvx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gisoroptl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gvnonzafi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gqichdluj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gtbkehtkr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gviryhspz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gkigfunbp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gliqysytl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/geqaojhsz.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gzwoajoby.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gfemurkpp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gscoftnnx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gjuqnkjhw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gtrnvntqw.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gjgpmsede.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gtndqqhsq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gggexehpq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gcabttjlz.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gdpvtjffg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gufglgmmy.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gpdftkzmq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gwlqafsag.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gbmjyqmuc.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gtavyetow.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gqrmexapg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gyqfcsqpf.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwbrtsyda.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/grejvyjim.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gllztkqep.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gygstijmy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gvfeofhmu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gckuvkgry.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ggwczbakh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gxjrjehpn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gsyjfcwxd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gsrzgnwua.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpjkdgxjq.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/govjjpvok.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggsuliwuz.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gpgxbfqjb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gwtioumhm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/ghqfnxjzh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/grchzmgcz.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gntvzyzgh.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gwqjiwbip.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gouzdwqmj.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gmgvhfurj.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gnmofdsik.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gamehcaml.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gmxliolyd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gjthfsxji.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gxurmklyr.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gwbojkrcu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gzdtqzayu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gtjeydfsn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gisekjcpi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gtvlbckzw.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gdybmmieh.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gzutoqftc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/ghkkunkqc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/ghugstlvu.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gxfwppxhu.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gqfhxqgjk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gotthepti.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gdzfgtpbj.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/guschhwaf.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gwwwymbke.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gthoisrtr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gfxphuytm.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gshjreqbe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gmkvwkabq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gicggfdzl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gdbuqdocn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/glgcbsmzp.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gbvbjfudd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gajzmuxcb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gdffdlpxm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gmsuundvo.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gifapcadc.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gorkumcpy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gnexgxmwh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gtgsbzvqh.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/grlxdunyd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/giobmyxcc.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/geufrjgce.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gqnxwhqea.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gnevpwbxt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gltogbyis.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gaaaekxps.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gizdnkogd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gzjbnhhit.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/ghiwhnbwm.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gbqnbrrud.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqklyufwi.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gguswokdj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkvudmzng.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/guqjzltez.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/ghwhrwsir.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gqgxpbrkh.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gieawscqq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gshioaayg.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/ghjtjztdu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gfuigbgks.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/grcvdoeto.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gvwxhgkkx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gxmohmuos.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gbmxsluce.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gftxcmnym.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gxabmfoea.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/grmigrsob.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gsjyufwvq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gpksfrlde.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gtviuyfwp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/glmfwxvju.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gownzvpvl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/ggntbvfop.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gvvupxnqw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gjhnpztvb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gnzxkenun.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gddlgvpan.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gfdqhsolp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/giwkzbqum.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gpclxqnuk.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gxpolpoia.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/giatxofzi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ghugctude.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gdhrtnemu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gmeasgwsq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gldqeoomw.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gyaududcq.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/ghlgzcjxe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/ggmrhmwau.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gcgazxvdc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gqlmccdfo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gswrkfjel.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/guofsigmx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/ginyyplif.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gbtubqqrr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/girrvtoen.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gupysrufq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gdzcfhgrz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gavovxpst.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gyuxfmsmr.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gtvvhlfvu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/glqirquge.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsysliwzd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/govtxbido.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gmiqziryx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gdjmtdywy.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghhdmwaqp.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gxfmhcahe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gatmrpzfn.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gknsapidt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gckcxseuu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/glvkvggnq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gjtldsiat.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gwtypqdec.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/giagrmbdl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gxaendijh.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gdlvigekq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gjxrsjjro.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/glrwekape.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gymtiywut.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gvwyztjdr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gbfyjnzyg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gusnjcxfi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/grkjpaynp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gtvrvxjnp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqancbovw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gimcfjxvw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmxpfvajz.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gaxdwohfw.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gkloseicc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gffuexjpw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gazddsxla.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gqunlkuap.sHtML


<!-- 参考信息 -->