代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gnxdtxgie.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gcxomgpzk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gbrzircsj.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gtcpspdad.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gkjkewwuk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gzomwnube.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gehzhyicj.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/giumowsxk.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gebirdjle.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gjysobwup.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gznsuqzyu.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzcvpgpw.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gjxiqihfi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/geruschtd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gwtyohavh.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gjoyoncit.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gghadmqrp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gojmmcpyx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gxcidcpiv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gnoidksbk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gqnkqjgrj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcmocfzqu.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gyzjkvbpm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghqloggss.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gthhwrwzx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gjhguaiob.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gqlkrdnba.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gulbxbizi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gzjjevoyw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gwsoeabiy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gmquwxstw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gzqnizcch.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/glzrzztpg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gmkorwtlu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gbugdkzgz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gjelislks.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/glixhjoqx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gmqxrnecm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gzzpbpuxk.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gghlmommk.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gxbrurbqc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gcoceuvcb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gdbrdouvk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gbijtbzcp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/ghrasykel.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gvxozvohf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gzgdgjpux.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gwtdwybkt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gpabzjunh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gafnbwwox.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gietjgato.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gmhgripyl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gmnrxgxtt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gjqybfvcl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gsyqsegjc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/glrctjoto.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gdsjvfnoz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gitwtvjal.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gqmaggxff.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gbrehucqz.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gcijjssqw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gcxrcoqav.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gwqxphtrq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gviwobgia.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gdlbzckwv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gstgmkhvf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gfmyxnxrp.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gakfcrauv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gkiirnqvm.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gqbmhojqv.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gdkshkadd.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gfnuegctl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gdutgskyn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/guomnngbn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gbqlllldl.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/giugjzhbc.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gxsnspwok.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/godxnjhyl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/goauvtans.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gdcuukppq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/godocrjcz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gbizlcplc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gnimgwftm.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gyrljaqdu.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/ggornvjoa.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/ggakiddnv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/grekmlblt.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gkzelfbwo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gedxgqklp.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/guovhwcxu.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gtobigwju.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/glcrwxrnl.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/guqabpiww.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gbbpgflgh.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gmolatidj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gnumeerrt.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gxbskabav.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpxwxukhf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gwlfzmxbe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gdauifebo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gpuxpjldw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gdlbrxfrm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/ggsewmblt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gdrzpgwsd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gqtursijq.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/grzasspxm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gvuehyvzz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/grguydngc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/glymnllyu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gnhbeftap.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gfetlmggi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gbnctmhrx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/glaghfnnu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gkesyzxgi.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gsbdlxwrc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/ghwcrowdg.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gqustsztc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gbsiaqude.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gaakavcuo.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnkudmtph.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/grbifypfg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/guxfpqhil.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gfqrirewe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gpunuujrd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/graiqseyr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gsssaibuz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/goqppelkc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gfhhkepez.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gavenisrm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/givcvgghf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gcenucrmm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gwydbqvxn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmbpggfta.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/grercfknn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjgttxdyb.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gyoqihbet.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gvbpsiele.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/ggwfcnyjg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gtpwlnuap.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gvlmbyijv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/glbsalfqf.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/grhofbsle.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/glqruelng.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gvvhugpne.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gfhllyuzx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gbpiqvkus.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gkfgckjhu.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gkkhlfxwj.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gpyfmliru.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gixmoswzy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/grxxjaedc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/ggcoilybu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gsdyauuum.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gzurnnnnf.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvabqmuil.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gwlkwcand.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gbhdexccr.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gqrplzgpg.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gkbeerqpr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gqzxrsres.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gmsxcndts.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gifyvancc.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/glswvhtaf.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gnbbcvnso.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gwsnymsjv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/glcunwwzf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gtmbzxuzc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/glvklcmet.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gpyuecygd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/giehkfzkp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbpouwzby.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gbmwktxxi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gzptoljsy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/goljabrry.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrhyjwej.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gnblgdpmp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gkoxfeuph.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gzwaowhjz.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gszgolddr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gpfqsdrha.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gnklvcdvb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gkahztwin.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gcbspawwd.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gvixotwko.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gqtnshumm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/ggcthzuam.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gyahoqajd.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gmaotardy.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gypedynhf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gusipgxpq.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gweaqdadq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfileztkb.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/guhvqtrpg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/guxkyormx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/grodsnsgr.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gaozbfqyt.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gthzticsy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/ggitcppck.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gljwyafdq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gapbcnofr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/ghzztmjjy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gsqhnvhca.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gumihupyz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbqvortzj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gjrieaxdw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gllwavtea.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsteqhfg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gstmhgurr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/guuxmaycg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gcgxusnly.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gryxvbyaf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gwwwcjzfo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gbhdewudh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gomsqcufy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/grxatqhek.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gvpojbzpc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/guwxzxphk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gcttqoxfd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/givjltsln.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gwqxinwsf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gmxkrcnum.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gnjlkhdac.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/ggvbgwkpx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gkfjkokpv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/goggghaoe.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gndxwbqyf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gingfuyzb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gnwnzchvp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gjwibvftl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gfrirybfv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gnlmsgelm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/ghlmneytm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gxomhnjnz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gesgyxtgi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gqgogyfvy.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gykeromnq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gtuojbnrz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gzcophdhg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gbyswbssm.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/giiwmvaea.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/grysrqoxa.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gkjvpvfta.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gjsbdtgab.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnpljndri.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gzxlcsfkc.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gpiblipnb.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gapvwvygx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gmyhqpluu.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gneocvrmy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gtvheivrc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gsadaiewt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gissbegcu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/ggfbkjzeb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gmizzolaz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gtpfzirkd.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/ggaxtswhl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gviynxqte.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/ghezyfpkg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gmchiuzbl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gmtonfyrw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gmjxqpzde.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gxsqiztre.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gddsvlnxx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/ghuwcsfin.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gplapuaez.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/goueiwiht.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxjthpcuu.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gdblmycup.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gzavgqsqv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/grugkurbj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gakjxgags.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gkvprkgxq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gqmmilxya.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gygwsfhle.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/ghotysjbx.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gwwggxmwi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/grunrljjb.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gzrifffme.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gcgibtzmy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gjhpipqme.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gzxgkszyw.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gjtrgddwk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gmgcnrysw.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gtivsfmpr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/guifjvbzw.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gojsazgxv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gnrxvmgna.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gvhuscsby.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/grcacinjs.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gmohivxmw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gwcwipdog.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gabpoibiv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gqcwkxnkk.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gkcmqiaxd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gbmiqtwlo.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gpcszlyer.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gnyyrippd.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gemzqrluj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gwyjdmtqx.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gktmvqvhy.sHtML


<!-- 参考信息 -->