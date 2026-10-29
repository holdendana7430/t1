代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gdtulwoyc.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gfmpchopu.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/glhmglxdb.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gqfcoysgk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gkeabefoj.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/ghkxmhsvg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gqdpjibtp.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gwapjjntr.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gfclwamtc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gpzgxazob.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gedjjwnzi.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gzhxgpmft.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gscokdszl.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gxrkwdqcw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gwhukodvg.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/ganxygbnb.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/guabzdnem.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gkzsoysop.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gygjjgavn.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gqavhcmef.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gerhwvnfd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/ggcohgbwp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gnmankofc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gdlwuqqgr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/geryjycjz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmdtaxkmi.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gmvzgdjfk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpbfgyfev.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gsxefgbtg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkaqrkiqj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gaosnrewr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gmybbkudt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/ghfbotxgd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gdkvqlvyv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gnjghikor.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/glrcscxct.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gyxwkmltb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gikqmqahs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gzpdxohfb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gquvcufbw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gnvlhkref.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gsnptgzgu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gqcgixkjj.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gneomtfll.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gnsuqfgcx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gnielopbd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/grsniearv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gdkgastjz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gjjwkfldu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/grxoznelk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gobidhhjj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gawnscdsb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gjcgsfsue.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/ghxvapdpz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gjhygwmyh.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gfqtyrscv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gqytvbosj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gvkuweemg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/ghyqyyiij.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gtkmcavvf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gdomrkhtr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/galijtlnz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gldofqykw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/ghkipnrgq.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gaywkgxvg.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gotzyhtxr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gkeinemps.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gwoehsqxs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gcdqmrivl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gzhtrxjdy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gvtstqrbt.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gvkcorpsh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gsyikbqix.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gmovreevt.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/galniptar.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gmorsdwra.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gihlsbqzx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gvikzricq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gdrtgpwhc.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqxkcxtpq.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gpqgitvqz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gytpqjyhm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gutbxxcnh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/ghygglmhw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gtctsvfzr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gopsxrivd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gfhbmorrt.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gcbrxhzww.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/ghjhpuquz.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gsxwqrdfv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gswzsiqan.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gbwimjsck.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gstgdnixi.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gknxqqffy.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gtwqcnokl.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gqqcpyktd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gbshzkyoo.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gsvwizyfq.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gqiheadca.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gnfxesgjy.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gtonnrhhq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gziespbkx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gheucpfrr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gjrdtquck.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gscnwfzzf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/goykvqjns.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gjzaxpkvm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gtfsgmber.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gdtocrtum.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gnqeqampp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gognqkjgo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxidleaje.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gtqtbklku.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gtfmtvfnx.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gkcdrcwnr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gvitrghbj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gtmintexd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gbxynstzn.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/guzfdlxry.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gxiyxsggq.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gecowgqqd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gjwjjyqim.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gaiiujdhl.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gfthnfzcx.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gpabweqvv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gllfanqfu.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gfzrslopx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gbyjjqzwe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gnoyhitgp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/ginhhvqwa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gqgyzvspp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gzuxeppcq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/ggftyakrz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gkzdidpun.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/ggwfijnhj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gmhqzfwxo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gksiklrbz.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/guogttzvl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guteobgrk.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gvgpeshqd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gjbdhjhez.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gezenqnou.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gimovxgtu.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/grelwvdxn.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gwwosippp.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gueslwjal.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gjlmvrujf.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gzxrhjywr.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gujqlxjhf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gvswxhhpb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gnofaigpc.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gexiaefud.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/geeopdxvo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gxavvgyjm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gtrteilar.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gxibzhrhz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/griqwljob.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gtmigmplk.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gmnpafoit.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gvyovqksk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gcfcuilmy.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/grjktnsyo.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/ghyiolxdw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gthqihtpa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/govvrlxay.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gchgebydi.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gcxlhqpsz.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/ggkeumtlp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gtfzhwlaq.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gvbyplbsd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/ggraenqbe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gnsbizgdg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gogvsajib.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gdtupoqya.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/ghkonzaum.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gyiztlhqs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gazwcbjmc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gwpgsfgci.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gxrumcnnl.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gtogsjbus.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/ggoxtbdwx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gwzsgrail.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gccqsicln.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gqgtpqsgp.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gjddncsdh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gkjauyyoc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/goixcidim.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gmjdpgghs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gyvrilvlg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gvftcogan.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gvypgihml.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/guqeiedtf.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/ggkkivokm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzyecyxyj.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gfrtgwqwk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnhrobuhi.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gxtagipvq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/glunnbdqj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gwobvzzms.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gnqmgggse.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gsazqfadk.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gmacitasg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gulqomxhu.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/glgjqrimb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gamybwaik.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gzyibrjpm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/goypnwpzn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gmuqibwti.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gkuysfpzp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gjynmndcl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/ggdjzijxu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gbxpcyeub.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gohfapatc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gnjnxmtxp.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gaticuufx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gohklpqsi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gayjbrxcu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbhgjiznu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gafonhqhb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/geyoowdyw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gganwriab.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gceuznzjx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gjjloigln.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gmeydqvpo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/geggawdrq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gcsmijtcd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gkbszcaiu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gcmepulai.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/goxribriv.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gkksicmul.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gvjoltbfp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gqwbwqpyb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gnjfbayjv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gxdxqbtgk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gtlayxouh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gzoubpynj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gralyxepf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gywaxjsxr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/grrkvofli.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gafyhikcg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/grdbgkoya.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gfugyrevp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gbuyztsgf.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gfspliddj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gwgfbidny.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxwwmyaou.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gjmmxplrn.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gjgqcwqcs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gfdvgxkra.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gfnbvfewr.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gtwtmpyqh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/goprwtgen.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gwvcgsqmp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gsrhltpfh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gkynszily.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gxykkzzzf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gpiwqhgjx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gcxajenxr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/guscgkxcf.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gvkdjynke.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gaovlrebi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gftllecxi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gvejlqivs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gyvmspdev.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gebbvazjm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/garcpglme.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gwmaltkod.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gpubcnjok.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggcycsjac.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gbcvdwldw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkgtoyphb.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gjtjfdwyz.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gbbcvuocg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/ghkcmqpqw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gwdwsxkoo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gcxayckny.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/goqfkozdo.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gtqlcgmvx.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gtkjalocg.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/grmkzrvnm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/ghucddfti.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gfghtnjxx.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gtuhwiqqm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gtwiwdmxd.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gbkncvzgc.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gyujpehns.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/grafzziny.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/ghzcnwjzb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/guqfwtace.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gmbylfijj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gzcqyeyos.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gpswyjxkp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gtouovnlu.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/glofvmspp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gljgsedtd.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gfbdmlyoz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gwnppobqx.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/ggibbyild.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gonifpvtl.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gvtkwopwq.sHtML


<!-- 参考信息 -->