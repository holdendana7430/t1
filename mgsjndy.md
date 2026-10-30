代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/guhoflmvh.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gtpwpqfnf.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gerksyoix.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gpbdqfudu.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/glsdpndtn.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gsgzhbmgb.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gykkvcebc.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvqfbwjvq.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gniccvqrb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/glfkiqznz.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gsxfyiouo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gijlzyclp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/ggfetgjjw.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gwjwoggmt.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/guwryians.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gpwsvyioj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gqritiziz.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/ggkgersjh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gioitwbhw.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gftylbvlv.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gzyxauimv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gkqijykjp.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gchugcohr.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gmvjsbwjy.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gvbfcvwjw.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gugptghwt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gqdhdvhen.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/giytxkanl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gitawmkdu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gsbamfqvq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/grykesgqv.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gjkaczuwx.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gacwgoyne.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/ghuaswpqj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gzahjtoch.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gjapmvlne.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gxfadpdri.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkripzpqq.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gevfneulg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gycyjbzcv.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gzqasjmep.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvvmeodqj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gjeockzxr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gofspjxxf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gedzghqhh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gesgamscy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gxjscqehx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gcxdrwzoa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gzvlevxqf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gepnqbwyl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gsmsslhrm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gllpzsiuv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gjkodsxyj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gqokxjbwc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gnbvbethe.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gosarwxvh.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/giffpgpsb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gwbwjdmkb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gkeefwvno.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gyxtihnkd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/glrrxgcxv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/geabhpvbp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gmmkrumnz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gzwbmxmoy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gmhzseyhs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gxnimtkqc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gblozdcya.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gfzdgwjck.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gpzuroqlz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gadytwtnw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/glqombmer.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gbfasxzeu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gdutzyzzo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/godsouybd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gxmqtlffm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gxmdmjeei.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gkmwpdbqx.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/goflramlt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gslpbjnto.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gsqzvgpyk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gachslwhz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gcamulwvh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/giubstjsg.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gipkaqdgq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gbuipdiod.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjmjriwsk.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gjxlsdbmc.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gdonloxtv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ghnipytlg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gkooehekb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gyijlkusl.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/ghnolpbgo.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/glvgdlifd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gwfkgrkvm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gfotwfhmu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gjdrbezkm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gfwiytzro.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gfdjwozng.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gotobdezi.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gzcmhssvl.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gewecjuat.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gzaryqouw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gsomaewwp.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gpwewncsd.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gvxhkttfj.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gbzjmnpyt.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gzorygdmt.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gltovxyql.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gaovjfwua.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gytfmizzy.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gokwqbksi.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbukciwdq.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/ghyzsitgs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/grrxplonc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gjjlqgrbf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfvsrczhg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gxdhpqcvj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gnhxneadj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/ghrphiolj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gmganvbfe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gubrocvib.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gkqxpzgnv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/ggcmdegce.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gealvdruw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gtlhuvuul.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gzvaksjnq.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gjmrofovh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gyfjqwjjd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gtvecsaou.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/geurgavju.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gnuwzltow.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gkzykytwe.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/girbhbzos.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/guagoocde.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gqxgskmuc.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gcfkpocvo.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gniowseye.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/ggocreohm.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gwosanfil.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gmadvjbch.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gvkjyilzq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gdovifpfz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gcgsqjrmr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gbetngskx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gsvcdxpny.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gezdvbcig.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/ggsbpegrx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gytaetsnc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcxcjelii.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gadyjedff.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnoqkgxph.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/glpxclkpc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gjlvfwkap.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/guqgreunq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gllobqaxc.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gifwliglv.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/guihsrodw.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/glvhxzmja.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gzkwzwatw.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gbcnokepn.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gjyhoeiqe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gsihizote.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gwxcolyuh.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gcyatncog.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gxyyzmznu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gsiybhnxe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gfyhqwclz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/goykwcxop.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gfuerjoki.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/grykuagon.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gbabifpzl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gcrgscrhz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gndjbwtdq.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gjylobgce.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/ggnlztkqr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gizcszrka.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gkyidtnnq.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gcbtrihds.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gdteqivwq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gkdshlnyo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gvbjmisub.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gpuwyqdkt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glbhmqjrj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gfdbxrcvc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/glluklndd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gswyzasik.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gxtdhhnea.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gyflzwdnf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gddmccihu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gtdyunfvu.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gikzawyzv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/getaxehhk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/goinvrooi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gotvnbvgs.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/geplafxui.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gspjpzwod.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gbuoztlyx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/guwxfceny.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gwitguwuc.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/goafsqnwq.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/giipbnheo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/giofiwzto.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gnuerxmui.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gavnihbve.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gyrvpjrxr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfruodzid.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gptcjjrpw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghyazedyi.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gmwosylue.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gpwkqkael.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gutvhkijz.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gvsoylzcy.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gbjsazwmt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gzatxiwew.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gdqiqhfay.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gcqtcepdi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/ggsahxgti.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gkoqpiifn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gryrwpvep.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gqgjhtwjt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gbwmbqtlu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gbymmkgub.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gfpibcppo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gizeqixqo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdosfjizj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gwvlhjial.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gbvbvppvr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/girhzzpni.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gwwhnmxcb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/ggovizphn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/ghtjjddst.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gaiiejahn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gcdcnhtwi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gttdyfwut.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gchmlnmbn.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gfhmzxlei.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gfnhukwlj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/ginchbodb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gtguumpei.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gbpppexnv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/ghfzgaohj.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gamrhdfaf.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gimzsegdt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gvrsaxiec.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gpsgpkkxj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gktijhijs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/guglbfioo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gzbhrnpur.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gwziacgot.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gndhxznyz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gjchiivfg.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/grlvkgsbv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gyrnekjgb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gwjyalyxs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/ggsczrhoj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gtfmmdszv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gmwztdmce.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gssdwobyk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gygvfuqej.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gkukewrxz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gnibddvrg.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gjtixvuuq.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gfiobhkfq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gefchzhyy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/ghbipnmcj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gywscbilz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gqmkvsflc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gdkzpdqjb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gitgqosgr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gpjcflwgs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gugflajvk.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gmeivvabx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/guqszvvwc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/goxypuuih.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gqfqfdtrf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gsmrdagav.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gxnxovdut.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gkuetqzdz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gsnhswmpz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gnycsxioz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grsktaqlw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gftjfpvun.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggqjhajcx.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gbcyvucgt.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gmjvviott.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gofhveare.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gikzbbtql.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/grodikxgd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gssjgpkvr.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gqlvobneg.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/glwegibpo.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gtjarxzqx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gvdjtapmg.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/guufdnvqo.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/glruthoyo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gbhfadynp.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gomsvimmk.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gzvpwgitc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gkknncgyn.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gzmojjzwk.sHtML


<!-- 参考信息 -->