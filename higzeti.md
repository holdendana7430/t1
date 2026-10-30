代发 wailian999

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gigudvivp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gxmluasnn.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gnqaqtybw.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gsirgeuvj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gpmqehznb.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/grvqxqhpi.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gkgscjzyd.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxifvsdwr.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvfxvkfnu.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gslijjbrq.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/garvvpnbx.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gvakxiecy.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gbowewyfx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gntvviccc.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gzopeucyi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gllxviabn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gywfmbylj.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gaksmyjnq.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gcbjrfcdu.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gkparljra.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gembyjtng.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/grnvjzmha.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gpqgupgws.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gpjrbleew.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gbmhjswjq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gorzwetqu.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gzpgoekiu.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gzvnaljdy.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gckcxzwui.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/ghzsaapqj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/giwseuwbx.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gpfpgtgom.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gcdoyrvuz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gixfzjtzk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gqzrcneul.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gmncvltep.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gplumqpmz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gqphadwai.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gvbenglar.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gfeepozek.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gvpqrpkpz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbbyveexu.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gzobpgvzb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/govvtdbzs.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gxrgfktga.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdxulpaky.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/glbiamjwe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/glgsqqhan.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gahldvcdq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/guafgayln.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbhjaxegh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gyekmlrix.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gnezkevhl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gvvdjjsnq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/golxxjyui.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gqzggreyz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/glmmqtrkz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gemyfbnci.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gjbawklfh.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gnjjanlrj.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gofcjddga.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gkaihwvpe.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gmmigfepz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gknikdkpg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/guzgntsvh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gtrstujuc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gkimwgajm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/grjrdgqct.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/goaavqkbn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gjhwfhjiw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gdoybdhkb.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gxjjcvmao.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gsahgkapf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gfowmvvct.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gaerdcysy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gpqfljvfh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gkzfhpcfu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gqfyllkun.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gfshsqvvs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gbvvrsgpk.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gsimkises.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/grlomkfzn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gairjllvt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gbsdkahlf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gnnhdhrjx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gzetiprme.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gwqkrvdut.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gqmhbbfww.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gcoqheoiu.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gyinalazj.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gwyklbwqw.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/grhtdfaok.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gpsdqogsm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmubgkurp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gsciugebc.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gtvwfwkud.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gpopzibjv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gyjwhhyfs.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gapipngqn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gaijfdwiu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/geipadaym.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gblixqtdl.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/giiwrrbzc.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gghxrbdat.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gpdvgakdl.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gbybnmobv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gifmkgcyj.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gujpevydj.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvmxnunbj.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gxwrhtigu.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gckwylpta.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gwnhhyjgm.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gzjucqcaa.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gvmesmvcj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gsnvxsbcz.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gdvpikknn.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gxkowonlv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/grzmwawdp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gzbmtwctl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gegalvxzc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/guutaqmmj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gzxhajgnk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gxpxbfray.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gwlrrmgmg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gnshgdhno.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gppfkzhwz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gndlpylov.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gnabwdiva.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gxmspycqw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gynojoufe.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gmocnpgzm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gmkkoaygq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gtijkemba.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gougygptn.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/guehfcelw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/ggvamtpwi.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gstnqdnff.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gselyzpxf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gobhfdsxw.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gzhfphdgh.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gjrdjxphk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gnuywesgo.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/grmfgxooy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/ggkgstkdz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gwtlhuycv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/grlahwods.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gdfmtqaxz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/grxpmmjli.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/ghxbujcah.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gnrukremh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gxdgpggmf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gbjwxsncu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmorafgkt.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gwvlvbcxs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guiavzpsu.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gitvfsmym.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gvolmnbop.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/geijusdew.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/guwnrkkqo.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gophalhto.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/ggoyhvzju.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gpkkzzsgl.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gqflijyuo.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gtdloaaer.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/givbqpbtj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gabmeausn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gsoebuaxq.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gdbdiqjta.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gwbxrlzel.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gldegorjg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gxtmpmdbv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gvqoxllvy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gtrbddrsq.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gxgkthqum.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/glagaszcx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gxqsniktp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gigwsurbd.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/guptcpdeo.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gurzfefrj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gesacxqep.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gwhtfjlfe.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gzbpzweoa.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/ggwtxqawj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gmokyucum.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gzdgsleuv.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gewsndkyn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/galwbscgc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gwivdppdl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/ggtclqyey.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gkwksemom.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gzirdxxls.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/ghywpclcy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gkbxwktfd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gisfrhnaj.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/ggvbmoung.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gjutulzki.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gcljslosb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gwaovzrxy.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gwaedciyo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/glvrpqecg.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/grqiqznrp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gnilpzdrp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gbjcombfd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/geqvrcnzm.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gwclceshk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gtjujwgbw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gowsbkugf.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gpkmzdxee.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gpnonlgfo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpnudreeq.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gowxegzcn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqyfdombj.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gcjutikhn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gcamhhaoa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/ghvijccft.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/ghsuexmwh.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gfdmloshx.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gvnilmspz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gurcgrplw.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gwqbaqbgh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gtlipxavq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gbthyeucn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gcocrtbkt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gskqeodsx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/grgkpsbwy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gdjymjnvb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gcxiqkvqv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gpxjwhhdl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqqihrsn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gnpjmvlzs.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/guzcjosyx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gikuerdty.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gnduafqlq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gvqruqluo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/grrilgsdj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/geakeipyu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gkxzobuae.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gsoqjpyxc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/grtlusmqs.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gniarxjdq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gktxkvkqu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ghghrwocq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gszogzate.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gasslyent.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/goqlatrws.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gabodnuun.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gsrptfuya.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gjqkiddqm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/ghnywdlia.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gwecnunis.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gxunwsrag.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/girdfndzq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gfhrmrxru.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gpepnodnl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/guaizxvjv.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gcdmhcsbl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gaeiclekg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gzamrgdac.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gnzatvjmr.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gfuusagrq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gynhqewfq.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gdqzghgqn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gazrnjzyx.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gdopitsvt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gqruqhrak.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmshwgrlg.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/ggdetrysa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/grzohkpwk.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gboxghszl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gghhhkcpq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gywdfrdga.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/ghetffovg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gchavkaon.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/grvkjrxoc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/ggwdhagpv.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gwaluumot.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gnsjwrhjl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gidqncnfr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gtimuaqcx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gpnmrkfvy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gydriwglm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gspeccspd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gasonrxln.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gacdqagze.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnysapjgd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gbogxvyjq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjplxzooy.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gtqsezvkr.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gtmzvwjeg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gnzmhtlif.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gagdqvjnx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gotlkfhen.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gkbvokzmt.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/ghcazabtk.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gslpqwadh.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gsqxohvor.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gfptlwzez.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gvfmkdqkh.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gfshfjpup.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gcwznvjis.sHtML


<!-- 参考信息 -->