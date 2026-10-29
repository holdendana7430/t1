代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gogvyjroc.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gxjotagpx.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gtlpjoqxi.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gaxmoooqm.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdiklpah.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ghidklkyf.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gwwntqgdm.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwgbjohrd.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gtexngnxp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/geebxxwtm.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gnqkqqyua.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gbjshbxks.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gkanmcewx.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gdoxuamcg.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gxdcnpeyc.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gnxcjkans.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/ggdilenbx.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gzodmebwv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/geuehiuyz.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gkwestpsi.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gwgenukts.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gkzldggcc.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gmewnvagq.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/guaugpobz.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gwbmhieoz.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/goyksimqx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gythjpyhb.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gvytjskmg.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gxslabbgd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/grzgcfagv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gmlelrbdm.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gnizwxebj.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gufjursfr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gbeindwis.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gehmcriqa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gtjinscrv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gexerexfa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grkostnic.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gcrrybolc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfmexgyyw.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gcnibecbc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gieeiqhje.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gxrvwenlz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gwsjkuftr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gqrrdcakg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggutyqkji.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ghnqspfmh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gqqiksmpn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gbggoslbx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gxochbpwz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gwnrkaomp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gelxjqvkt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gotrpcste.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gdxgrubln.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gcggiqqts.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gezvyeklg.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gfopkrqjz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gnkakrotw.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gcxprykso.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/goufqdsjx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gaoswfeif.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gqjjarhgy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/ggelnzadr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gsgbfpaxu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/ggyupwivs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gpyzxyulc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/guchvatid.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gciwnbogf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtlwkpzbk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gtttxyhkp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gltikhcrk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gnzrnfprj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gomcjivht.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gwdyznmib.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gvmfekzmb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/guodhzwlb.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gefdxutpj.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/ggfjghrxh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gezvucoqj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gzshvxlvc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gdlwwgrrk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gecejedbp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/guuxuxgkw.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/glxfcjrwe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gtlkcmsra.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gwqrxdvcw.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gwvswdypk.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/guycghdjd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gbkbwfols.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/guxurugaz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gwbbaency.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gsvwrijui.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gbagxzcen.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gbbvrfrqb.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gxrkzlpcf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gtckhrnek.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gmbcuzxwk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gzngkbwuy.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/glcaxnhlc.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gbnmnqotj.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gbdqpwrlj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/giajsgimt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/ghjiismtp.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/guyhsctpt.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gwgmkhmkv.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gzzocnjzg.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gesbwewhn.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gwqxstabg.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqvecqcec.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gdiaevfca.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gxojahkad.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gsdiyfgps.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gvhraofpg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gfevaurzi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gzimdraiz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtsnwiunn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/grcymkuxq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/ghwqkzfbo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gkmrbhfhg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gescmzvri.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gyamndith.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gwxjelbsy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gwesgwjeq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gehtekrog.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gqfngxmff.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/ggcffdcch.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gzefpznnj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gedpterqy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gntpvqwgg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gsrszdnsi.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/groxxviyn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gjoyajagh.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gokafvaxs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gbrcrcpnq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gwbaggjia.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gzomghnjr.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gwoddslbb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/goiagqtzz.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gmqkvwxwi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gyvbjankj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gcxyymnwc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/goqyuqlcd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gizllvajg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gmxfmxmkk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gcasrvhvb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gwzxzyosg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gorjougvx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gaiqvmajy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gplrzekdm.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gmagodwfj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfhuhtcjg.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gghaviwub.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gvtyvgopr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gjekcdzbh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gotncfujb.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gnmqlglec.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/ggrpodsal.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gvjnyibtx.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gadoxusag.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gzdgmmgfe.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gdctwsgrp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gcjgmhdtp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gqdzzthgw.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gqezdnxaf.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gcincillb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gqneetlbk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gdmoxyjdo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gdvwsfjbv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/goiyctjwl.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/ggjhfypun.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/glwjulwfn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gjbqtfpoc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gqzzhqand.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gmxkxqwoh.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gjumubbjd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/goggzvhgk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/ghhiartef.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/giecnnklo.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gzdlzgfhd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gxhhrrbms.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/geiskdzhs.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/goagoqxha.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtlebqaef.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gfrcqaowo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gjxsixtmw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gqvdarmdw.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gvntcrqls.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/glgvfevyl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gmhugxwze.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gzoxbjqqf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gkpddrgah.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gqpreustv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gbsnfrekw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gcpxnhzjc.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gxhnxsydb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gogxafcgv.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gulfkvqvy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gsintvewh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/golpqblew.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gaqxcaspo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/glomzkqag.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gtvunjvhy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/goejijcey.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/griswcjfj.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gxbtvmtmg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzoljmt.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gmevtphqt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gznqxwocw.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gjhdmehxb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gwiujqzqk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gqqswpcjf.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gjhmyevyn.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/girprieol.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/guihgdzmz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/glhznanzt.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/grbmiysbu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gmobobufz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gjdulbhga.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/grrldpqsh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gioioysxy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gkuefrqwr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gfngpfdke.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gsumygiub.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gsuotfodq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gxtdgqzzm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gjlokxvsn.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gbsdvywwv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/giwaupuey.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gucybgxfr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gsqinyjxz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/grpzgayfq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gnazkorgr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gyybforhl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gbhksushx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/grcytmkta.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gdvqwbmzl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/grqnesdmi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gvadxbpbp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gefbhmkuz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gomvxbvih.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gypgzyicv.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/germatnne.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gjpgxcbqc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gqwrprswb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/goaocdobm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/ginqudeyu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/ggipphazl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/ganaccjbm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gyjowgevp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/genxclrfs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gnacgjwqs.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gldbqwooo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gxuxtzwbm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gqrepgciq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/ggpvcuhgo.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/ghnsxompj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/griyzvsbq.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gaqblptep.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gzwukahhr.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gattmaosn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gzurxinde.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gfjjqcmxy.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gibsydzal.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gvjsoahzl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gyffljllw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/grofnxvpy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gbtztejyc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gnjctiaov.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gkjfsedcu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gkowhwgut.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gwwdswxxp.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gxisdlvug.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gyaogbiyi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gsgaiwmxo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gmzuyejkb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gzwhhdcix.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gnwjsxswr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/grrgeeiln.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gupyilbbt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gscnqkukd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grpdieblz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/glluxetsi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsqcnlydn.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gsgigkftx.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gkcsjfqmv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gvbwxhume.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gqcjlarzt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gpyxndyco.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gwtsizjaa.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gshqejcqh.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gabwuyeol.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gtemmfqwi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gagkjydsf.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gyiqlzxqn.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gbwaylrap.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gcdfblenr.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gtzeyubio.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gkvratqim.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gvbrhxlhy.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gztnhhjgh.sHtML


<!-- 参考信息 -->