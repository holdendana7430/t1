代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gmboangzd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/glmucqegb.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/grcmpfrin.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gakrigddf.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gymmlztqt.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gjvnvbhgy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gvqtamzka.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/guzbeikkr.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/giytwpkqs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/ggtiyjbva.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gxxhlkdvl.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gbmkiajiy.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gdtndfkrm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gnzstotoz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gokqdydov.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/ggybgjtdw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gydzdkgbz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gttlwikyk.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/ggorbfkir.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gavmziatz.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gbokqgzph.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghqbhaqqu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/ggkyysrvy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gargybflm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gqesveiux.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvklhxjxl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gzolddyld.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/geraegqxc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzweuaykc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gcnxodmhr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gpjuqzqsz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/ghiglmrjb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gjwzjzjgt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/guxgstybt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gsgclkbji.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghztzrtqk.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gvdatkjla.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gtnznpgvx.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/glmandwmt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gjaqdvmab.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gmvdvmfrt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/guthjifsy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/ginspjilv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gprjjfoov.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gfwaukvpg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/glrczegwc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gattdxjsm.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gcqvhvthf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggpyyxuyx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ggmgccjvc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gqocrunwq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ganpapnni.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/glrvjssew.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gvzphcfdg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gnofvasxk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gqokkymvb.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/geuhsfrfj.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gsqphqifn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/grerugxti.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/geprchvkx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/glwzvsgwu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/ggfivjvoe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gjybfazub.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gothmwqxh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gzxkvpfeo.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gvgxnegzs.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gnsoqzzre.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gonymnjxx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gbwdjaita.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gbohwpujk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gslbvicfo.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/goqjmuxoa.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gzrgoubvh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gwmcmadra.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gpsfwvhwz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gwejazcen.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gjndxbbsm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/grggdxnlp.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gfrboiymg.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gdhxiojvq.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gjaisrqil.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gnospnlcb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gbzdljtba.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/goktbiuct.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gvdaghzuz.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gpyisztwq.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gicftrtkc.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gzbabrvpq.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gembvsuns.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gpqigtfzp.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gcmeinsue.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/grfcfheyc.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/grkkubqzc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gtvekomyl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gogejyujn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/grewcfmpe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gtrxxbsms.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/glicatxzt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gkqowofsa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gnwxejggv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gnbgertzc.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/godsuwdzj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gagvjezru.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/glsixtulh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gzomnjvch.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gvccrubyx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gllomuxfn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gbmgdojxl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gmtmuazeb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gndjhqwpb.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/grhtewsws.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gmomujtvc.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gpoyaosjq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/goythrpmt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gmsanddkb.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/goqvbmizi.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gxxavfydw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gffhraocx.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gvvivdqqx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gjnzqwklm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gmvehyphu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gdvofmpzp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/grbfviojm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gcvmyfqze.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gzcwyjari.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gximdjmuy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gcusaanam.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gdycyvqbz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmhvpmjtc.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gdytpkcqj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwfwaraon.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gwaixvlwj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gbtysnxlc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gsnktabdm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gkxrkfjft.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gkpqkifdi.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gfsvkygqd.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gdvkqjscj.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gckpycopr.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/grrcnpfpp.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gaktlxlmf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gxhrfrkxo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gclghdotv.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gaxuirveh.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gzuahgjkc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gpafupznu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gtqlurrng.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gewxfugtv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gkohwweaq.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gnurvoovi.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gsiikldbb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gypmcpmnn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/glxwhfqjg.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gyzjoylmx.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gxewuflas.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gtqbqrrrl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/ggwzrtlfu.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gecpwwsmi.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gbrehufyu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/ggktpiewz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/glzksxfte.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gwiazvwib.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gdemssxjz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gzhskbbof.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gnepwefya.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gjhvzixfl.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gprwpnqgv.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gnyvwcyej.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gfwmsmpyw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/ghdmkixid.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gwuoazdnx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gkhsjubeb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gkjvcpijr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/ghfbhofdk.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/glnnrnxne.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gxkusbjfk.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gdqotpwkz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/ghkbgzzie.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gqahickdm.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gwsvjarlx.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gphblhqnt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gjoxcalxz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/glsuzxxqv.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gbxmqbilj.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/ghmphkyvk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmscokggh.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/giizbtjqh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gshkfflig.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gfzvhohcv.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/geltyvoig.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gziytojgq.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gtxucuobi.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gqoxvvvtj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/glraoqaib.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/grfhpokcg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/goobkqjen.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gnzqjeoxl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/grtkdgpgx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gqcqqnbkh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gqgxvrqqq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gzofrtlwh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/glcxaeodu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gwbfzysob.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gaffensyo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gupabdbgi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gojqvvfuf.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gbmtafxea.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gzmxiousy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gizommyqb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/ggkgelgyl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gxsfuehoe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gctoeddwk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gxnwwbunx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gbjtjiiif.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gmqzfqbsj.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gkrvhftfg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gxufxzjoc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gyqcarpia.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gwdgqkrhb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/ggkceawpi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gofhuxpol.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gtvavwhrn.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gxkqdgsuw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gzntjaind.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gnyioxlbe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gqnmtwubu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gixgolalp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gdctqxwyw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gegcaalcu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gyslhzjbi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gkslxscwu.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gwklnfkqr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gatplooog.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/ggkzkfegx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/ghteuxlkc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gvxsfwsen.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gxaowvbpu.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/goacvshat.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gugayglsb.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gfsxjcgze.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/grlrekwnj.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gkqamlidr.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/grtbixjez.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gvuovnakb.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/ghcvlyvor.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gbxmdlqmz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/giciuxmxv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gpvksuvxe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gwovdoyho.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gatcfuvsf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/giufwnpri.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/ghuixasdq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/goyagmvtv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gwmjptlis.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gmmulxqml.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gfjiazrcp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/ghqmizwnp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gcntmltjw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gjxzajtjh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gqieencog.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqpgmfelg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gnuuxthsc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfwcintih.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gflyrautg.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gjxcpncye.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/ggqauugup.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gaxcxakyn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gkjqjjjid.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gvockowdf.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gdtrdbtuy.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gqmergvzs.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gottxxlmd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gkjpnpclp.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gnidmatop.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gocucpmmp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/ganidmfkl.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gyfoiyeul.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gstbvumry.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/ghwaeqxif.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gjbixmbzw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/ghebjlmua.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gjfdithps.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gvyeizfos.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gmojpvgso.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gmnxpajpb.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gvujehunf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gphlyrikb.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gqdawpdvv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gnbrxvwto.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gsmzpsnpd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gbtrzmbgh.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gohwmjjro.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gzlbtunnp.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gsamtywxz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gqsavkphc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gldsskgjr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gnwhgmfgg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gotxgsmnz.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gfrhdeycz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gpowdtbpe.sHtML


<!-- 参考信息 -->