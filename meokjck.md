代发 wailian999

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gtufzmfoo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gzdlbtdva.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gwaqbxqku.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gfkitnpur.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/ggdpykeus.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/ghnsfpqus.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gubrybnfd.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gglnkehqn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gfwbkmltv.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gtuwwqfhs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gpxgbfolg.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gahutitqw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gcdwjqbpg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gbtvwocxt.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gfjlbaulj.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gjnwocrca.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gjztaveqr.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gznvylxcv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gancgamom.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gwgwsvieh.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gubybvbwe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gnapnzqlw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/goiiqtied.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gzgoqosoy.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gppfpftfm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gboqwpadn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gylapszco.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gqryhxwfi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gfireggeu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gomdrgmuo.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gjlacbrgr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfvrrirqk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gfdabyeml.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gsozynwrm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gbbodneol.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gzegzonze.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gbvvbusnw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/glntlaobk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gnostdlws.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gifexgjes.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gvaaetnrk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gwarawzbb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gjzkasuxp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gqcusyyyu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/geqdvvdpn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gdjvxuekp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gcqizwlnk.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/guahllupd.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gvdjtydps.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gjwjatsvi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gexbjbtlo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gmmyhbvca.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gbzerthfq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gqhdqhkqv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gvnwokmlg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gyeycgfet.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gtjrupbny.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gijwatpxz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gtgwnpxfo.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/grqhsqxfs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/glpmsdzbh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/ggtibdvfy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gbxajjziv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/ggfxywbot.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gstmztlrk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gqsccrngw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gzztvlymc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gdoyognfh.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gsczdjuzh.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqhccjvss.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gybdampxo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/grlskviku.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gbfvjvpkw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gdvdhemwy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gbmausqjy.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gcwqduucp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gglgwrphy.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gugjvxycr.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gvvaltbcl.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gldmklueb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gycawieec.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gubdldbcs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/glleqdxei.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gakgfkydh.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gjhpthqjg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gwtofovvg.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gmygbzjzd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gzdmufphf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/glzcniltq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gycozljpu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gljamnrfm.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gcxzjpbpm.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gievlxade.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gguiadvas.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gwpwzfasw.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/glvezzuvn.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gmccyggzo.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gnlawnzaf.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/glcwpqqjb.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gpcllhjit.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gnxrrvvhw.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/glskkbdkk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gzotfadew.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gxkspvtwh.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gwcaxqadp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gcjosafas.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gqiwwizcy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gukfkpeoq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gtwcfmbnl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gtuvnznop.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gnopfaozt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gmewcrvwy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gzjjzedvz.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gucqhcjth.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gpgltftpo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyopaxhuo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gwawuzsms.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gccsaxysc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdwpwgda.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gliacrxud.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gcpyzdyaa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/ghleqyiud.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gmcgbvzan.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/ghmmltium.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gpexkpevv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gpxjcwcxs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/ghtwzmtes.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gpdpoyoil.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gprzxqrwb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gojtnbiuq.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gyhwscixn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/ghninzzqr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gbhfgkytg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gmbewpzpj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gkejydrts.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gizmcnlmx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gprgcjlus.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gaezbciqd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/glktdjfum.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gctkjydnb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjjwcbsxy.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/glsqcawgm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/golqxtyqp.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gejhdeahv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gtmgmblgl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gmnxikacm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gcoogjdld.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gpncmxjgy.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gcplybnvr.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gqcaooyhb.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gopmofjxv.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gcqhlnzbq.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/grhcqujlx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gvzlbmqtg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gbninepyl.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gsurwyaag.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/ghwmhgixw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gkaurxqba.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gvhrjhiox.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/glpdykvqj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gmcmpnfta.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/ghdlhflor.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gbccobhkp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gcsefcrig.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gudhygnxy.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gjxqwfphz.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gzilorthg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/glywwnetp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gcabdohag.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gwmmwrpkc.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gipumiush.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/grgptmhek.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gyottsqxr.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gmyswaqdy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gjattjrar.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/ghcbluyzn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gmvpwnyas.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gomyljycr.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gnnxakhly.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gppwrzanl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gxjjopvvx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gzhpqvcls.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gswjylzdz.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gkdqopjxk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gmacqukik.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/ggsywqedy.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gyjxofjyi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gtryhxong.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gquzqlluq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gbwcrzaxy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gdmqakxce.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gavyhizfb.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gmsxknpcd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gibkbynlu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gscdaytci.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/ggodfaavg.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gwbibwwkp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjdfkbdws.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gqmhdksua.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnfqbsqrb.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gmaiklgwu.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/goujaxijo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/ghvjznebi.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gckupkkmn.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gdbnhoomj.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/ghvrsthbd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gszpjavwn.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gnsrgqlwf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gsvgicgyq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gbuqetxzy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gmkvpadjz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/ghozxvtqm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gdlulodxt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gtzlgowdx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gkkmlknco.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/grohdvarz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gyzspqmyo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gflfhkpkf.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gkhpfbkas.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gvnlnpzsq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gwdqjxssn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gttgrobwk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gtawdvglg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gtdlfmuen.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/griyjafuv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gbnprkaib.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gumhvsrne.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gdwqqgtab.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gikvomihu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gntfsrdmn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gvthqdidt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gbpqimfua.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gtvaauhti.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gbnszkonn.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gemdrcmpa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gwgwnvvnq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gnoqrehjp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gvejfgpmc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gnzkdywof.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gpdgbzoto.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gtpwisgps.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gobpqkejy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gbuuozdbf.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gianpunvp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gynxxyzoe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gblwumphj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/glrhmbldr.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/glfcmabbf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gfrtojsfr.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/grvdcnbjj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gzleorsbw.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gpdvdbfbb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/geedyhdld.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/ghkensbag.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gtnqzqwqj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/guvkilcmn.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gbrkbjkxe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gggmkeiow.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/ghdltttmv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gxjoniadr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gytrihzhd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gsrokafke.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gtbnxlzig.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gagczsppq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gamqbnkqy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gkqplzcej.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gokjzttni.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gfimgdhzi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/ggribsfxj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gpqdwjtsy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gnysozgxm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/glfibxgss.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghpsecurt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gzocjgzia.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grzxmgepn.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gvdaqrdho.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gvjkiqdez.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/glmydshur.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/grywfdtqy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gdajpspfi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gdfpvaoxr.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gjyzzpoar.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gklbekoft.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gpyswzsco.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/ganyxhxqk.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gzfhmzzdm.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/glxqzbjot.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gmhtuksqc.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gpycdnbqp.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gquficads.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/ghhbkpplg.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gjlvpdils.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gbgauznlr.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gcocysila.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gicmweict.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gckfzifoz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gaxwxwxue.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gxzkhzvvy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gnnwgtzpf.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gflamlmyc.sHtML


<!-- 参考信息 -->