代发 wailian999

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gfvrxzylu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gbtrmeyrb.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gyjvwwwjr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gepqqcsar.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gswswvglq.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/ggukxkoqq.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gwnjrsqgt.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gvgtnuvon.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gttfhunuk.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gxbqapiuc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/grmnlvexj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gdaeivpkm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gkrgbwkga.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gtusakaef.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gyfgotemb.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gplgfbvho.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gqeozocxs.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gdpqcqtah.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gnagbpfig.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/glkfaniff.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gkthjnybw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gaaufslxl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gntomurso.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gnpkonqsq.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/grnefxltt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/glhodtezj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gzvuhvgki.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gmtaoztmy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/ggozbppsp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqzjkxnue.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/givcogjxt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gthfhwngf.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/guvibrrvm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gbhrhigku.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ghyilmyif.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gfnuknoqn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gmafdgxgy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gouhqfaws.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/grhohecyv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gnlakfusd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtpxtkviz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gjbtkawzh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/ghxgbqcxo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gvcmjhrkq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gmfuhsnih.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gukjzbzwt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gobpzoqdp.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/geozswvnf.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gthcnmker.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gehexixat.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gutaereei.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gotmwecbh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gsbcxxiyt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gqumuldwh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gyxevqtbm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gftksklxt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gujmunbbn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gyijukpqp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gvswmlyti.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gdsrrpavy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gcxsykvvj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/ghcvdvbfz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gorgtlttx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gusanjpha.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gqnptsiqh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gnmzjleat.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gfejlyrfi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gysxlkifv.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gggdcaxan.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gnfdfjugh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gmewodibw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gfmilphfp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gtvgyauoj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gukcxmqht.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/garikoqiz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gehdqfyyw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gecqgvegp.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdfjmomac.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gmgtjlbup.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gfigjoaqx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gvluluypv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqpmhsdaq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gblarlmdk.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/glxqbcfyy.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gbqczskya.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gdzrvehkr.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/guvwjdamr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gonujctbu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gbighoxxk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gdqgqwjwf.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/grpyqvmbq.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gcxhjvctm.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gtyyvfidj.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gdybcmtpo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gvdmyxtqb.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gstnobmkz.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gcvjffcia.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gugujhyuu.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gminbgxio.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gmbbripcu.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gcemkuhbr.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gaqvrgddh.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gapfpzadz.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gaecjeyrp.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gmaytbveb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gflzqnxph.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gmhcuhtob.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gwgcqaymo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gjfkkijov.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gudcjntvo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/ghqssnfjs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gabpmvdiv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/geyvtegmz.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/ggwenyypw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gouutklvm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gxipgjota.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/ghogwnfsw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gcwkltbhn.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gqxtbyxek.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/ggxdzgoao.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gwfeotvqm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gezchpdhu.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/grzectzal.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gvuttnwqj.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gqdztidwg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gvlwasqdv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gevgcjhzp.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gcniqqmor.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gajgiorro.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/ggjtjklzn.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gqhmpndgm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gftgobmeb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gtpmwzqcn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gwgbffcen.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gqxvuyvoz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gmsqojwvm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gjewdypff.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gdxgpalpb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gbyhihqfj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gluncushu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpfrszsmf.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gpjluebtt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbvolatlw.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gwvrxpzcb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gqvzfzzvh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gztmvxxfa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/ghvkfkqhe.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/ggtjqnodv.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gemquaewh.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/ghwubfgzi.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gddxzunyv.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gpekbkguz.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gqljiykfp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gegetmwun.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gahuyrxft.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gcddspuym.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gkglunbwh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gxootcctm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gdijeivhk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gwbouxuvn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gyhroxuno.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gpnhrvolo.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gjiexoeyj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gkrjfcbuv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gweoaydji.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gevbqlimf.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gbdjsihbk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gwidehpuc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/geubtgapj.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/guolxiohn.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gikgsptoj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gsequfhoy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gsjzpgjwi.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gyujkhbrg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gstvrhgon.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gllxtgfke.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/ggezfnekl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gzznmdxrb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gvaghqzac.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gxpmwpoks.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gykwpsqja.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gzqjqrusb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gsecvwmpw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gzrxgtooz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/ghvvsxkue.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/glrcjdduz.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gffxlgfaq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gzndqjaxb.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gwyozreho.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gchjeeahx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gkpdnjint.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gfkbljzow.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gapzygdty.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/grcrkycsm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gmubnmoyq.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gvopbjpbo.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gfsmobthb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwfwjxycx.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/grnhidvmn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtxdpbrpi.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gqygoefdw.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gtydgnqaa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/ghrwubmye.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gbutlqjnh.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gwschqigd.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/ghkformyz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gkxeerglt.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gezbwbuzz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gpatsymsz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/goxoofycz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gzhghsipn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gpiswhrrw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/ghdwmkkhd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/grbpgpdhc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gxfcufldn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gwjudmfiw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gnugptldm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gqdnuqgyd.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gqtjzvwcz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gyuggrdgm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gsrhtubja.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gndzmyuwl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gadbvqyrb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/ggsgirtap.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/geuroewvi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gxmldpsnq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/ggzppjjoj.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gtscqfsaq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gaequsshy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gnhaefbdw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gkocpxhxi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gjwgtbdwi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gvtopqocx.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gcizdwfcv.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gnadagnda.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gpweikebj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gsfpuhtnu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gwnqzprxg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gupreomgs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gonqjdujb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/godzlbfgs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/glaowvrrx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gjbvvigtg.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gpicidkyl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gfiqufrfv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/grvkbdnpd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gpytmuzdv.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gsbrzinua.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gagrgconm.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gorywnyij.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gdneqmmci.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gejzripsn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gzmigcmmf.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gvufzxvqq.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gnpcvlkel.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gdibcajeb.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gghfxtwis.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/grwvsgart.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/ghtdrncfq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gvpvikpip.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/guxgtpqqk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/glfjsnbdr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gqgkkqxwh.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/grmyfgqon.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gbxgsmfbb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gsdbaukqg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gojvjvquq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gybpmjmmd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gdxmnlsrn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gbblagypg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gbeiiwmsp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gggfljaxq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggatwbpux.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gnbjgshhm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpjiisphf.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gunvuhdii.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gwyrvndkb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gxytzpzzj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gornmimsm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gqculrjko.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gdsapivsr.sHtML

);
来源：http://baike.hesvh.cn/Article/details/grrddjtcv.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gbleaatcq.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gugnweslh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gbwpfvthf.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gumnkejsf.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gyaivawff.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gspivscwv.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gkbvtfoiw.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/grxyefanh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gwwtyqktu.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gqwfgmgeu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gnxseaeeu.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gdfetsqio.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gkvurhhol.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gqailmgbk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gccbaisph.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/glslyvxll.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gaaojkgdg.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gtvjaubsu.sHtML


<!-- 参考信息 -->