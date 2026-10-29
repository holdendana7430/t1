代发 wailian999

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gjuefjsyq.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/guhiwulqd.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/ghpptskve.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/grcgqcxxi.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gstqxmpps.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gqasafsyd.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gczocokoy.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gecnjdpnm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gczqpdtgu.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gbaukdrkb.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/ghzbmcmqd.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gdlavymjf.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gyurahwzt.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gksqwfmue.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/guddejrbg.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gjytiycft.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/giktrwfnn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gciztgvhw.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gwigxzkhu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gmzqiqcuo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gwrtcwxnm.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/ghqztbtcm.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gjbikcsot.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gtglgdqcz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gvhxwlnyj.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/glcliocxo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gekcqgpoo.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gqozdryxr.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gxbuoudmc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gzgsccgwz.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gxxhodazs.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gdcljkwap.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gshajvwwk.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/geprxvfaq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gxarlkvqv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gwuspyhjp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gvvcuekyj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gaoxcvxne.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gwtyswjws.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gymiwzmjs.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gmtvgqnam.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gkgvvugyh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/ggwxboull.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gyygnhxlp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/ghvnmbqsu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmeqfumuv.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/ggoqpuzkr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggnotaeuo.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gwiovysfg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gfutevbjc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gksnmcvvf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gzldnjxjg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gpnpvhejf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gqhxbtmtv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gjligftju.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gdbeaynis.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gwnbsjrur.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/glytigvdk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/ganlnxeey.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gzfwfqbgn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/glyzuenvr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gbhoqoldd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gvpjufkhh.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfogxjugk.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/glvbncvmv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gybzljsqw.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gtrjcsgbo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gmkosiyhi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gzzdusbqd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gmbduzkgx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gruehxilk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gpwicqcyi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gbeyxsjub.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gatvmfdle.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/genkjhxrg.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gfptcchwo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gktfsodzw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gubbtaekn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gslukmepw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gzjabsxjw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gjwocucxf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gfgcrifsk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gqecarkak.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gldakmnfj.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gocfiviud.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gwpkkykut.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/guxxyijna.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gnedmtlbz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gybmncmjy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gkszuhbyb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gwffdswxh.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/ghkbqzkce.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gzefzjdxb.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gdnhcqzur.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gvqvmugrh.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gistbitng.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gizddvsvh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gagqdfvaw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/glpwytwzl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/ghvldsurh.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gegjcnnsb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gtovmmykg.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gvdjnkfbh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gwkccfzpq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gzzpkyibk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gtvqvvjui.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/grkywtydb.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gjpvcxcvy.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gdzoddnrz.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gzyqtbqsy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gceeqvfzj.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/ggoxemijz.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gihpsmbiu.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gamfkztqu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gwhmvluqh.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gzvxoesbi.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gzjsesyge.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gtnjgycik.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gflrbjhex.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gnmiiirur.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gcdrpmbbv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/geetzdlpd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/guoacchwo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gobeckaja.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gbepaghve.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gbcvetmfz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gkaiskqkl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gsanpwqag.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gvubemway.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gmcbbuufr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/ghzupfhse.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gzgididrp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gzvhnvars.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/giloglqyl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/glhharqem.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gxdqamfsj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gcjvvtkqh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gxpjkgtin.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gifqkwltc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gdiadtble.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gxjznjmhd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gouerleew.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gnlcaopoq.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ggffphsff.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gxqnsglla.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gzpezkmyv.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gbcuptgih.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gnpicanzo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/goadaaupn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gkmgiyyax.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/grzcypkxt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/ghdbwgfck.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/griajwsgo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gpsdzfguk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gvilisaoh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/glgvcykxq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtsjvfaay.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gapqmfqih.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grvnfvjsu.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gcsoadmwh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gxtdilbuu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gccqzmflm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/glxdsajhz.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/ghqdzwxqb.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gjioxgsaz.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gaddnmnch.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gycgixvhq.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/glmjpldtz.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gsgsewzcj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gzobfynqz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/ggiintrue.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gweaieywh.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gmslxfchx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gakzwricv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gqcglhoec.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gpdvmhetd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gxovmdrrp.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gwuzrprjs.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkgdzhkjk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gebprqohb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/ghsyaihdk.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gmpzbjvqi.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gojymtpos.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gntndygtl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gsuokzmgv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gkerscshc.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gjfagdyvd.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/glbkxihrk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/ghhrexcfh.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gztzmufoo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gbjwqchoz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/geiwyhmxk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gafgtfadv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gkokrivcu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/glquaciws.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gltjtzxsh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gbexfeanf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gmoithxhb.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gdaimgczw.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/glwsqqefq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gcrftyqmq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gxgjfktxt.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gqxhxxnwh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/guonftvhe.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gglvxkcgl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gzlkrjoug.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gwrtbbbgb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/grbipecja.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gwnonkdnw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/ghqwmmnte.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gyjpeoktc.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gxrssfviv.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gzzncxgun.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geyvehrth.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gymobbvqb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glrmoacgl.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gfruxzyvu.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gocyddiew.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gzgtgowml.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gmgfoaycp.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gbcjomhmk.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gxwfxozmt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/grsfrpqxq.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gayhpayas.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gaixuyrkz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/ggmjewhsl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gfeuslkrm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gjebugahr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/geydforhb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gwlnktmgl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gfstitvzg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gykjemhmx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gyepzordo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gxwwxrqjn.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdqyipile.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gvsftrtpe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gcpxpxvfe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gpykifhhx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gpnsktkqz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/glihudtms.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/giurjetuy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gknlqlscm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gueplkoro.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/guybawziq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gadryqzaf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gbtjqxkfy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gqulfsgym.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gpbbyshhb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gpqlqvziq.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/glktzdpic.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gfugypipa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gwvqbplvx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gqgkupsng.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gktpysugm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gvylgkfkr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gyovmcsgl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gzrdhoncu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gnnpfjfwz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gzszmrlbk.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gbyxawgrv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gfazlbycg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gphirfjax.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/glmcxhwjs.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/ghxrdqpxw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gllyipyeb.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdptviole.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gjytgwxbh.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/ggfwiewvk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gqpaxqsnc.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gxlckhsbj.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gbrwnfxzh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/ggaoggxfu.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gfvqlxebj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gmmkwzogr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gpmhetkuj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gvwfprqen.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gdauwiiri.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/giozlpdrp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gnzgcjcyl.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/ghwpstwco.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/grnlzipfz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gahtpqeam.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gwuyolids.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gmhfdhusk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gdflpzghu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gzdococnw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gumvjnbkw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gsfdvbheg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gazpgvkrp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gqacffeub.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gghsqzmvc.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gaqvsaofd.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gmkmbkunj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gauzcbotu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/glardnstz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gassovjuo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/girdaduku.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gofrngmnw.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gsaxbfhyr.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gmdrjnwla.sHtML


<!-- 参考信息 -->