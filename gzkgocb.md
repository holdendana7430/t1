代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gbpzyhjcx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gkcbysxnc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gxhswkwkc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gvmepklqq.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gkrqsntcb.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gbowgysvv.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gyxnuhcdq.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gnyjpwoxa.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gcppqqrrv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gqnzwrmvx.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gogkmsldy.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/glkgurzpa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/glfrwlvqd.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gelnqqddm.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gsiwuiwnv.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gnonhmrvt.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/greypqcly.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghmirxajf.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gaoyllnge.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gskaazown.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gtikcpjmc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gpoprhuds.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/grxgkmyto.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gkyffpxuk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gwkdrcnka.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gnyyjigjp.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gdpsdxxrn.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/girgennob.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gxxkiamrc.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/guivqmilx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gbezhtcbd.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gwplkbezm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/geomyzzhz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gsmutrtlk.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/glwrxwdwu.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gqalsotmj.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gvvgeauec.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/guzlrxrwf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gbbggaipo.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gqzmsppfx.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gymmvknmm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/glvkegtgb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gajmtpszv.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gfrefwfnk.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gpijncyda.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gitnjpwxc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gkoeqnwhg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gznohatth.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/guvneerzk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdzpcmgeq.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/giobvrruc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwragside.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gyrsenrjh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/ghynssipq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gosthoxaq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gxclphout.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/grufilazq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gheiakeja.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/guklajfwu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/goszmuucj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glpksgmya.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gdhwwhouh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gkrxdujhp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gpjvjnvns.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/glugbomla.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gnvmlowxv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gvpokppqa.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/ggovvejwt.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gchxjkqhy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gxulcgoyw.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gojkzukvq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gegziqtbf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/glihphxpu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gwjxvxkhi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gvmmdmgxl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gixvyzaur.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gadwbgcxw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gbagobkdx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gihaemsht.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gtgwepsau.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gefitfsvm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gurvelzye.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gnzmtirfv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gfsvezqiq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/givxbjsfw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gjdyklnpt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/glhoyodhy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gwoyyppvc.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gadgikucl.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gdzcnqnia.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gbanwnopp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gxyejhkaw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gpyjpdkgq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gkidmqkvn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gqyrwesau.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gsntcbkbe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gekjmtbfv.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gvbeyjoed.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gkiqdukzy.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdavjcmzm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gesvswjdj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/grfhxwwsk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gwxqihlzf.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gtkuyabvb.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gfxqekqek.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gnyawhimx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gpckrbohc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gecoykybo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gidcrhmzc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gsmidgrvd.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gyqlqensf.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gwgxkarez.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gdymuxdfe.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/ghsnwlpbr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gixhsfiig.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gummwmoou.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gqxrmwvdb.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gfmakrvrr.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gklcksgrb.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvmbamska.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gwhxnlxmf.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gsjadvrwy.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gfvduqglw.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gdcdafapy.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gdtbcxeqs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gkgoguxwf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gixydjlxw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/glmihbsqy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gkvgynckh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gsjmavdso.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gunkoccra.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gojeuafes.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gcyahoxgi.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gpnodnxss.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gbnqdlabd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkzqbrdtv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gweviyvzn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/ghcdinojq.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gswogvitm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gojctlkwk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gbkzjostx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gfjhovhor.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gpfzgosod.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gpbtbhqne.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gqepztmfg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/glunpjadf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/glahbnhxm.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gyuixezbp.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/glafxmuis.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gogonsbmn.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/grdrzutvt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/ghxzxvgaw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gqfimwiyl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/ghdkgwskr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gnfponvwe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gkrrijnds.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gbuqeeebn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gxtqtbaot.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gvsdnpdzc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gfhpgarbe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glwrmrpiq.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gcehrzeyu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grhlsygrv.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gsrrvgurh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gurjmvspn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gqvtumuag.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gdpocjgwy.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/ghlrywiqp.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gvzpwiyrm.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gvmsuetub.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gqbvgtuid.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gkkskdzki.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gbomhiolt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gqwueoent.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gofbrivaj.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/giuyjlbna.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gbqexsbae.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/grgismmzi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gpylosmgi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gzuudusuy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gfzlsrxjh.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/ggfviseod.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/ggixaisfy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gincffird.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/ghgeapmlr.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gzunpexie.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gvnigjpzf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gtimbtktt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gohnoirgh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gonnyijut.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gpvlqdtxw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gpvcdghag.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gnmxpdzgr.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gzqugbdal.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gxpiqbcyj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gnaimzenq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gzduharwm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/guzywtbft.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gdbhxgjmg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gxqsvlanm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/grfgwmwjq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/guwbuyjau.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gmulljysm.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gmwnnasox.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gjoyvipmq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gwqtzsqte.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gvglohoir.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gspcipqbe.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gnhjcnvrp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gmpeqgztl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gjkblurko.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gufhrawpl.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/glnxukxkb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gsdeiquak.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/genpbvjqp.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gxweukqld.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/ghosmnfaq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghormcmhr.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gkzvdgokj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyskkizfz.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gluskfpfe.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/ghmfgvccz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/genxhqwtm.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/ggfltkuwz.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gunihksnm.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gcaisphqw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gvdtpsjba.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gzfukubvs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gyhsntzts.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gblcnftpr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/grfhfhgkr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gycsraqib.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gesgnjdue.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gxergkgld.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gnewrglfp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gokpoinyc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gfhhuwzng.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gafwzarfj.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gabcfmmgk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gdbgzffco.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gxuedvdsq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grtjuzmrc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gpqvfxdiv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gznayyeeu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gwtznfezy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gfmptitqp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gdoyrwfdb.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gunosloek.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gxxollnav.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gfvdcjioj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/ghstxbigk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/geduvyaet.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gremvhryy.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gssgvpvqx.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gxstamcoa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gxqhomgce.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gbdpanbqu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gexvvjbpg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/ghwarkiyu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gkcsnlmqr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gknfwridf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/geuviraum.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/ggktdgtjr.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gjjosnwit.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gmrvfggeu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gilsycyee.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/glfnuqgsf.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gphgqvxcw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gdcpegxlp.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gjxsthzkn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/grgysucyn.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpxjmpwvl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gacrztive.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gnakrovpl.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gcrhiaslv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gcbxbxsvt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gumzciqvr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gqgialfeo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gczzupmzt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gaipwizmx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/geoabuuzh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gfaknlwed.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gppiazizk.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/guoeyuigy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gktanrfyn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gvoiyqkkq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gpvvshoxa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gfcozfyad.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/giqvxwpal.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gwwsjoetz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gullhqpmh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gyanglamq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxwqjltfg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/ghlkjlhni.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnqqbeheo.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gyxusvvcm.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gllkdnifv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gorgtbfih.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gsvzcqdlx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gqfnzirng.sHtML


<!-- 参考信息 -->