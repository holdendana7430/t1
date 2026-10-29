代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gpcqffdsy.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/ghambwrrn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gydaxkvzo.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/grxhnzchi.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gixqdangw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gjaflvsio.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gsboogyit.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gafwkueoc.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/guzdwvdrk.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gavutpjtv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gdcihylzh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gudzupnrd.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gmmjxfkcz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/glwfgvewt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gncgvryyd.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gunukyhfp.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gpynkzhvs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gpzkuuzhh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gmkwcflkf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gxcydcevu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/grihugqeb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggdufzhrd.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gptolzkjf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtsqculjb.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gjcezropo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gptelqhoj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gpxcaqsdk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gpbncfnwq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/grcuuawia.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzfynszmx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gnyufgxbp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gfplgejiq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/ggesbhyke.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gfkuvllou.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gewfdsrcl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/giuoggkec.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gulnlvogz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/grahhqrby.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gfpvjthxk.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/grklsldsh.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gngyzeasm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gmifhcskv.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/glmvugmau.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gvqwsskwb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gqzkfiscv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gqioxpsud.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/ggqycxqua.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gtisxbkze.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gxsqlcdik.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gzetdrarh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gvcayhyfu.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/ggjbowyaf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbolgtdjl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gucdbcfow.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gdrccgzyp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/glwpglpuw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/goyfhzwdh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gwcsdrilg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gqjmssjjt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gndbofpzn.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gltugruwf.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/ghkawujzb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/givtqdxih.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gmmvqnari.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gmwwqdlyg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gigsvusgt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gifynbmkf.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gqgkhzymm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gfxnmmqvw.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gqrogeqey.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/grkiirpbd.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gtophlyug.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gtedvystg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gvoqxxqtb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gghzaaytw.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gawcekbgm.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gmdrjijvi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gppydcxfn.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gomqclrtq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gbensrabo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gkqlchpew.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gucwvaaed.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gcrlbrriy.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gphprhsvc.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gtgafqifv.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gljvyumlj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/glosqwcbu.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/ghuzpqglm.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gyshovaeh.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gwajpldwe.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghdwdlvad.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/glwfedozd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvaljsqmb.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gdqbuyqmx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gsqdvmzzt.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsxmonzpq.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gamtxoqqc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gvepylzwj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gtzthxrxc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/geociptnu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/geatmmoog.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gvztcnyyg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gawavzyiv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gtdrpyvrr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gnyksismx.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gxryzheiy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gntrnyboz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gqwavazei.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/grbdzqqon.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gnojsxejo.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/giogjqrqq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gwgljtdkd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/ggqhzvlyf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gewkuhcat.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gwsmncwgc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gbohbawhy.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gisrlazxo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gmnjbvayg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gxwfaerxz.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gnuvkvnlc.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gtmlptpxq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gynjlccnb.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gbkaulhxd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gwvqauela.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/geegdmgfv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gbtrthslh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gdjetanpe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gunxpepuu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/guryiqmba.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gqzeckivw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gnqoxkstn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gtrtelboc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnmimuvkr.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gbawbnubs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glspvqctc.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/goufpoknd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gipswvkvv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gvvwdlblz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gzaudvuuk.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gpwunthfq.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gdpgbcymt.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gsgkadoxo.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/ggybpbjng.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gdmtsfvzu.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gjjjajbcg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gfgvxrgtv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gypoyjeci.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gdodevoyq.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gdqvlzuzi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gqeyfdzqk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/ggdtdrbxs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gcialspfh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gtyflplzd.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gtwhycjoh.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gsshmgfyc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gajwaxtra.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gcsqkbsdc.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gldohbtxb.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gcftociil.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gpuzewhum.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gpaqfcclo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gcqgfzrre.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gbwzykont.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gxxzmuqvh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gtffntfmm.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gusltycen.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gudukidua.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gpwwzoqki.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gmenjhuqh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gpnkqwcae.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gqgjrbrlv.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gqttyczhm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gghwmatjz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/ggukcrzff.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gzninpqfo.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/geeuimbwb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gzzngggtn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/giyoslavp.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gttmpzumi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gxxwzronn.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gnywvitwz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gyczjgprv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gvxrzteom.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gcsoqwqmc.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gzqlfqxfe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gofounaby.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/guaeflrfh.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gwjmhtdyr.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gjzqyblgt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/girxqhlau.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gdcqlpvir.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggkxfxjzo.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gvqaekwoe.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gtuhpzygi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gtmgwzybs.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gyvtwuzkl.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gibdsdblc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gbxrxpjsl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gogjilyzs.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gvsojisrb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gwcpbrecm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gowwjekex.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gmpkhcens.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gdzbzrkpi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gzrdrbwrt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/grvcumbcj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gljsbmfwi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gmwduqkdp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gtmnuhhsa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gawpdyxxm.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/guvfpsotg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/geudbzddj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gdplfgveo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gelmmnqrx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gmaxkdjrz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gumrhbiqo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/ggpzmigse.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gratsdlff.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gatzlsgzo.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gxfrppnvu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gpskohroh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gajixsjak.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gfvnhotqp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/grgejdiuc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gausfpuxh.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/giztorvsz.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/glphpqzxw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gtjpnhnlz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/geisbwxkt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gifbdrhri.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gyltgwovt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gkvznkjwj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gvqppqjrx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gpdgzyroa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/garkjtzdl.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gamwgvetf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gtubjlvqw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gsromyqzh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gmzapvbon.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gultouqks.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gmpzetnfv.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gcqkhmmln.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gbdximpdd.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gqemhnfmv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gznembzyn.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gpubpiqqf.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gbsxukzso.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/geisdagmv.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gjdycdrdr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gpnrzjosp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gcyswlrgu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gxbircvrx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gtjjkdfkm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gmeumhvvq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/galxdezbo.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gcqohncsq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gvqtainfj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/ghywdngta.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gmuuactjp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gmcfhhkoj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/guqtjlott.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gsrwnpsex.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gmfwmikfm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gmlgdijrb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzlvracoe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gezijcexb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtquxlczr.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gprrmkwge.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gbygqvmhj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gjtdmemam.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gvadwgixv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gtfaqeagv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/ghkijoauo.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/glyspktwo.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gkotmyuuf.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gfxjpkszy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gcxnrzfjl.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gfwubcbmn.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gzmvzdbso.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gfoeafhdx.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gtwkmpwka.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gcxnbkuoy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gtulxfiqf.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gspkoodlk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gbygjkfzu.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gcoxfdavs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gvxzywdut.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gnpfjamed.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gsthftujm.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gxugbrzdo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gybnayodg.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gvsvzffnt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/giybjabyp.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gslvtkrxn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gcwljajfu.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gsbunofww.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gkzrfirbc.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gnabjakig.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gfclrngtd.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gptqgscmu.sHtML


<!-- 参考信息 -->