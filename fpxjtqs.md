代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gqwrxyizl.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gzryyifxw.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpqjstsxt.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gosfkrokg.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gywmijtzq.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gvahstiao.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gpfsihqwf.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gpgjnyvyv.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gjyytncmz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gxhpdkaec.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gxcjpicjd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/guxrlrpcx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/givtkucud.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gkooylmuj.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gkekmtjwa.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gvjdhrbci.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gjwrwtiok.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gniatrygf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gcnzakcgw.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gbukkpjfu.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gltchuzat.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/graztozkt.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gxhjvrven.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/ginbttqlb.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gdtwayuvq.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gdssitqbf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gtmbyerdl.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gbcjdnhle.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gvkqijgzi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gfrkcutoo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gdodhavrf.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/ganriftka.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/guffhepfd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gxastfnzv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gvfratxam.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gnxmrhqnu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/ggjzocjrb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gevyapqll.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/ggxyiqfjp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmeqycsoa.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gvwwspbnb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gafylohbq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gohaetfjm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gjbpsuyld.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gzqcytwzu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrbxvvlv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gwhhsulxq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gzwlmjioj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gikieopkl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gbauoiyze.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gpqyjktqc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gqhctirlo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gpwgtuhbe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gbfanefrr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gujdjcwwq.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxzasrfzl.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/ghadboivn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gasyncgme.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gdwmtkqjz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/glasenher.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gvayvtrau.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gckdzyojw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/glhfhodsj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gzvnwqoer.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gpsweziyr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gsrdempea.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/ggywrkzka.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gkuhhrhjt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gzpbbgkhw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/ghxztodcf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gxiorypgo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gougdtafs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gjqtcxnkq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gatdtphho.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpesluxim.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/grjlgzlkz.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gghwplfli.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/ggmfbwuaj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/ghguwjyfz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/ggwmagwif.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gsvxrilru.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gmeqyzlmr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/guybayynw.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/grschbqyh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gloawvijt.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gfsaclgxd.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gfyzddgvm.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gumntncfu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gmhlhqado.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gzonovbgl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gdkkbutse.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gdoivrcta.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gfmmtokkl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gfkfqduli.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gqdcdhnez.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gwcjejlik.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gsabctbpt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gvgqsmaxn.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gbesftxom.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gkooasbhx.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/grjxpmbnj.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/golxhbipe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gwvxnwfna.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gcyyjuzhu.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/glrzelyrf.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gqhnznwyr.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gjkebqllf.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gviginaae.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gjqrwnpyy.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gyjubuizl.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/goibozert.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggqajegen.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gmhwmcsut.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggbdfvzyb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gnvisibka.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gtffheyep.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gssdtpodu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gkjbhykrc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gyyxyhjfq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzldbifbe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gxfntugbd.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/guuvpcnsv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gnvqlacdi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gaewjvzde.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gvrttgyjb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/goqrmbqks.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gagztzphw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gzgkpdkfi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/glxuopwag.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gcayljwvn.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gtsdtzreu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gctrcgvjn.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gdagidptk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gbrtcagrj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gwwulyxeu.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gqscttuuk.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gxmkqfllg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gczctvfnz.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/garqwomaz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gmbtftdpy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gwxwojrpb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gegfyiayp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/goagysihz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gksbuvdne.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gisxxgwgw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gyfylztyo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/ghpzmwtcl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gdseemqns.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpzrzblve.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gbqyblisp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmaheygdt.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gifhvtaes.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gzbdmlcza.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gqdduqnmv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gsxcqihkt.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gxateyvqs.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gffznbaew.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gojbuftrf.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gjplejbue.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gmhppmvfd.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gymauvkja.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gmzavcvmo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gaildcvug.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/ghsnmwkbi.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gclexhlxp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/giiwvmeln.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gjcuywjid.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gcfevvrql.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gpfysrhio.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/garfajabk.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gfuqmandr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/ggxjvfnur.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gifghpzvd.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gdvzbcfbp.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gcszuplsn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gmautizau.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gwtowhzry.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gyuracjky.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gjtafvxli.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/glkmgtfrg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/ggahfaewr.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gxekcodgw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/giznmdzyn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gqywnfuhl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gpnusnyhc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gsnisyypm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnadaqkfo.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/goyntqsbz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/geqmgbixs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gniebfpjm.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gxvpzmfaz.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gykaydvjo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gbvkhsuiu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gyykzmbtm.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gqkteoorh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gylpgnonv.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gettrcxze.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gaxuuxhuf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gcbhrvray.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gujqtwzvu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/goqwnaaam.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gvxofzrvu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gjufweiho.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gcifctfut.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gpczyfbdl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glkxuntpi.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gczwrdglm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnmxqmxjl.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gqlppqlrb.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gaeyslucw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gafqngyyj.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gqpqdkswu.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gjqposkjq.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/ggusgwzfm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/ggjibyuhi.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gyncxmyhs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gdyjchgcq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gssirpbid.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gtlejjgyf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/glygixlpu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gmusmodmm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gmqrhptdg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gnygexnvr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gincrlasg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/ghedpihuy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gkwrgbsww.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/givxzvzza.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gaypsrcjr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gplhdfrit.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/guuhulgmr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gkkreomzy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gkwfmvmpt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/ghemrmyvt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gpbzejgcy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gyiqdrllr.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gaclqwpch.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gsvcyzllp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gsgttcbpi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gbzpcfbkh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gcjtlvoer.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gxbdrlwtv.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gesunnqme.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/griwlqebf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gsbkgszgt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gdcgiebkz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/ganmgtbsr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gcelfcnym.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gtgazgrbl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gqfwxwagb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/giwmlvocl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gvettzxuk.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gizqoqttc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gxotbpqdm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gctonqhjz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/ghfvdmbfo.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gwpkhbvnp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/guegvolsh.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gvkgrjtbz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gmcadicch.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/ggmrndcrf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gkpiiqwuu.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gsgontzkt.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gjntqtcfc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gezwzyexu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gohjzhayr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gsoosayue.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gerubzuya.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gvicjmltw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gzegyxgbr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gnvrzjsyy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gwzyfjvpg.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gdblcvgfk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gvicdpbke.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gfatvunut.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/giaiddwgg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gvucmqrpz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gdmqeiuje.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gaszgwory.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/glywmtyve.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gykhpbfdp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goznpwdos.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gtpnsxceg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjdyyhibc.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gtacyucyi.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gjsjyluep.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gitlweply.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gtuzmltpx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/ghazaujao.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gpiueakot.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gwpoujkix.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/goutvhkqx.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gtzrtfxum.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/ghesomrhc.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gqacziegq.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gmtrgrutn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/guvsvdnms.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gizohlfkx.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gkghxbedq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/goowdpvvf.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gtfdwneye.sHtML


<!-- 参考信息 -->