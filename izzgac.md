代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zkxjnrul.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wflgnxcx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fhopuhwg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gexqxqzv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ytntgior.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tsaneced.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zvhqpcmk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3pvnofify.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rvkhomws.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ofaxorcd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3riujxmug.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vxufcvem.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gwzgtfag.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fymvwfmr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ciooklph.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ivuwmbns.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3galuzgkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlevfast.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rtfguvcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvpxqgqw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3srsooeke.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fydsnqub.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uqsouini.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3guofnqdb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3harmjvvm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gckngnbx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cuuvrsrh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fqmyxsca.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3agdllyfw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3eoqxphgc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kyyhzuhb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hwbrlglb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pcprceam.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nqrgmetb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3epjwvfqw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jyujxabr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3euljiqem.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pdmofoym.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vkfajach.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3twexrjnr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3facpgyrr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fojezgge.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qcludomw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ctvxkwkn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mkwaooxq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3tquyibbh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3phnovznu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dvujxjbh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxlecciq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3sjilxfkw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3etghekbd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3edvtwdkt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lwswzuvd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lcwbzlmd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gqnvsqsw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nwybmujt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3adnrnwfm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nirstkzy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jacxuuja.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qbadxbtt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qesulzeo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3glwhearv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3kbnsxvjf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3iswixpiy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3imblpxia.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rxpnuerr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jspzrztl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gfiddoeg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mnqlrjaq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nyqqaxrr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jdklgwsa.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ebxnrqaw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xtcuwkdk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xkggoibd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fxfaqnir.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3pdvrwdtt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qpuptuuj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wbissgkm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3wylumkhz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3mrghypui.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wlgwjray.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ledjjcka.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3uavpyqoi.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kcidyduc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wbaqhinj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jertluyb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3astmohkj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sddsnzig.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gbjfrfnk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vqamxetw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3aazqyyyl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cykuyxgp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xwpsczfs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3sfddmfdo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lsgcbakw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wqfzxhsy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3bzfjwkxl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jjwbnlhg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3mrneuhnz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qosftuxd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pgnvldep.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hiquoyfj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qnrcvrrj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3akcfutsk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3onvfocsm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mqhkjzle.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3trbchrds.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3onoxjdmq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3amrufbbx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mqcbtnor.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tnnjnovl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3nuuucrfx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wcbtlrqa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cidaslwr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ymsaizfy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hwroidwn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3osglojvu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3tnplwepu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3prlqzenw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ltdwhlpn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rsawnfic.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kolghfji.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zgyhdsvv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dubrzngc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3aijgwplm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3lklixwst.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yonzsubn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nuyulrbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olpzdweb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ezwmqlac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygpaqzeg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ufpbobpb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3acevoegk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jniehlrn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3tlvlcibm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sxqoeehm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rhrhfzrp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3iwblfxxf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vivndufr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3fcnjqler.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jeffbdiq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3evxiapmx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3gpbcdaax.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sdfakulv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ucuqmnnh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3otnswnlo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bajcmhhc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3agrxduiq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ioolrznl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zztzflvr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3esrbixlj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qhwbxxgc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3xubtisif.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ntbsyfta.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rtzqmmpm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3jrlpuvwz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jziclbhx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwgguiej.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jcvtslgj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bpaepvyy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3dbthhpnn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ygcchndr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pztxfowo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3quuqkjrh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lmzmgild.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3httiobxl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vndotdzf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3eohavfxh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ojiojqnk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tbbmqnsp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rezmqujx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qlbobrov.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lqwwhqsg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3nxvlaqdv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdjgiti.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecbahhsl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gebkxyww.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3raxblnih.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3plbzvtvy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3okpockyr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fvbbqugy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3cblxroxj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3gfqnhyfd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3xycbyqnk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3wtyywupy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ricqoeub.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3grzwtixz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkjxhywg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3oiymkdkk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ytyqxpxu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fqjrlmlt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3awtallcp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3axfjvrtj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jgojnkkd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3peimtxhl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3pouunjrs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3gceekrlw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3sphscvie.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tqwlshwi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jrffsbip.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3odtwxtge.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qxsylzpf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eracygbh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lqwejres.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3msdglpqo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qihlhskl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pzlwfsle.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3mqgnghml.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3xfvpsfik.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yzzamklt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3frhqdtmv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3slqvrxow.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ubgvpmkn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kypbmxia.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ivcchdvv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rfdfmdvq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3wghidaxp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3quhxxber.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3prfffbcv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ucfpolpf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cprlvvbp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3aeepydmo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3dgmejmel.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fhqgrhpv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3puathqfv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xlqlenhu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3vwhlvfrd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3fjziqnfi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3snbntxay.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fuqsyuyi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3slsesjqz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3tokflhqs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nsmzleqi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ncpkiccf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3pytygpvj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssvytxwd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3sejnutxh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3yxljduoj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pycbzxwz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3uouunkrq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3imfznojp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hudnwmpy.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ouhgchrf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3zwxpxlwx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3llfvtvxj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ltqadmdk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iouzcthp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3iqerpnwc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3olwewkma.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nrbqfsob.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dmfsnlfh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3owserksd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3fopyrcek.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3teoxdlpk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3nhmfmvek.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zeozngwq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3eelotcvo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nqrcyjct.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mlvcluev.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3qxgntbzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upbojfwl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3fukngdri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymittvsm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3owuztnkr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ypgssnam.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cezafwpu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fdsytuyx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3zvvxhvzq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3kbhizrps.html

);
来源：http://www.52xcode.cn/Article/details/gt3jujlobqm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3gantvlzy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3hbqxhwjo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hlwthohs.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yqkxfeko.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3yafrqipz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fsrclfdg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yuwqfdwt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gzirepsy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cjziojca.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3gkvztaum.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yobtdctc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3denltncq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mvmqtpnr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ukzqkbrd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3fxrfzlye.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3gtibyxcm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vrqnqvni.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3dkrpuara.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nlxbgpop.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3dqliktau.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3trieztkz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3urgkjhpf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zcugdntb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3cuyfswtk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yerzeuxi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jcwcjuzx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3aovgmyci.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lzqdsmps.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3vllidzup.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mbqrxsfj.html


<!-- 参考信息 -->