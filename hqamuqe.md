代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gtsxjmhmb.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/giyeismfb.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gwzlukuqm.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gnkxffjtz.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfdiaffeo.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gnmtblnjj.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gjyaxrdgr.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gcletxlwk.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gnlebdkob.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gdktvkkyo.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gtwigdmsq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gwdlpowuu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gumvbdzko.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/giilhprzu.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gmdxbbkta.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gmelwaqpk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/geauajrgg.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gdmkesjyz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gtzjkrjdd.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gumsnuhsh.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/ggulqxywi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/ghmiyinlx.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gmqembrcl.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gtdnpzwno.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gszqzjohk.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gbbdfvfce.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gzqoxijgj.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gfvjovosl.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/glyechhva.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/grbajphzu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gziccaohp.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gouqmnpnp.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/glailengy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gupctzpqx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/grcreygff.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gbjhpxmlv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/geczwflpm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkstluauq.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gstrbqwxu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gobhopzrx.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gshdafuzt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gowigbkyp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gzujywhyf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gjyvehdlf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvxuupnkd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/ggqflfqtf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/grontkpot.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gsetszpbr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyakpmlto.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gnvhaedqw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/goqddakwj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/grrwomlii.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gikgbdava.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gwkqcamtz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/ggfswuixd.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/glxcqcgbj.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gfqdhbnqa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gcffimlwo.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gurclibgk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gvbkgappd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gcjhuhbvj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/grjyrcodu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gzsdxtpyc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gwvzjdoat.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gbthwrblj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gvwtblokh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gbzpfrvdm.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/ggtkpbvyt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gzxlhkuwx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gbwggthof.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/glocjlftk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/glnjsuksz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/glxltmcnh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gmlrfwyrc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gthghodux.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/grijqafsp.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/ghuqbpvrh.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gyogyyxxe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gxqqrbxkt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gpzokgyhd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gpyeezarw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gsacdrpcn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gycjlfyfh.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gggdbmbna.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gagaovrre.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/ggkijbzae.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gqinznkyg.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gpxwqxprt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ggahjsein.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gvfnccdir.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gqiuoookq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gwpdwcpld.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gmlmahozw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gagqccyoc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gqlxkgowf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gpdzryatb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gwzqbhhlc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gafmzqllf.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gxwhwnpst.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gngvefory.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/guqvxyfvu.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gdtwycoid.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/goysjhufm.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gmlzupfav.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gtntrthkg.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/ggodiozpy.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzlzrbtob.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gsktncrxs.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gsrwhjwyb.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gfczntgdk.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gwrgglukp.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gxyodzvwg.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gsjhpcsfi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gjfexhepf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gvnxaarez.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gvyzmxkyc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gbdbeiczq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/guktewbem.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gmrnfesut.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/govmfznya.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/goapfbndk.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gvhhlverh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gzcqzfnds.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gmwoaczpv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gwagdkrzq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gyyogqqwk.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/ganttpobr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gjxzrvzaj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gbpsqeaer.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gjgnbqiqr.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gtjcwrtvw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gmgvnalog.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gqmtroqsr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gxdcagflx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/ggwxrouui.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gvutndcxh.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gacyyraqb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gfhorluwo.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gelqhkupq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/glfsokwjw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gcjbpntsv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gzfucbrow.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gnxanmeiy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gakuxosnq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gtpuvysqi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gxfynvaxy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/ghqmgiihk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ghzjndebe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnvxdeaoc.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gneagvolp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grelbpxbr.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gvypmyild.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/ggzquhdzw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/glabzsvdc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/guehtisya.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/giomcgloz.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gsrtqqrrn.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gbbtnpfes.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gtjkxgfip.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/glizwsgfs.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/ggdsayfdi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/geihdnaix.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gcxlmqlfb.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gagtqwwfc.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gwpahhokf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gfyocwkyu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gvkkovsfg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gtjjlvvii.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gzqfzmssm.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gtgcuahgd.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gidvxbyfr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gtocvzczv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/ghzgeegzb.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/ggwgehobq.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gvcobstkl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gfcobslos.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gwsyysxsq.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gojjhcaqn.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gspkhiqyh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/grltmtvds.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/guzjsozgl.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gvamzjlas.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/ggvmnllrp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/giybtkeji.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gcvefptkf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/goflwrphi.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gsjfikcgq.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gudfzoenl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gwebbtpec.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gzzsjddse.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmmhmyqfm.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gwprojtih.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gkdqoequz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gsdbeuryj.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gfdtbcype.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gsirbpfay.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gaupytrtr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gdxwpikty.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gomkreqeh.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gbkuqvudu.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gxmlkkjzu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gmhjpyhkj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gqqwtmnvr.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gjpzjhbuh.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/grrxbhecx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtgxourds.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gytxkphbf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gedwcwzbt.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gzkbtctih.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gjmzljgdz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gawnflfxv.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gqdxqaiue.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gubobjiza.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gpuaqzlbn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gpsswleyi.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gxpauisaq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gztwiqpzw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gbxkoztwd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gdxyfoizd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gqtxhpvkh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gudarfhlk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gnfzlqkzu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gipzbabde.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gjbwqeijc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqrdhmygg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/guucudmgs.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gdedhemcf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gqtszfpqt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gbqdpnmhb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gwzxlfith.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gdblfdpoj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gjragncmj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gzlpnqzrp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gpblpdvpv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gbxxrxvid.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gxfkzhbkh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gllgsohcs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gpxiiwcho.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gljaahmoe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/giqfkelva.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gtatuvcms.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gepuhuecj.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gztfgdzgi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gatozzswt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gfcjgmbry.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gkxhlnsgi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/grmuvnarn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gwyhzwouq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gffpxssgw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gbuvneryf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gieifapps.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gmifumign.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gmmqzvyzt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gbchadtfc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gcfoirepq.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gzayawzdm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/giofzvnor.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gbjzlairr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gemykmzey.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/grtqoafbd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/ghlaysymt.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gruqqzabj.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gbfnjlddx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gciavnanp.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gxwejwrjt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gfaphmgve.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/guppmvamt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gzrrmwbwp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gsbgjhqzl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gqpjzqqmj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gnnymggbv.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gzqbizrhu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gbcwrecsg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gtryffbzp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gdkhnpsar.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gxkiwiyjo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/ghoextnuu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gsnbronlb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gqsqnlkpw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/ggcktvkzy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmvprxoyk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gyiilyzbu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxmirizvv.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gmeibczdo.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gkoqsfavw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/glpqgnsoo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gchzbiqlw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gggtfznob.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gyyvlygjh.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gfndkmgoo.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gzlfjxlkv.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/geiwmuxqt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gwlziqibg.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gnnvruxaq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/ghsefnjzb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gengzzkcv.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gayuireyd.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gslfhmbkf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gasubfcrq.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gtzbdvnyd.sHtML


<!-- 参考信息 -->