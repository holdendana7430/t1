代发 wailian999

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gqtvotunf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gsyzmlceu.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gpwdeyqjt.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gkaqqglpc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gprobxbyn.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gtnevnqdi.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/glpqsiktd.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gzbmnhouc.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gryiorhxa.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gmhlmmoeu.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtcxlpmtv.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/giwlalato.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gsjgtlgxe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gmsutaimj.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gyztianhr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gcvcrqnjb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gqkugwmme.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gguekgobp.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gxcrruczz.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gzknurguo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gtpwhgwur.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/ghfibswln.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/glutmigaj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gynqyfndv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/geitkftye.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/ghcqfoyux.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gynjwidhl.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gqojijtfx.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/guluhtgan.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gowizmbhw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gabtwvkzi.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/ghyjtydtx.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gkxiknrdy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gzncumgkd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gnftvxdew.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gbpoabdfo.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gjtexsomh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gvypqlqig.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/geitncoir.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gaeirqnfa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gjpclzzpy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geqvbucih.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gllmrsisz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnaueepuy.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gsglhmyjr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gnajzhsuo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gcgoaeydo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gmvphrzwe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gaxgrvrgm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/goekshziu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnssiyegu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gxspwzufp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gewrlgrhh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gvynemypi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gqsrtopgz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gsnsarzka.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/ggweqnrto.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gubyaoccw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gabuytvzk.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/ggwifnoun.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gdfsrgqwh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/grtygijjk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/guwsigibh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gdvmeiyet.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gthftquks.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gykwddujb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gzmjaagnl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gmyjyrmmz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gsjuyjark.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/ghznvwjty.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gruhucyxu.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gwgcifsib.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gzicpwldj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gzrxoychi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gijocdwja.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/glsfdzrlr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gylofliir.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gmidrpcuc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gtpmpjxlh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gbehdsalw.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/ggyxjntti.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gnxyypebl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gkaamizjz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/grqafgxgq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gxycyqjwf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gmdjzdwrq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gkwjtwque.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gokfiozgr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/getyzofvx.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gcijayabu.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gzetkcmas.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gpjpvhpdz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/goahczdwf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gysaiyped.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/geanmjcfd.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gyaxxuvuw.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gxvlyymqg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gtiyexhtq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/geyprpbdx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gcoovjgpc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gljmuqzlu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gnffnbpdk.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/ggfwkjmos.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gfhzjkror.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gjxuqrnnq.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gdebxaris.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gqnnhpbpb.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gfmwuisno.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzycxgitm.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gkppzxgwj.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gtswrxbcd.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gfpfxpzds.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gzmhkuwif.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ggksdgcqz.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gbxjbfkut.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gdcqcdzxa.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gjmcbedfx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gorempkym.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gykxrnyof.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gmthiehol.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/glxcbuigu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gkxfvjbuo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gqvyvafdx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gtzlsnyvg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gvdezdgev.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gjwxbcpzc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gskhumjrl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gjjagztpc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gvyaxnjzv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gvihkttzr.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gwfojtqdi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gwvrmjcqb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/goftvihwq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gzviblylz.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gxtubibru.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gpibxacrm.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gkpqfzxdz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gihzhregb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/ghhfkuysm.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gpxntenfq.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/golhivxus.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gcanpralg.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gmsuhhitp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/grvanumnx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gutwurnlz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gbfewfvoa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gdslvjnmc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gwuvzazxr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/glosxtuop.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/ghtcukqej.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gcadwuyxf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gdjwupsmq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsgoxclby.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gocmqywpu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcjrnbmiy.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gbauclhbn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/ghxcxfcxn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gbkhrpwoh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gqgrccqgt.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/giycmfycg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gyyypxuyc.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/ghvjygsfn.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gvliqifnn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gjocrcpjb.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gxbsspszd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gtylhjarn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gsorrdiyz.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gkwfcnvzh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gaxzywdcm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/ghcwmcodq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gxmypaqpn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gqqklnhkm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gmzziaufg.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/ghhnqiwms.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzwyqqkyr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gbnyceder.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gyhtxmobz.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gtfilxmkp.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gehtqklrx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gevrvdjly.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/glgkcxenx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/giyawuekt.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gbyjtpbey.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gpmevutqr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gfklmzztn.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gjvhslupm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gfnlzjjjv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gzybuksbp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/ghsfjgqnu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gcpsmtcbs.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gnkkwyphw.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gpxojgogc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gfvuwmlme.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/guwdmjswb.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gistypzll.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gwerleslu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gdyfapekl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gtbrfkdqx.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gefymflgy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gweaubjmg.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gtfswhtmh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gaydrwtag.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfpcyepvy.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/garyjioth.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gudpbllth.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gpqkrkjlk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gtbylrtqy.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gstmyymfm.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gtkyadllf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gumuunvrz.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gvfngfqzc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzpyliesz.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gxiabpmzc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gmltwnqor.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gnsiajmuw.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gqljcfqys.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gatatjicr.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gtffezvkq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/ghqfebqpw.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/grtgsfpau.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gbwnjvvga.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gxtywerqw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/goxyzddcp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gmxnjaeaj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gomjmnjjd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gifputhbq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gfxdsxhzj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/ggpcmnvxi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gaxoyaojq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gksmvicjg.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gxxwyatto.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gsjkkfboo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gslmxqjgc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/ghrnkrpce.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gifkwcpjm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gixcpruqg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/grjeyalsi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/ggqujqsiv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/ggeczmher.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gjztrjgic.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gmckpcrzd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ghnlsmvlg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gyfgjawml.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gdwpaidtm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gpsxlqewi.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gqqpiuuwd.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/geihksfoy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gbhlmyxxu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gkzpsbfuo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/giokmtkje.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gpemxudxu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gvxpythns.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gsticdduo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gsaublwwu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gmzlbnijs.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/goknmolak.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gdyiuoqjw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/glbyngmsx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gwyhvfpux.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gmzhyhlbs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gkioqlobi.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gzjfdvtqv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gbjczjobb.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggxctmsiw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gdnwuvyfp.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gjyzskqnk.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gwtopxtob.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/ghcivzfoh.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gdmbfsavq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/ggwppkcit.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gihuthomp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/grackqwho.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gcspoybbr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gehhiardv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/ghrwnjvgx.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gvjoelzqy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnbyqghj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gmvfbxjmx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gxkqkrhnm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gjsxsbnps.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gcjvzpcrv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gwhmxuwlh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gtwafxhmi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gcvdxqyra.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghpciahvb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gaplwthag.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glkjgerjk.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gbojdsdqy.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gwvgwoeem.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gvnxrunoz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gendwdacc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/guilgivuh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gengnmhxj.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gbnupkhdl.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gkpnycrxd.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/goasbhfqh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/glvfngtkq.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gufnogpgs.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gzwuaehpy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/ghknalues.sHtML


<!-- 参考信息 -->