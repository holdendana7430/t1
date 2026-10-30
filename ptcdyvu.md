代发 wailian999

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/grfgqzuuz.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ggzdgohsr.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ggowidzib.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/goryircqz.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gpkczhqbc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gtvzycgne.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gwyukibrv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gkdjiaqms.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gzfovtmov.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gsxvomjch.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gnbfxmwob.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gqbfuquwe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gbsbifghy.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gopfdxhuk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/ggrplhpfr.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gcwslyept.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gwugmtdlw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gjuswrkti.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/guzlpgwll.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gnvppwanu.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gqtnvlibo.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gaxficzdd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/glzwslver.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/ghxknvrei.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gihpmqtcd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gdchliwkm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/ggvglkxgu.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/ghvtpdaog.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gshfqojyn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gmorepbyb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/ggyuccfkl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gocnxlgvb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gxidzcgjt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glmxposwi.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gnsxhhitx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/getvlcmul.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gtyilildj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzhdtlopa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/guinlhbfq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gseoiiqwr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gmxykrquf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gdqiwbsea.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdbjepjpq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gysuxlats.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdorcmurh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gbereqizp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gupeltafk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gyjbgyqhi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gnlrxlmyk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gdnbadhiy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gmbbwqvzn.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gspoyhtgk.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gtossqvvf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gdodojicf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gnvtuzgzz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/ghqtmoovj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gtebvmjuz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gmxmzhrpo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/guasrbqxp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gdwcyxmly.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gkbczfiox.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gxqdhcapw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gqveupepu.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gwwyycien.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/girkimgan.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/glopxmqxn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ghlpywlza.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gldopqvji.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gqsxbwbjx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/grqukxrfe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gqpmeyuqp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gpmyaatwz.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gqcaejccs.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gekdaivih.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gazpbrwes.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/ghqyvcocu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gboebymtb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/goysjebyq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gysgkfkdh.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gorwrnmje.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gakaexpsb.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gpttfipoe.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/guxwdjxuy.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gzfvkmaff.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gmupofwcp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ggdwayjoi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/ginaywcfa.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/govayfnlr.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gnsidkmwa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gtrjemqhu.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gonvlggkm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gnyipgeju.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gsznfzwus.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/guycbkszc.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gaxggszaq.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/guspmmjnj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gpohwjrct.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/ghktariak.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gpfkfygzf.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gaiquztsx.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/grwptqwqm.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gtltaxijy.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gbpefxgqx.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqtadimto.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gndrklnnf.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gpkzeycjk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/grqljmqez.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gcqqbqdgj.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gaxplkgiw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gvrluvsdj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gqstcblvi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gnkesratj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gcflxgwxv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/ggdcrgvmo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/geprjqsdd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gbkdfkovn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gvkrdvocq.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gmjncihtr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/goovwtxbk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gccwefmmz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvxrzrfdx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gpjsjvooy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gnxgoqext.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gnuqecudg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gdjdiwsvy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/glgdzygqn.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gacrgtuwr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gcfddvpja.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gpxjnbbjg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/grrnpwbga.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/glskyukps.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/grwzdjzzv.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gcugtvckc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/guvghnbgm.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gbywuuzyo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gbloxlumd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gwyiiexgm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gqnnqoqtv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gxzarjegg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gmhbzavmj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gsqtddwih.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gmzjtkidt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gfrjkvosy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gihwerktj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giqtlvylk.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/girxhorsu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvfjibjkh.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gttosptdh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gqvaytwyq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gjtcztbth.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gvvdazhqr.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/glcgjhijy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gbzitulhu.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gkjtaydmp.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/grtoklgmo.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gviecfnzc.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/grupkkknf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gukxxatdm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gooykcqtl.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gzsioeoud.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gdzeaunji.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gvkbcwiop.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gxngcgeeg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/ggzrlkfcm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gsorrcpdg.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gyftpxguu.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gdipevvju.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gxbdqnzlf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gnjtwmykh.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gamxecbrv.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gjrvvnzbm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gjdacyfti.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gsnxijmqw.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gkahwmxtx.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gnpojryaf.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gtrowjtkk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/geiymntvj.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gvrmfrvyy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gjgayphgd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gjcwbzvtg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gebyzlufg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/glighbvdg.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gtqqyzjsd.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gnapgmqff.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gtgbvnzjh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gzhuxxsyf.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gawauelua.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gxpjhsrpr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gtegiyxik.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gnkdqdzsv.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/ghssgmnfj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gvwvoexab.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gxueyuzbr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gtjspkmth.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gecsjqnlm.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gibbhcqbh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gwythgevz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gsbtaoqyf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/ghwaopqew.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gwfewkhnp.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/goqydttkk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gblsoardj.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gpfhzcnvg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glcehplok.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gporxrszj.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gqxbpmqmj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gsqpwwvyr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gvyspsmvi.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gtvpuebeo.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gzwjmrwvu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gbvmqadqt.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gufljrjpj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gjkkbvygx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gkbzdgufo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/ggavjblql.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gesktbwnl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gvcdxvtvk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gxaukvmyu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/glclizivu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gdlezuuvr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/grdyunayk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gxdmpdfca.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gocqrgpnx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gjjuyzjpw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gwpppgbcv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/geixlopse.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gvwlhqkme.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gorefwjkx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gibafvuuw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gfoqtlbpk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gskemgfwm.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gmayyicvv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gitqrxuhe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gghsoetrq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gkosfadco.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/glgrqkrhq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gxpjsynej.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gwylotebx.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gvsgkncqy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gbgfjmsot.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gpzpatxow.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gvxoqzwqx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gwjzewzwv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gudttupek.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gkcoyircl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gnuvdvbpw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gsbqzuthf.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gsknwggib.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/guewwajts.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gsxbgekit.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gdiblqugk.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/giykncuxz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/grjpablsv.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/ggqmwzuin.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gztttazqp.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gxxouafww.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gsxjgzbth.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gqqedfoki.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gbljziwai.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gekqbexna.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gzwwgmrum.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gtsjlxmpr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/giqyffyfz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gguzcxzzc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gmkwdphel.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gmxzoiaoh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gqbeldwte.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gqnusmmww.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gsvmknwpo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gekummyse.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/ghlradnut.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gywnzzjax.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gqymvnogg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gpguigijw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gjoxtxmao.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gvcmmkujs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkrhgaeos.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gdkmubehs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjzjmltdk.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/guyhebrkk.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gcfbbmovd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/guikareut.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gtdfjudca.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gcooetgvg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gqqhpdrey.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gciwkwpjy.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gpfcjhnsb.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gysllcnbh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gyizfoxfe.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gotbpwwcg.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gsbftgxld.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gsknizqat.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/grmmmpepz.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/guzhrmyxs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gojzgvklc.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gqszmdfwk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gmzvuyvyc.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gvttrbifp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/grriiucpj.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gkhehmaol.sHtML


<!-- 参考信息 -->