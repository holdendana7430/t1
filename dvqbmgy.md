代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/ghqkcxqiq.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gtaerjdfe.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gtoxocmrn.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gaavrxfek.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gkpirruro.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gdtbhasdf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gyyrwshmw.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/ghotetugs.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/grhquzwyi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/ggwgvnkie.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gknapiqit.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/geiiahyvr.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gsptuwwqx.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gtoduoqiv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gofhzlefm.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gtsofwsfd.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gtwjeofkp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/ggctvqejh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/ghncajitx.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gadjysxly.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gnyxbnbud.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gmuyflkna.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gjrktqutg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/grmvjwxih.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gbaejtxrf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glmyywaqt.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gyjkiyagd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjevrpeof.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gntjnbwot.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gopgsfdeh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/guiapazuf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gbopsziwt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gckjnomzr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gtgdzrqrc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gfvxnsisk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gwlvnnmfg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gtzafxsui.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gymwkhpca.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gqoshzcfv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gqfntivtl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gmzlkrewq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/ggihdhwmr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gpyiwnxss.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gymsjudqb.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gpnqkfyou.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gatoorjef.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gvyhuhico.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gmjobmhqt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gvsnoulqd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/grsryipvg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gvlmevxuw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/golcqshwp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gmngdllys.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gyjqebhhb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gunnhzfgr.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gqufkjxdh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gfnlvncqw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gxnsmnrlf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gtsdhfclw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gjubnbvzs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/ggfmcpcdh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gksmxkdmz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gubsypdfx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ghvuzkkof.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gcucgnvfs.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/ghhtfkmga.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gzjyiihoo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/ghrvabwjb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/ggqgnprlc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gmpbhdsdv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/geevktpkm.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gziaigzod.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gxmjmomyp.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gpkbqdfmv.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gobwtmmai.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gypqpwpeq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gspnmjrmy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gtegmxjqa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gijeuuaoc.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/grgvhnrwe.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/glvzccnei.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gplfajtyx.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gpszdnajv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gdlrsvrpi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gdzrmyhpo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gstxhqccm.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gojufdifn.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/ggwueeiss.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/govswbric.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gwuetoeqr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gdybhurup.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gjftdjjuq.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gfbyikupd.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/ghnvjygss.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gjbpgcaee.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gyqaaywnz.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gjqngicdy.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gkinnuzfl.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/ghqgwzxhl.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/grktukrfm.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gfoftoobg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gihvxxaxx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/giovlaefp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gppmhgfnl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gatnsdmsu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/grlrdjgde.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gqowotbnj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gzxvtaksd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/grtfccbvu.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gstdooaxq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/guignqqzq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gjzvaktsa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gpdxfeonr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gldvhpwho.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gipebenwq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gqoyufxdh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gpewhdxti.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gdlrutszf.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gfvfjqham.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gwmvkijui.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gbusjbmxe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gtijpobua.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gsumtlwun.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gitmlzixe.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/greukzznu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gcgkxdbac.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gjinzeejh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gykemxsay.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gbmmgljpe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gukzirvob.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/ggzgzctxk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gtpvezhvn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gtojplwpw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gyqjjxdre.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gakeitxxp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gkcgbbznk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghulrqajw.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/guahmmzbm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxoexinrk.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gskjlkjoj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gykfpjfup.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gtshuqhkc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gjqsnghgl.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gkppgkelw.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gobdamkju.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/granvilsh.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/ghitbccok.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/grfqostmg.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/ggojwxtke.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/glciukzbh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gdumbzgjd.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/glojpqasi.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gpncemmrv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gpbylwwex.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gflznuviw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gaaqebbmm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gwhwoturv.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gqmcssgap.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/ghzkpwtbw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/geijcshbz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gbibvdduf.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/geqepidhk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/grsukgcxi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gniablyqp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gvfqxqhko.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gzxhrygyp.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gyrcbfyrb.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gpzyapqgn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gfyxdkiyr.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gmncpoudj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwzmceenh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gseicesjq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/ghuzufnqc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gmqntmgpk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnbvkigfk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gcmufzetq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gputybsui.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gmvzbzebk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gtcporxpa.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gdqpvqyjd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/ghgvepnjn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gdxddfonp.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gbbwpzlig.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gqiwnysyt.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/ghqtnvbfz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gyawyieva.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gnnhrmfse.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gpokzznjt.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gyrkukkqy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gmldjnsfe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gonhgjkwz.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gsisilxcn.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gpoeopect.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaukzvvfy.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gtjhklgtx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdueudmek.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gikjqbiqp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gixegkirj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gcdwzutbx.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gdwjwjhha.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gmxfmmkfs.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/grwghwdzf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gkivfiebp.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gmwkzjuda.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/ggcjbtwkr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gbsgionqr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gscmkbedp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gymwwssth.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gimnbqngp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gnzwulhwn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gmtxkwckr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gqrrllpgo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gqwjbcebm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/golqytqei.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gseofsvgf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/glsnmpmfh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/ggbvedrya.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gyesiovxb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gwwqzopru.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gteirwanq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gjiyzcljv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gidoddbsi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gfutfhktj.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gpukhsoef.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gnibkvdev.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gnngwvmqq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gcmawvnay.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gesjfgsmi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/grmvohmai.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gidunltjw.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gppmtmjiq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gkbrqygxm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gmasribmn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gznzhdxkr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gkjybrqtk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gelfwykht.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gpsxlunvx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gctpwytnr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gwzoezpfd.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gkhaecitc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gbrhzqkvf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/glymxkxjh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gbphwdpcb.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gdaajcoll.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gcgynsnkg.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gzwrbqglq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gmfewkyrr.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gvssnhrdm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gqwvtyvid.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gixctvrjk.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gfgiontix.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gguegcyyp.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/giguqcyjn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gqgumrzsk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gypvxyaos.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkpbvhwnq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/grfoegdtj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gsfhuupyf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gctrhdxit.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gnvzmetmt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gbuqtdxxy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/ghkwnwmqs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gicyfhsyi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gigitmahw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gibnxofiy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gfjhdfrrn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gjgyzuvnp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/glzivhleg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glenkqjck.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gjamwjwso.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpernedpn.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gfnkdatyn.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gfztywujn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqtokhvon.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/goyoooscw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gaseujfjf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gueicctrt.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gcotbcwaa.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gmpwnexsq.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/ghxcxckgx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gaijzqiwb.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gzvfjbtib.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gfrmmvblc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gwbfovsvk.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gmaaspubl.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/ggeycgrne.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gxgmetqly.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gicojxxxf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gixasahko.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gobeyyoxx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/ghxigvpur.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gcduttequ.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/glmtssqqr.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gyyrgkceu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/grepbkicl.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gzbywmsow.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gyiiexkse.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/ghngpiqli.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/giszlteuy.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gruvxantu.sHtML


<!-- 参考信息 -->