代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ssyxieju.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3odfnebnb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pdxhuvqu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3fvgrpuqz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3iueagjpx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qtooqhmz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3irdgopzg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zebvggho.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vsuanemi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jkitgxcj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bfjpqkkt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tvouuhnb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3topvrmsb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3tlelyusx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ljbusmlh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vfowhfmw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mxuidhyd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3pkfywxan.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3hwzzqgaa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3babknygb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hmbrflbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtknfkrz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ufnyuquj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krwwwvqd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dssnytxg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ylrvzijs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wwgbkooi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bvafbyog.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wxaefgau.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3auuedrdf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3govulsho.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3cqzagetg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qaghbtqg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ekonfqft.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3avgstdjm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sidjuxwp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nqjjhqot.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hypetubo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3jbnezkhe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wibrygte.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wodssbkv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ddjvibvb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qhwdudbm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3nazaelfx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3vgyvpzje.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kjkbgigz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lasktlcv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dqojzcri.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3gwjfgmxr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3lkqvcbps.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3stfmubol.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bhoazyen.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qtxqhhfl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3scusufzx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ftzagrpf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oxlkccel.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhhytrws.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3dczwobun.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxqanilk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cbehnhgw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3miarttah.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3oxnpyaiy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ehpyjikl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3shnitjht.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nskshrac.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3muajzjwv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3rvawjhqg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3sueqfxnb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zksagukp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xoftpbto.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jrkrkrbf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3flvzywvf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wkdlmhmj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kmccttht.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3dilcvghz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xdpmtpqp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3abearjyz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gotszoyq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3uyapffil.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3grjnbyzw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xzgrqzup.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3rcqvzvxy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3nivisdpn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3vsfyfhdb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3qehwinow.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3nzoqhiti.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xlgbvdgo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ikrftfyx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gyscttfl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xzntoomf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lyodtbop.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xqzdpjnq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sglttcvo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lcowlscg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3kjzfbdhi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mnokxunv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3evcecpik.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3osbvybcb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qkxxwdjl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jdrahlai.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bphsrrpr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bcfxgbww.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3rxrkabfi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3azlqrzpo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3sossfxka.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3nzvooyuc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3eaazxkfp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3riskifxh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3xgorhiqh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mefwnkyt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ygzxpnkf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rpvkzurh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vudtdprd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ciamlxmn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dhrcwejx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qluppfoq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rtwtxtwa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pineuego.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mmpzudgp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wbceixgf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fnoinmiu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ihwwqkfe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vfcjbdvq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wnzaqgoq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fqcabhvy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3oqpaccje.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lrnlljtq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gsffxfxy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3plcxuewm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wnmbwowt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3asvxtbpt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hxwfqklp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbpovfjz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dzwgntjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynralapf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bkuygsep.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bkggcnrn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fvohetrz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gengorzg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3htxdsjqn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gkixfbvh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3tbvrrpon.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xmxghhbb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3emnpmmxw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hlxmgzhq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xwzysqyc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vjkgrcks.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fibemdsp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ffifisom.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nkdnpssw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3nxfetfwh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3weezjkju.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ubospwnn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3dhhvkurp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lhiegksu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3blvprpje.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3xwhxyflf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fdcxhrgi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bghynkwf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3mwhjrdzt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rgrzkwve.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3defwosey.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hydppyci.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3mngwalsj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3cxwegzam.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hvrrwytg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wumyjqny.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3jxgltjqc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jriwjvaw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3tqxspyga.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpuysrlj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gjfurlxe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kjzgnkga.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hknidtak.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dfxzrzgi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3stygvicx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ubtzgkzm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lnydxibv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3emaxflmc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3chdumxsq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nmvvtara.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3hxptxhct.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3mzdryntz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3euuwexcd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lnshjwpu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nksizjuc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rumfxvxf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dzzrurqm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qsootuap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cquscldk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ygfiseno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czmtrljf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3eapourzt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3cimxyyuf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3cukciixj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3siauolwc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3umfxdxkc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ttajshgb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3kufbodst.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3llsscyxm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jrvfehpw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3aqipfbgl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3kqqihyvq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wqstyfzy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vzivoflt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xbqeamjn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3whekdvyg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dcytxczl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3innzevsl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3wqppnwzl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qlbzijuj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3wyntglde.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3curjojtl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tlxwohts.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3afhnbvzo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3nsflgmtf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hjxvsrau.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kmacfiuo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kcvlqfer.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fnhnhfwk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3itndajhr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wbrxvymp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ftewkbsg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bimelkbm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cypgkocd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3sylvljpe.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3aphkcfbm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mwkkehpt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fgdcqdlh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3imlnjgyw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wnmuwlhw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3woltzwoq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tujsyzld.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3rqsqfoeb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3intwemzx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bahwehlq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3uvgkptzr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dcovizpr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3supknned.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkpidkxd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3eldeopbl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgwclqrr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ruibhrwp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3dgugcyxp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wemsknsz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wmansscd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3oyovhygi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wnhfgztd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3mzbqndwf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hddgcwsi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lfqymlwk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3objfrfzk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jffbacvn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3pgchjaxw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3mzwdapyi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3nopewjwv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ymtxyofj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gtoxwcss.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wfccmbkh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sjdfgzkv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ojwhunao.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3otsrupgs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3gmbehccz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hdhxmfol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iphzegvj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wqqjtapn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzjipjvy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3bjlrnafe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3zkjfutpg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3agjbucio.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xvbzdtcz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3tkutrrkw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qsvyaonu.html

);
来源：http://www.52xcode.cn/Article/details/gt3daavxrpu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ydppxgoa.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xwbsmpfe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uenlpzzr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lqsjfktx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3qdgabcno.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3tpmjeusi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3janqbdgm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3smryamqy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ogmnvabj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3loeospwo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3nnegthuh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3abrzjoqh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3fgwhnqvl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vwedblgl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bhwmwzba.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hrtdtwbu.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3tdxdhoad.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ewvujbzq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xvutmcjd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3dpxmetyo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yfgkubfj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hdzbpcfp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3trklhmij.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qfzatlxs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3iwjogzjr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3yomspfza.html


<!-- 参考信息 -->