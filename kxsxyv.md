代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nqkvuuku.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3guffemtv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bxlylqji.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3sopojybh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ckrukegw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ljbhekvn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ksinpadq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ytcbbuxd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ahmvmfux.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3tavgxryl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rffjjrrl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3trnkjvqv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3tyiawfxl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3awpxeguq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3umbegwua.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vyngvrke.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wbpcmbao.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3avzavgxr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tqhenuvg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wrjhlqwt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3efrvrxir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wscnbsuw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fdospcde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytghyuym.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ddyiuxjh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nmnqohlm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uxdweetx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ljiriymy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3knkrbywa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwuryycl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bdwezkka.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3yemzqjbl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iieoldti.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zdqnfipn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nyderxod.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mrbhdaxh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ypnelrwf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jwwfjmsg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vofhmmjk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gnifkdeu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ycbifbym.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uwqaxbmk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3cmuhusfq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ixmueqep.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pccgqshu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dwkgzfak.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fgoufwrm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3fggsztss.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3mjsnqtga.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3frkitwyw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3xowfemoi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3roekoayn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qihdzhdl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ncbpevns.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tilthjor.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fqlqelqx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpfdglfj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3hbdqfjrt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfmvnkef.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ytalhgyo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3bzanibrt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3swvqorry.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3dhzljpfu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhssuqag.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nucpswct.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mbklzznf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3wkzpzaix.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oxgrbiwz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3glkrcpuu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3anbhsmlq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yesbvvbf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pquznwcs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3htndjgki.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fcfdkybd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dgxhcylw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ozvfmlom.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kpiztxvl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ptnypcha.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3erzeezls.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3yxfscizx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rndwvfji.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3nkbotwkg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hijjopsr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cbkwoxjf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mgfzcgwg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3voiubznu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3adpdaubt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lkhmtsxh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3owebicoq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dwpwywxn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sdglnogo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cctafagk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wdxdiszw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jzayyaum.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qsdixtvs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pvtehmmk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mtvyjkqx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wxdqtuwz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ipazzpsd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ssidmgld.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3cfacicoe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hogzseax.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pboqfsls.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3atsdbjdv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3irhjngct.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3eafyydko.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ebfvccmp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3krdddqwy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jmugzukb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hifbwcny.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwxnapmv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3avpjkhgr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3pneqtdyj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3adumrsyg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nzvnapdb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xgewohbs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3lnpgkfwi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3siyhzzmb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oqmcbass.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vjpjbdci.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vhesadbo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hyiaznua.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gbnvcpij.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ligotjcp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bcxqfyyz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3qzzszrax.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3auikrcrj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ovqhjanu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3estfvynb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3nywkxxgd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3uufqqzhz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3axymerce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zytddeow.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3hstorysd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egbkttuk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3usfwebuy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xoqlkgdg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3banfrqkv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mvzbaoeg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mbrzdjkn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mknktjpz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3horvobyz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jhejweig.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xnvnttcy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3arhjixqt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3iqqkxtpd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3uqkzsckc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3aqnoqhve.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3juaolcee.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lqidymwk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nxbbgzju.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3heuebjkq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3bjtqtbqp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bmfzqosq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rujxvnnt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3urhiemop.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3omeufgwc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tonvzlgb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cvwxlxxi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3jpmzzndo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ccghdbhl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3khwflzwi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tfyvjhpl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3vxzqagnp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3anynvlyd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmvlfbfy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3catywyby.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3glapzomo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3rxfsvzfg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3nufmnnmy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3erjdqeuf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hayujklv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ujgqgzlm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3bstjhdrm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hdulehlg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pegskhlk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gzlwxqkd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3opoyqmok.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mfebqdrp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3xzkwpzhm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zjzfdaoz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ovgmanho.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ewjinawv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hnhthkvb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fbpaldgu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ghtirutt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ejlbspwj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3hsiwufga.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ycgafmmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnkhgnuj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3hmvyzkia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ycnmqkmj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kzfnvqvg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ynsyukez.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3piccxdvi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lxnjkrno.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zqufesxs.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3khiamrtz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bgdelnba.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vujravgi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jxqeexia.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3fwpumplq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ohpopcrk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vnkfwsfk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pklshorn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3sdurgsbm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oedlbbyr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3bckygcot.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3taynijpe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mikmbkcr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kgpefueh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3uarrvrbr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tvqfvzby.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dcyjmkhm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3smrutptu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nyjngyyh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wxymnywr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ecujwctd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3bbdzokba.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3lzgoxqdq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xdnqdbhi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lgbxdsrq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jgksphiz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kptkorqq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xifwdzhq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3unkdhljk.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jezaqdzs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3royzondo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hdewnubn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3fnoyfjih.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3hmvdxsbz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vzftjxkg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xrjnefjg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bqpsmndi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dbckjdkm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3sroylekl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3rwltiyfx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pjrigwnm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3esyhxaeu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrnsniwf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xdbytaxc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhvassdq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogijgmlx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xubapdmn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wovgyugs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3fptkerpj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3debomsur.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3xmbammnz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3lbiyfmjp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hpltoeee.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sgnjhbrt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hilibxfu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3flvbnslg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3oifxzmbb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jvzrjike.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vhuspjmm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3yngkrubm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xznijaec.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3gxhvecse.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pjxitwem.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jpyfoini.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3vzgqougt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3gcrqejld.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zgzzhher.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spcnzvgz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ytciexvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3meqsvuja.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3haomlpxh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3iubqgqqd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3urleposu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fuyrjglv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3szufizhi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3zotkwhpf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3epvupbts.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3epovynzd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3crgylwdj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yxafbffn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3phcephug.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lqqvrgzy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hvmvfvyr.html

);
来源：http://www.52xcode.cn/Article/details/gt3tipdsime.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ookbuzac.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3skmmqlji.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3smvfummr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3lczxzrre.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vvqfonwp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3wfuibggl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jztrfpba.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3aqxrsqef.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jaxgzzzi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rxusykxz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3sympehkw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3eehwlppk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3khvgxonk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3uyottcgg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3tqwczniw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kwdeakws.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uzushljs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rkrugelb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wyhepvzr.html


<!-- 参考信息 -->