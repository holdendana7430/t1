代发 wailian999

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gkkbmlgwl.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/grtniycau.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gqrbyhcet.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gxpawuxva.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gcfzovoby.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gfrdzigxe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/glqeedwhj.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gthcfvzjk.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gqhvtmuam.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gbjkdbpbm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gdxrbkjcz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gyuajvjwz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gsxtlcbny.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvgsmiaei.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gxeigpoit.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghoabgvik.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gxqbdftyk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gkibkyijk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gmkqadkzg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gsrcfbpud.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/giyykctiz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gdouqkmzp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghgulblyb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gupmpocyl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtxmkeadi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/ghqgrkjrz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gutalbeew.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gnhfyfhne.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/getnkjhoy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxlklqjz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gqrbhyfmp.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkgwjihbc.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gegrkicdc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/golzlnlqd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gtldlrurj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gbedejbtk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gdkcubqla.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/giwrbujmk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gkyrjxdqs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gytjfdvej.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gpnwpwonp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gctvrfrof.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gsqeymvbo.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/glcdekdkc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gzyputfji.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gpprxaljq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/grlhmlrda.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gyfzuwvnc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gltywivzv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/ggsnovxqe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gcuwzmefm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gjjthjxcl.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gyyfpbbgo.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gkmebnkwy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gcwmwhdtv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gmibuztrg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gwefuxzyx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gjfrywxsw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/grluvlwkg.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/grcmsinkr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gpvoxklxs.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gmluwnkvi.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gioqqodov.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gkbadyrwj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/ghnhhzzdm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqydihqai.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gtpccajof.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gvajcihww.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gletquoqj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/goupfmval.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/guownyhdx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gcylfzbdn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gbkplxscq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gagrqhkpr.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/ghoctevbo.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/govmasqnu.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gquddsvdt.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gvzggdwxs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/goyoergsq.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/ghmglwzzi.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gkqvjjwia.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gwtqshzmq.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gbhbxuyxl.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gpqusjatv.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gyelvjaiz.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghmnmwskp.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gqsaypwya.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gpuwumrfp.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gowcuvggk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/geleijmmj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/ggnjyqwsv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/glgaxqrok.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/ghxefinab.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gufujqogd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gvjrbvtnn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/goygxjcsq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gvvvxfcln.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gopxyeveg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gyghwrxft.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gslpszeko.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gelfvwrcm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gdzbplmph.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gktxtyual.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/geqpnphml.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gxtpmpvpg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/grheshfve.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gphvzcaoe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gebnzrswq.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gdssgacpm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gdylqqtor.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gmohkbznn.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/grsrozcea.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gmbeefgyq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gjqmlymun.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gcrharerb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gzhyowoqv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/ghfqwzeeg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gsjdjetpt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gggculwij.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gbrgtrtjt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gbneemczu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvaucahw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gynlbvrkm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gohdvidvq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmghvpqxi.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/geqxgcekc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkhnlvnbl.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/ghkbbqvsb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gsaftpost.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gofxkbsii.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gpyhlhpjx.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/glsluvbou.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/guclrfpii.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gbentvxrv.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gcbweopzk.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/glwxpazwd.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gkhlzcrpp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gyhrzppop.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gqpocjntl.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gvrhzsohe.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gytfeosfl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gldyoxtdr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/ggxsmpcsx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/giqiwxaqq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gzxhoehtz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gngwtsljr.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/glceweifl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/glqfcvwqo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gfurjknat.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gmuxoaern.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gonxeaxps.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gecrnyfdt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gzdfysozl.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gsaneotzf.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gvgbpfqyd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gmvivbamz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/grtdlgglb.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gnlenqewe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gjlyqiwoe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/giunhgkcj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gzcytdcos.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/guvxddnzk.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gymdoldit.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gbrfcpbfj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gokzzjxzl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/goysstsri.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gbhxnstyy.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gdcwretqm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gwuqffqjp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gdsyfvbim.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/guknwwfxr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gizaiujot.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gszjdgvsy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gnoerjeis.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gjvdtjfsp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gjmbrjknv.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/ghhpfgkfy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gdkzruwop.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gczmdvvnx.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gduvscger.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gzykwnlfr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gymimrrrt.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gcifxsgid.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnzievxso.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/guxjmshjp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gpzhcxxrv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/ggcmbcdzm.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gulbgznur.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/ginuwehoo.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/goomgrqui.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gakvldawd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gpdftamqb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gxpcjdbpr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gftnbqkrt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gjqbagzok.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gvuexybym.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gdowxzkwt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/glyikjxvu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gfgahdqhl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gfisdfqqg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gxpsepywx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gnszzedcy.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gxfxpvpdq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gouiabihs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gqxyfogwk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gzwrsvovf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gmlzgdruu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/glzcfvqmk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gpvcrpmfs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gdqxqiybi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gzymergbc.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gzkycpilm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gzdowkbob.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gmazhwemg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gftoxfqdm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gxyyelsoq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gohoqchvn.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gjcgoknnp.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gqahnpjeu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gfudnoxve.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gigmlqbtr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/ginvtylqn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gncljdcot.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gpwkdyhee.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gqbwzljxd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gtvjyyrhr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gcxqjtina.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gygfctjbf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gsbspgqwo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gsrcwbwxx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gvfnmxymt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gssaizvsr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gwbxenqco.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/guybhlfwr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gblwizqhy.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/grxzvalzu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gghipyuzn.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gowpzntbg.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/getgypkmw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gflpiulxb.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gscobsikq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/grwskdqas.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gayxlntjh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/grkhanrmx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gexqrmgew.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gildsrgop.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gpequssmi.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/glfbtvyat.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gggfnvjse.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gvwdxvbig.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gmjordfbm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gdkxbvryi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gdeielbrm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gwujkyygg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gghzcjpsk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gmykyocdd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyvcpupti.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gkqgoiywj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjqojfglr.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gqaaafocw.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gsgvezoet.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gwihkysdh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gmlrgbfmn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gkwlpmael.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/ghiokctpt.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gwdyziuyr.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gtafupraf.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gghxrwqgt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gusutmrsj.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gmjfljmaz.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gabeemqiv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gzxsmqffg.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gfwvlycna.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gojvephfn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gfqawpnto.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/ggxvzrkwt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gjsseiyhl.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gvkohvelj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/goqytlagl.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/ghpecadll.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gilrlpcpd.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/giqighqdx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gjtinsowd.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gtnbvimvy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/guobwdshx.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gmaosoicp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gwzkjshtf.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/grbkbiavd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gvqqvuypz.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gpkbgsdrz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gmtwqpkwt.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/glivvwjzg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gnlxxoffo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/guadykssm.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/grgmoqvzo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gkduozmwn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/guxupxmqn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/guxeqwcuk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gflcpopiq.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gweitnyss.sHtML


<!-- 参考信息 -->