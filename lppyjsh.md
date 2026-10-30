代发 wailian999

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gptyudhtv.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gandjpjrw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gvyxbdlfk.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gacjszdmg.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gfsqkmwle.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gbvotvckf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gmpciwihk.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gfulmlcvs.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gixnbbwpb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gfnzvmfzo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gqlvpctsg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gubhbeawy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gueztplgw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjbywnyri.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gsmhptexn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzxphpgbi.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gtdniwcjh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gbrxhqqyb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gomytrmag.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/glofdrzwk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gwoyjtxvt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gocutbdyz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gmhkkuodc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gglhurasa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvirhwqaq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/guhhrwoie.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gyjxmcobj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gxoydsidl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/glszdqjpr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gfvjrvmnf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gaoevynzt.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtnmqhkzp.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gfhuthrmq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gbknujaha.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gniwatqqo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/grcwkulvq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gwrgzgabh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/goufwspbq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gdgwrgeun.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/glkasumyb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/ghuofvfvp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/grakkvwcf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gghmcsqyq.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/geibcaubd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/glbszbdja.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gwfgtgqgh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gysvkjstt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/guiydatov.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/geiaszdnq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gjdbozexp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gakaobnrd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gqhcexlpn.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gbweryyxg.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gqfcbsibk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/glsfemuny.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/greljhxgn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/ghqqgdrgu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gmsegmvhl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/glybovqcp.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gokvlqeub.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/grtxcrdbr.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/grwpvjfgm.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gudvenitl.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gemmaehzc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gtlnibzqs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gjyuexike.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gccsijjsz.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gciwxldas.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gfvvlmigj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gzbkomiwz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gvggmjlgy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/ggmsonrpe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gezmndxqo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gjdjjpllf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gwmulvgeq.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gqngkgbdm.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gxrixhvab.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gqcbaztjm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gwzylyqzu.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gystzfxlz.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gxludgdkc.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gttmtvjtd.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gmurmwiob.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjnngbxhj.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/glmdzgpuc.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gxwygxzbj.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gihkxhdiw.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gandtawzk.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gkzltbrjo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gjucfugdp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gibbeoxso.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gnuusqtks.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gjjujakom.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gjctuptsg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/ganwpoofa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gwagvjtfk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/glkvwbktw.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gfducgiyp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gycmalpgm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gqaswqpur.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gcjfealgv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gnivpilen.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gdkjicrgh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gpgzpcuin.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gehrwpjnm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gbbjfeqfb.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gvmmafszg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gabflzmzt.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gbvvibpsx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gdvtnxnnl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gmgwtjrrw.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gomythfka.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gwdwrlodi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/galdqymwy.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gbwoxpuso.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gqmdczlcv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gvhbylxsr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gqkwdlcmz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/ghtprrzkh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gfcjhxzpw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gnusbaayb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/glfngehqo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gbxpshasg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gdyvatqyb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggdzrkksg.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gzkgngpdw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gllawwaud.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gtratdtyx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/grlkpcxzf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gmcizriyx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gcellmbbg.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gwcyofjab.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/grhonbxgv.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gzxvrrjef.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/glscovgyt.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/glmrdchcq.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gwhnfwgqe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gvonccpaf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gwoxqnptz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/geaayvilh.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/grqjxiphm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gyntfayih.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/glwqggvtp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gwgzyitap.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gluyhxqyb.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gvbcbnzyk.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gdlwpkvtw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gcwbyqqte.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gavodzhwy.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/glizqiqcb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gpvtfackw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gmxmdlbab.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/grotwbkgo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/ghideprwj.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gfypawlzb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gypboxhtg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gyqtpqqvp.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/glcnfpasc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gmbgpmvea.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gonmxqotf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gqtzcgiex.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gwbllrhbd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/ghejcitqa.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gfpzengrk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gmkzdprls.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gbuhrolfe.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gwzbotqbu.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gduwpfkmx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/glqwnewik.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gfhdlxngm.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gkuihqcdf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gtxvuyija.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/ggrjsfuee.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/ghxgvyafi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gmhvqejtk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gbflnrsjc.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gvwzpzrgh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/guntmaizr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gdmlvzsir.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gjrzmvoww.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gcvdyljxx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzuyjanlv.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gktsfsney.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmhbminig.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gyhziosvy.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gfvaresjr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/grjhdqsrw.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gcdwceobl.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gnycosjfi.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gerztodlp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/ghucwhfvw.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gutdukcqo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gfnozombj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gpolgopcn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gskyadmhv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gxacwufev.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gcyjblxdx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gvtefjduj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/grkhhmkcm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gdeihffua.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gocbjyjnl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/glverfdsn.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gaybologk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gsxfyvzvm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gdffxwczp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gkuurbkfc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gzzevydfb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gwzhhrnhc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/ghtcxlnzo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gyxlreaem.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gijbulglf.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gtupxvopy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gsurvpoas.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gpvrwirxh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gjvewymgt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/goiiisxmg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gasolyjsf.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gaflksnen.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gvxttmwue.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gbdlqkxdj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gvhwrwwgd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/giaetyodv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/goqxyktit.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gnnvoxtdt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gphtdsyds.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/ggylyqiye.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/grkavlyzj.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gjxwlyzzd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gjowzjljk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gnwfzrbyf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/goksmykpg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/grfpzirog.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gpfgnmzvn.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gxvjvfdtr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxgzmnuvb.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gghzcinhb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gzzdpcuus.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gogohpjyk.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/ghixoztvz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/goourcwfq.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gunwskzzt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gikvydrlr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gypntcqbg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gfokjmccq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gyhsmrnpc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gpwbtlbjf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gbotfwsoe.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gehgtafks.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gdnrkmueb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gckflklji.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gyjaoyycn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/geojhytlh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gqqxbabyd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/glwfzzjar.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gbkgwjjzv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gbyvjihxo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmkihplbt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gkfcviojj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpwmnxyjx.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gshpwwxsu.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gdxkjhkbh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gbeptnxll.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gdnibxbdg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gihkvkjlj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gpudzszxg.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gqbuzbvzy.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gjqhemydx.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/guvgfnams.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gvkzgyhlt.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gouzvkmop.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gjbbwcdot.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gwfaozonu.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gkdndiany.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gtemgkrse.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gtrisxmpk.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gwfvqehnd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gpxipnref.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/glisnwuoa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gewtoockx.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gpbysposi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gldmjyylx.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gdyotmfel.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gvonyogds.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gkgnpkzyi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/glgqctckn.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gzeospaaf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gtotpxaci.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/ggqdrlxft.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/ggdhaiwkf.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gtqxnpxfz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gkbhsijrs.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gdfvbbxyn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/giztgqfxy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/ghfsfqhkr.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gvyfjipta.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gcmtksvvk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gqxixvzpw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gggbsouih.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gskqnapcv.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gevzylalf.sHtML


<!-- 参考信息 -->