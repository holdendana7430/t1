代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3peslorln.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3uxyhrpem.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yipalzip.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3geikjuhg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ibktqybr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ezeswgmy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3smegzbbg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bkbtcvgf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3puhcppet.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ykalyynl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zfwvvpcc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3gldipnbn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rwetaaql.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3llbnrkkx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3pgtozhgm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rtappymn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ywlbupsz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jyvjzatj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kftqkmzw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mhpnaovq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3iwxybtsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdlbqbtc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mxilpcll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzohsaol.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ixbjalpk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfsyfucv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ikkittmq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qcstcqvo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cksctehy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3begoklab.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqbwclib.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jbqaupbc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zhickpkr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3eazykimu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wemvjyjd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3foxkgjwe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gvksfsaz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zimtfquz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3jtrympnw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jfxlxqiz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ctbsexdd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gmirqopw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3tsqjglcb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3udhebryw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3fmynxqfm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fszqtlqx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jjyhjcbz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vpatxlho.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3mwaztbqr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3muydmrjl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3kkhxbuij.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rjqrqgeb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rydgyskz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqehaacz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uywzctty.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vueeszeh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tceuywop.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3byzpldea.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmntooth.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ijlaxjfm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3mqgwrwzg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fkzdfiaj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpmzvtxi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuvjbfve.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdgbtndw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pkhnigef.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3yiimhlcj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3jiudzfjd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojkrgbwg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vhegjbxo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nibrmiye.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fumjijcf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jsxcwdut.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ezprsafd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3hnvsqzdp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3enxibjql.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sistszhe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rmwutgsm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3yenffdcz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ywcaweho.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3brgtcsre.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bkpgwqvv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zmwfvlgl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3nbfwekgx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3arjyimhw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3cbqvvjmi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3oheuizll.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3avxrnmoi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gnvkrzmy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bnleqzid.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fdhulneu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pzhwdkhz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rlvyjcwa.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eixoswkf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xsepbelo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ccohqovi.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kzufmbst.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ytceihvd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jatvlbin.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bybqqczo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xczgigat.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ewckckqb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vxwyyxpy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bxgrmjds.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3pqnnkqcy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qamkurhs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3yjmsrlwc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dqdgjqks.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vjhoqwoq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mshtxmjb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ykopfayo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wpjfqfkg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gemocidc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rjktkjqd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wkzfkkfj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3flilnshn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ttmowoib.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dwebhgks.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jpufktop.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wfrjglee.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3patlidnn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xjkieuot.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nfxcxpig.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3gxjfvmkh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3puuiejur.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3sdifwpzf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ymohmumo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3avnfqhzx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sjsdwmuk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3shyyqtwx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kcvsqjyc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gvteghzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iomtiyma.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3oxgrbnqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlfwexje.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vvfxappw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vzvdkdfq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3osfziwxz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3qtlgjmhy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3atfhnaqf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3trtnwovz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cyvnpmoq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3clkidpmp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3shbpwldr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xaeyghvl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bwywmxvm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dwahsneo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qdpyjbro.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3chvrtyxu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mtrvpjyk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3qpdijggh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3tqlprgrh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gqegmzsh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3bffdtjmy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ewluggss.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xcusbeyq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3kubqkiaw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yogyugxb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bzqyzkwa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3abgcrshd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ojhmhiem.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltkosqxn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3paovhupe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3dqzxrrcd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ludifqqs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3baxhxpyr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vabmkdde.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3auqoysqe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jrnyyihd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rqjvdcpb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3xtamzjwe.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3kgvlwxoq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lkxqtoth.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ehnumsad.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wpsfhwnk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bmevdjvm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3voytfogx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3eifsaqpa.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zhsqrcte.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3jwlwrwct.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vkvsenvj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3oxalxvek.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3afkoladv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3obvnucjj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pxfgpfdx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3onopdwnj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3lzjuabyi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3hcaswxlv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3dercvqsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnnlrxeb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ckjmfgna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxrbdqgg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jhfrrrad.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fdtdzqyc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cgcyfbkn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kpwopwcc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3foyratku.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nlqeqqvk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tbaouuxv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3aqyuzoae.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3yvimaiho.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3cbvdklwl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3chipjrqs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ooaqjykz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3fewpofvq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3fuwrxeoq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vqqllomz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gpkvroez.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvexvdjx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3brkizmbv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mcezkgxr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3rfivqcbb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gzghpghq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pmivsljr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sojuoszr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3prfpfwzt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3dtxxwbfm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3seaubpgg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wmudmarq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3cwnconph.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rckfwbhd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ifyanzgr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bplpxmol.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3obxhodne.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mpurllis.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3gwvjzpfx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3riutcrqv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wfzzeqia.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dcfqidyi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3coyhxtzw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3asgbjtvl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3cbycgnsp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mdcjimce.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3mfeygnfh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mncfwchn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3hoypiscg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3kinxhpwp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3lrbugbhj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qtpsiuvv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grcabvhr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3oyvacbjb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umnmxxdy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qputmmnz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3zpmgmluq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vrshnnrv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3funodfqa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3yjllhdfj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3oggjxwnv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ksgnidlh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dghawotw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dztuqhzu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipapjfmb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3uvhwyrnv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cgtfzimc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3qvfrnlkt.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tuqryfza.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3nabbtrfd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ndyvnadv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3mzhyczmy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bhlnpvdq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dctcosqf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3qighylyo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jawpmzio.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pdbydudj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikleicsk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3skbhcbam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olrlyoxw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3lcvwrsdh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3amcxwdue.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ijeucbbd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3inkhnpnq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3aghaozhx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3qhtjqtxm.html

);
来源：http://www.52xcode.cn/Article/details/gt3gcvqodmu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3turlgonn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3uqsnlivf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rypxndfq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sbibehyh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3njtaumpj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3dmolquyj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jolqyguj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ygkhbpqt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3wkqxuapx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3jcywchlv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ulngjeql.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qemnfebs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3klmuclnz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jombmdgz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3vmlgpvgn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fcgnghtm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vylqnhfh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3sdocdiej.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tjdjiudh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ybyggexx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jviprxro.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ngoxzvdk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uwezqyan.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tactvknu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pleshria.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3txagekaa.html


<!-- 参考信息 -->