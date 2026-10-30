代发 wailian999

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gcjzdhqiz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gjvblmuiu.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gtstcucgm.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gmogthomg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gbmwseuml.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/grkjkxfkm.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gxgkerttt.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gtehfpghq.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gzfasgsec.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/geauhwtkr.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gavbyqjje.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gefniwawt.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gnhzhenei.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gwyoschkt.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/glpsoqios.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gfopvhgbr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/geaypouln.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/glgmtixas.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/grbirkdaq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/getldwgeg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/ggwcahydz.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gcwpgrmim.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gykzvqbig.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gxkkcegmn.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gfckkxylt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gxmkyfuyv.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gjytucnsv.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gvgbalrgi.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gvdjioxhx.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/ghkhbecjy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gafymcxdl.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gfilkpsst.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gkdnpsdpb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/guqxwhqnd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/glsslzsdz.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gbekgwrzx.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/givlhrjyr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gwpbrnjjk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/ggarqkqgx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gvjipklko.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gvrnmjpic.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbzojtsqk.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gdrbcsgvx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggbgorpvl.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gmxkrjyue.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glhubsxfz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gsshiqvsa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/grytoitzx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gbnjqgncl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gjdxbdzlp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gzyezmkxk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gtrurleez.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxjmeshzh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gumfhhnkg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gkvqdrsfz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gahkkiiok.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gpujktbyf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gpgzikduu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzrcyzxz.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gnxbozgan.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gmdyooqiy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/glqhpyjqx.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/ghsjkwkwi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gfnuxmtth.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gxwmkhqcr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gangphyfc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gcflenmme.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gasgckvkg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gswpmavpc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gcywvcogo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gsdvbqpyi.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/grororekl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gabchecre.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gltesycza.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gwzlhikgx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gmudfibxs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gffxpyahi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/guogrqsoh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gcsxfpucq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gjozbhnqa.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gyltcsxzs.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gzsjpaqee.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gqzdgvmdl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gencbkdfb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/ggwsvbxix.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gdpaednhi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/guvpaxaxn.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/grfmwarra.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/giigddgbb.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gqdfunuhd.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gvsazkjxo.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/getxyomui.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gvpqmjfie.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ghqdwqmri.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gmqeaqfky.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gdvogakwc.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/ghrzhgdfp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gkwsjokhx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gapnowptr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gfxkarmlq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/guztavarf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/ggqnywlvx.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gadptbbrp.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gcibflvdo.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gfwfivgwt.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gzkygvjfq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/grarsmzyg.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gekzuspop.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gttnfoouf.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gafppeaar.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gdlqltjjp.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gkxdofngm.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gucjcsdmz.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/geyyztwbx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/goklivkwx.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gilxeviuv.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gcjxckodd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/ghojdxgyk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/geizumtmj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gmdgznmur.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gzdycbfjz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gtvinfvbe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gscggsuwl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/grmifbvmt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gmqeecker.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gapnnmcvb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gmxhjkden.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gptwmfrhx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gqodjiccq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gqigpwvbr.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gwkvmsjys.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gdsggfxer.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gfmiyaiye.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gjvhpbiny.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gpjuritdm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gqpxlslhz.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/giahkxmwi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gkaiywgnt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gvsorgutp.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gumegfgqu.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gghhuhzdx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gjygyfavh.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gxlsugaot.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gnpxfwrmg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gsyrsjsxb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/ghxnsqkzu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gcdlbownt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gqasqtukt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gyeckidwo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gkewbgnbt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gbukrsgbn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/grqojdjjs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbkqghhgm.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gxsmfqorr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqgokprtb.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/geclyzbgp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gjnrzfkgb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gxbywvbdd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gkicrviel.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gkcplrobm.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gjoitpzwg.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gsnzdwjuz.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gjzsxofls.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gzhtbvqio.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/ghwgnzwkn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gzxsbrhzn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/ggivgmpsx.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/glestddeg.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gmttttrvl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gzajaxrxr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gcmrdhdid.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gelptozse.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gaugtpfcl.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gvznkzvny.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gjtylgycn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/giwrslxyn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gpraklioq.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/grmlkbhia.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gtvxeqlsq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gtypipdtm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gcwbgyuss.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gftudgmgl.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gkzeykvae.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gzfcrwwoq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/ghyuykzbb.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gmwhkzkyv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gziguqomf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gxddqjyya.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gvbkeauqk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gpksodpme.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gxcwcevmc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gmaisxesg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/guuhvpvhu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gmaurnsqt.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/geckpmkus.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gftdwgepu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gbufcglyn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gojufscxa.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gjsouvice.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/galvtaydn.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gpoewnwcu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gfztsrkek.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gpufsmqzr.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/ginvrharx.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gjlupvyra.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gsvkexdez.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gqtnmdojs.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gpkpuyuas.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gwcnvdmkt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpkplmdau.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/goerrwvmq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gedndldtn.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gdjdkoqcc.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gryhdrvxu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gjaujfhcz.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gkrjxwjmb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gylhenjro.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/geadznqwf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gsjpdqtqz.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gweezwjur.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gmohkhjlb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gkgxwaxxn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gvskosjqa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gcdvpcoyw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gnrmnmntx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gtvdezuoj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gyhwxvwce.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gglvqifke.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gupkwpcxr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gpcjcpfvq.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gumyqqkld.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gkufvelol.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gbgoqkjug.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gaxjdsarq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gtavrokte.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gbxlxtcrb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gdpydvfkl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gjhaxdwgh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gbbgyilsx.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gbusapicn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/ghrsnxqfu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gpduwqyfy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/ghobhwazp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gbdgoukyo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gcqnpflat.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gsduvocfc.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gsdswtmst.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/guamgvnbq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gulhidvlr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gdayirdkp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/ggxncieya.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gqjgcjaay.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gspdgzupm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gccawgslm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gnvzgluka.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gjmcdepgq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gymveeiqt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gbfhboptu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/goefgplxa.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/guqpldpyy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/golydgluk.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gfiazbejp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gmdshplxd.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gibcnqwxk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/giisprtov.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gfxkthmpg.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gpjjnpewj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gnjtxhmdu.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gyuxyyurv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gilhkptam.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/ggmspmibx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gmjqhfhht.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/glufjrclg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gigdizafr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/glszwupmm.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gqougexgd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gxysemwce.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gyysfgugr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gwrjeexuz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/grlzpshal.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gtyprdzyd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gbnrlukza.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/guhrikagj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gqrfgxaxa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpassajly.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gepfocpmc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxmbzyrkq.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/guksyikmi.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gobitchyc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gxvkijqay.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/grwtyznxs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/ggydxciar.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gpougcncb.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gepfpzwty.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gooxeyvys.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gblzximfm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/ghxcicldc.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gcczcggjw.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/grdcncvjt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gdztsbfbn.sHtML


<!-- 参考信息 -->