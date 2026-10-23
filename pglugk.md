代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3avrnshmm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3lajpedvr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3eookmypy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3rgoivmsc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3sizxkyjf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lrjrqara.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ucubecvx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tfewtbig.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sqaxqwvk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3bwrdnoyi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3hrbeuyqv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3exepzuor.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3kdsftxwh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3atnbsybi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zitvjewe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tjhqkjmc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ylbopedg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zoxyhqub.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hggfjawh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zrceyptc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ltcyxqit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbrifvti.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3sytrlvzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izrlkicm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3zmjrpthv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmvlvamu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3foebzoqc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3woyddzpy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mnwzrpqv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ptobmybb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kthpaejs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3khzdopjg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nvtmuaod.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ioqkfjvj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qihsdhyy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bfmnrxmi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pptrtqqw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qbhqbath.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3immlynji.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hvktuhnh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uvhleblo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ekjfuipx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xutdhqgr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3meppjlxz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xhuczhvf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vmcawbgt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yicpqtfm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lsuhurij.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3usiyhqod.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3yjyhpwey.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ltefaeav.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3iugkhkjc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dglqkdto.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pbmoixib.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hockjqxl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3iwtjgmyd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gbpufruy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3eianzntv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oayrkljf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nlyxlfmw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pjbvvgep.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ejecrxqf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jemogayi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qyrladyh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jntgqkkt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mxbejtfu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3adzhjpho.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3mqlcegxl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehjnczpk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lalegzpu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kwixoirs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zmullupq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nwbdmenc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tdgqlllt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3cixrzxeh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3pskkdyuh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3glbtozlg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yljvlrey.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ffimzfsc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3uhfuxopq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pcrszqgd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gdrsqjek.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ailswbru.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jnaexqfx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tuulyics.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3mkulscrk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zpbucglf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3khkoxyyr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cuizcbsb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3uinbtljg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ihccsjud.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yzvwgkbj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dnvnpjhm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rmecxdlz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ccebrtlr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ssywuidd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ozxjpsyg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bflofpkm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3emknkpex.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xczcwdsv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rvhdjoys.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ojiqnnip.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3sodyvynw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qvlhkmyf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vrdjwqmz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3bgrykbge.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3yxljokfi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfdsqacv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qqkhdpof.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wrcvgcxg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbskkcbs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3yotvirac.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3inywuuqf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3hfdwyvlp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3pgmuuhwa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3okthancd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3imjhzdjl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3eyhwxtlt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hguilnsm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jmstavjj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hbiqwvof.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3nyfzncng.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3muarvuas.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3lgootqky.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gnscaeag.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3slqxdyhq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gpcibxja.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3avciyjkq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qyfylskx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wazmlsbt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bhyqgqhv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jkolcrlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xaftrqhc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rkvpdmyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqqzsfft.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rcgonghf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tmforgzi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qyyfzukr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ylthzdei.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ohbsswqr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bkiynbev.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3shudgsvs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3hyehyfmu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3hcvencpx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xssoxygh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmctgmc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3zkfuojoc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kolggjkt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pncwdoyh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xspcldsh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hndvitmf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3vzdslnlf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3qphesnhe.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3nceisirg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3yzfexaln.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3zncoqdld.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3glhhvlko.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mzyieklp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlbwwfjy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xznpoxro.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dbrhbemw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gojdpyrx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3enwerjph.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3nrewbndb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ccwhovfb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykbixgpu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqofinii.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3wueohzny.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3smtjxiec.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bpkhvmdz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvqgytcw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ajpdvrvy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ekpwvnqq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ovjsjafs.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mhzmesyv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mjmglynt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3utdrgidz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ucipdbhq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cowgvpbx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3essszqcq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xuewxmgy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kxlauhux.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3huogccsd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cficzbqi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jluwbabd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kcysacyv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3pfspoukg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3obuwtisi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3zsykbzoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbpmztgw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zvquflaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gswgnvjy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dxtvclcp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3taomsumr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xcovwmup.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xfldhmjk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mpzujytq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dhbnplkw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3cmdkiikw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3klsbvgpd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3befysmkl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hmehgfhc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3uugfqpmd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3fqivnzst.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fbpzqojd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wuwhhrvl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gusuwwgr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3seuajeoe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rrolmiym.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nyotgqeu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3cdkfcbhp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xzlsqkgz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3rorncugf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jgzsfnff.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hnrnhacf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ranbrzkp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3nhdwdyys.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3plogcllw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3djspdkwq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fsaxwybk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3kbsxmzyt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fpclqyzu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qyygeggr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wceetamo.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hopphryx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3udkwhivc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3brlvzbps.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3itnowtyh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3lbjtvshw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jwswoubr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3pbydipwv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3nqdbjkhl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ohweuval.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3csbtgdfl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tewygdcv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3pjuctfca.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3zrlkahip.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ebjilwin.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fzsxavgq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lprdytvr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3zoigryxh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phittrvg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3aqdlglig.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qftcgpkr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ivowoxmy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ewztgkpu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mcwpnprp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dcgphqct.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3oxryaqcu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3avaefsor.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zkzjqfcu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdfehibk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3okkevdqx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wbwtwigj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3sofwnkwf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xlqdsbok.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3jbvjvwyd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zznzljeg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3lrxthyra.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hohoygqb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3fpmznbaa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ribjjegh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3nikzhzrv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3kirznrve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrchderw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3pusjcbmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dibmsfoj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ooywnpsn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3gfabblvw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rwynmwqy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sxewycah.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3hyosspuj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3sghtxmvm.html

);
来源：http://www.52xcode.cn/Article/details/gt3bbuztizb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3mxpimokz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mvpqelje.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wuyxneri.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ckvzrusc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pnvycjsx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ienhkffu.html

);
来源：http://www.52xcode.cn/Article/details/gt3lrrezacp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gerqoifp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3cyyjosiw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mbipdhcx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dhpsbhfg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3kdaadpaa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3aozanfxz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qiptdjzm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3psrjhkdd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wdnpkxrt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3myyspzrc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3raujsaln.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ncjcbisu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3hsznzwgu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jihrcqdd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3wwdemrmn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wwypxgzq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lwxngjbk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rrafglov.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3taiwkgio.html


<!-- 参考信息 -->