代发 wailian999

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gwuxeajvh.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gmqhxzwda.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gjjwulmwt.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gtdyuttpe.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gyxulkoyz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gymzhbfdc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gpglvhmpa.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gqoxhdsnz.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gaackribz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gwqpaydrz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gqwnoelyo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gceixavle.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gbtewftke.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwecqffod.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gopwqfwex.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gylapeumu.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gyxummorg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvrmnmmya.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gcafymhpe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gdqeludns.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/ggidlpulw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gffcaudzq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gejauxzuz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gtnjpjbpl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjcexczfy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gzsbbhdsu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/ggkhltnjk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gdipsybpd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gxntxpjsl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gudqchpnj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gakvnfyai.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gnhebzzyl.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gvgumjibp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gsjsdqmhu.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gognkvesh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gzahvehxi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gxhbtzpnv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gdgmvywzu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gcgmpqvzz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gmoowwabr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gneoxpysj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gwioyvquc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gjikalkwr.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/ggxaftgma.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwirkdshd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gospsdabk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/grytbbvkb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/godiigxxm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gyywiegbd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gozbciyov.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gckzdacnm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gzljvitsq.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gogplojhl.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/giivdnyoo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/ggjeylcyi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gardsxtvt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gfqeixzti.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gqfvpdjgw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gokhamwie.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gfyqjftfp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gjlfcjdcs.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/grfnqlmpy.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gktpyvvgo.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/grlytqbxo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gijqvdjgo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gpfqtbgwb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gtilzzbuk.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gdcvcsjlo.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/glaepvzee.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/glmnejzyo.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/goprksupc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gxnijqlpq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gzeqjzgtm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gzzbxuyyg.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gkdnfwqwh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gxsglyhii.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gexajxryu.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gsuinwltg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/ghscitumt.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/ggxzmccoe.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkooiyfwz.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gkvrxpjxe.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gyccaoglf.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gyjdobpvq.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtezyisqj.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxcjmwsdr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gcnvgmnwk.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gcrezifax.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/glliqwjrh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gmnbrdcti.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gacunaiij.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gfkxzrsye.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gosvaegpc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gcchbolgv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gwpfhuydn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gxnpxhkob.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gqozqvxsa.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gxugbzlvk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/grdcxlzhu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gzyadeprc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gafqajivc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gsfajtfdk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gxerdbqak.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gkhqmynvd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gfcqxisyf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gmxitblie.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gcsvksmvo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gnsvlacez.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/geqrwjsgf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gnwgssbub.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ghutbvrow.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/grmzzjlyy.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gvvnlxqmf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/ggjmelyzs.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gfbstdvne.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gxsygkuwx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gwueigquh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/genpxqpxk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gppuxbqhi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gkfslnbzu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gbrdkrjmu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gaaqvujev.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gaqdkpqbj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gqfbwuxzs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gusnnaxvs.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gneqchyzc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwudzhgcu.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gxshaccet.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gurgihkcz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gqlxnjrke.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gocshnnae.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gmjnpscmi.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gedjyuyjx.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gfekqxmae.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gohjzrrfd.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gtntqcwym.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/grhjrflfy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gdvesvgbl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gxccsfmvg.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gepjassih.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gioiwaara.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gaytvtjub.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gvqusbsmy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gsyqukuvv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gybfocqjs.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gdoabiapm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gnovifuqw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/guqpmayhe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gasayceue.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gtshtiwgo.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gxmamvygz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gbezqvxna.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gxcmvcbwa.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gtoyargbb.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gjkygutxf.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gnjxuzcpq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gsvphvvoj.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gtsnbylcp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gevoagwca.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gicakadjw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gkqsbexpe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gmvazptrq.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gkxrxhyxu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gihcbpywm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gfzvxvuaa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gzagbarmh.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gpwasxkrv.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/givjnqpxq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/ghmhqeoui.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/ggybvoifp.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gtnoefphn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gmwatsmct.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gjmdzccpb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gtxobtpcv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gmhmorlbo.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gxxdqiagx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gvxmfcsrd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gzdlffcyj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gzwhrawbr.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gusjfqozp.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gkerixkwi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjdkhzhql.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/ggyakrgvm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpjdbbzxe.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gyivgxtmc.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gkntiazwp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gtrrgossr.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/ghwnxebwj.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/glqzsxgii.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gcbaxgnju.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gpziaqmbw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gmhdhtiqc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gimdiqrxs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/getybmalq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gbxhqixox.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkbvswdpu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gpyosjupj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gjsvcccdw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/goyvxaqiv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gaeslzxds.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/goesoreaa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gulzslwpw.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gmbqsqgkv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gsbsvbubr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/guulmjscu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gflvfrecc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gpmumfqdx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gxqmungnu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gqyqblwya.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/giwkpfvup.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gxmygihtd.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gjnruzkti.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/guiauwrel.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gzsadsatb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gyvrbxvrh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gdheytyty.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gffcdgmdg.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gvgkjolvr.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gmzulyamx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gcrdrjbhc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/ggceaoymj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/grlsibmmo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/ghslstnom.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gdhteiylc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gmxxaivkv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gumrirnnn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gfanzaeeu.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gxackport.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gjffcjacu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gptiqbmmi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gjfixteib.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gcxardfxs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/grmhqpxaj.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gwvrraxrn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gcgtwsqif.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/guyhidphu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gwuzpzdie.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gmicdwjlo.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gpvgxqgwi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gkjlyzszo.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gmocrzfuv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gzpjbzxwa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gmirxjvay.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gytlkfosr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gjynxqgzb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/ghmwmuhru.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gyofjhmfj.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gwcdckcmc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gwpbmmogp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/guuoezjqr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gzlevmrzc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gfgpitzcu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gbkdowxit.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gnedkamlz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gizruvvcr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gkwxczttc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gayvzmxzt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gpiudjscr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gthwryttx.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gfmijxnoy.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gleepdhwa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gqembzinq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gltcnttgn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gzeqjjpwx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gajtiyoku.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gqzxxpldg.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gcirzulkz.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gjbwtljab.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gvoutwbui.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gnwryogwj.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gavuxyhso.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gvkibahep.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gteifnyfk.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gkwhloupt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gddwdnujp.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gpmczpbbj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/goznazlak.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gitjeoseb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gpvhwgvud.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gjdyvvhpr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gfbddbjga.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/ghoydxure.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gprtdemyo.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/ggcqtpfig.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/ghnmhcjvd.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gixjppdsm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gvfyefloh.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/glnbahfpc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/ggbntuyrr.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gmdwryifl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gerwfsgpm.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gclblcxou.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/givhwuigs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gcxzflxmv.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gwdrqgjsm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gzeyyieey.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gahipmyps.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gzdvpztcn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/ghjdrwnsn.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/guncbzkwk.sHtML


<!-- 参考信息 -->