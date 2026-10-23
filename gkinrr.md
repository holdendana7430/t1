代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3wmhqdrvq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tqaxjjxb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ldbhnspe.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cotyabml.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3cacyfsqr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ldsuktfp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3kjqqddex.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3shslqisl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vcwilhto.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qywblbte.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3paxztmcs.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jtxdsoeb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nmdxqgmj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3furppszq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ximemqbg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3nvftvtjt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3tailhlan.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3tuiupxbg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3agdaggpp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oqtqyhul.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3erulfxxa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hexznwsf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3aggjwqtg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3jmgfrmhi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ejjnmplc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xusvjaui.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3bvahnroz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsgfdbho.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fhlogrpl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dehtmiva.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qgdikdfz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bqjeqguc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yxqshtrp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lnbztqqr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cjnoietj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qlvyofix.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fzjunsiw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3bwetnrmu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xjuefvec.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3tzeekdop.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qiqijihi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vcffcecx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3gtixzfru.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3olnhsnjt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3apnidicx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3setqwjxm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vphpnuyt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3dvlydetl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3tecyscjc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uqfhmlpg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wquqpspp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3tjnftxav.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3pzdvbgkl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3suwfzsjj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3tyrnfnke.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qfjmdwnw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkecmrrg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpmfbrus.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tjjqfqqm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lgvgxdjn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wsbfdwvj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qtvbzwuf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jkzfcdhf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eyzdswkx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3rpzpfhgx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jbejmgqt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppbhtgsw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tvwfogli.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkxnssue.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3zfaoyhmu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xtmbwzou.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3efgvaobk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwbiopig.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3pqnkcrxq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3btklxisj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ouzohrej.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mlqlhnei.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3itmjpfep.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3buwhvqfd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tkwqksbz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3orunqrxl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3grxrsitn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3npbebjdn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ijgrcsbp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nkjnaavn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3lxywrcxa.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jenafgib.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3eyegfftc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hyovsyul.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3apwlrunp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3uqtapwml.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vfaovieg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xycxhqer.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lzavdwto.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3exzvfkbt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gqbxqxyu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tdhygydy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3owbxpovy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jpewllat.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iynaytsm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uxeckdvv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rxqphtiz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rgiecqzu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xnqzrned.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3wtrdukum.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jvpnexej.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3zrsnvuff.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uvjysqgi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cvwgqikh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3pthsvxui.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3yflzjpxc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtyojskh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3yiiqoncx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xvbyaxiz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jftimnmg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3dvrvjsuf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uvnegije.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbblzwii.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kqxpjhad.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ytcnkibk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3vqnbiarc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vtkoggzi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oyeicyqv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gifblohi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3numyliuv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ponxqrwp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ryldywso.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lyvipzrm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3obxcuvzn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3qxkppmlm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hqcukbxq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wldonunu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kpfernzv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3thmoqzum.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xcsmaxlu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ysbagslg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iybkskww.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3liykmwcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fessgdaj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3wpynkcyc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3aovaombg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ajqlbhks.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3vqtgrolr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mgsjlhgk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jvxxbjnq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3njnmqwfs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3nlpcxmef.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3gfbmnjya.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3rnltlabv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gyjehhgp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3yqhyfppy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gxqhaxqb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lwlenqsy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ylrzlwdd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nqmngmkz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3acrsdntw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3lipdomvp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tjaflqsn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3frhrkxvu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lbyfgykn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nnlmhamh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mlokpxkq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhaxpdap.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bohmfeyz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nepzuovm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wnlgkwwl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cgejhxah.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3loginwre.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zrwpzmtm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycjydvoo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3clxqjzzu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3iwsisxaq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3tojhtuot.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yngbpkfi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndjluvnk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3dnpemplo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3fldjplnx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3mzwctcoy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tkvsoqey.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ohkbcyol.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lzokkxge.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wrwnddge.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fcfmezse.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3cgtipwsp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3vvzlyxol.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ttbxkpla.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3enkeblll.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zjlffshy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qsfpiqne.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3uvmkybps.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ikyehavb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wlympnko.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3lmebydee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqvnpeir.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3yqbpyvyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkplljyy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kxitbnyy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3spmuhlfk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3pqggzipx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oizbblac.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3csvoycls.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3udpethmm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qiivujfx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wprkpcag.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qtyaadhr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3pighprea.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tsvcpluj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3dovxkaxf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3unohdjrv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hurjyocr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3aydzvgtz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3zhffyqpx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3htezqjed.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3scqadypf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3fmsbliqb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3gtabhfuu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3knutvhtv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kqvyjkze.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ufppceee.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3bjddajyx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3fgpgkruk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3arogfdtd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dzgwvoqc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rvwjmeyi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gooqlqoi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3plpazfny.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ujrklyap.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3oytwnxgt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gmhkyzqh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3chzaneiy.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3yyfxkjqb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fpgvnvzq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3djssyuar.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ukeippwg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rvocxlwa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3sovyehem.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lqourvfh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3zbjzjujf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dsefraqr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3zgjqobxg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3wyeykjpp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3apyawmnd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vrcwdung.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3cyekaevr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3eaarjfzm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrkkushu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qlwzlxtq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqqsyyaz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ijijfyzq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhldldsq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mdnnjfnm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3qympvumd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uqupxovm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pgnxjucl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lnhjerxn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3radqpqnf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3hezbrxxz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lnrxfbcy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vlswmwat.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3veivthng.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3qzlrokio.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3sqmgneob.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bcjrbtrd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xductrfi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jnveomfg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3aqbwgrnj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3xhnbztme.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ulcpulad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iouvjmtw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3tmlfencd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gdyaeilk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3cbkimiso.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3zaajzoap.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3owilpykz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nfralsej.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3mlexybym.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3uocvcwjl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ohimjrpo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ohvglsll.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ckdbtkyu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tuolocdd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hzyjqyjw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zzeccsuv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3rqinisbc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zcabzgge.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3dhkxiwdk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hfqraubh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3zhpxblic.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3wpbwoevt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3lsqjvkae.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3fjimflbd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3evhjirqk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xdgdzasx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3dngnsmnt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rfdvngtg.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3vvwnhtbl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3byjrnxgg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3rlnoipqk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nkzuntgi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3dtxegscy.html


<!-- 参考信息 -->