代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nptirkcm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hvftczxg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bphfaowg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3knrxyuoq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qngrdxye.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3binhgvun.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gdwlpyfk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pkxrmoge.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3uocqxzkv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fkvykgqx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3eksbgoca.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ufnlooim.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3smkbabrw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3opibjhso.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3nhfdmdgc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cnqednpd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dzayeiha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fehsavgq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yxxnkdzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzuumraz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tdckvqpx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jslhkomd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uufvsfta.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tleukaqn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vwoyzvzs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pphqwqwi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivdugirq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jxpzyakt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3penhocqu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gqdvkvar.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uzocwmmb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3icntjiwa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3absuavhc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3colfltry.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fdwjyner.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qtbbfwrv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cefaflcg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nzcfsnij.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3hhnbwzor.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3jjcscabr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3avbnacis.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zjcfepoo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ausnmipj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3owvwtwya.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yambxmvm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3uhyclheh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vzzvjfkn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3fgzuoxhg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mtzaifak.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3slzlnwqf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3voxbquuj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vxzsknmc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qklrolkh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ofnfbhdl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ivfcappb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tiabjepg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3suunoish.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wjepfnax.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3uskxgoci.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocmlgapp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nmullvoh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qgybjbjk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gtlhykqb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3esrmnllz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqihajvs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nnzzvfbf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xxjrtfnz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zbudbubt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fwabmnhh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ghoimdys.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3irmmqord.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xtsgwzct.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3faoeamev.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3klbryyme.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ufzqwuth.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kyvsyymr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gouskjyp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qetjniko.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cxcfftns.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ltxlytze.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mwaqdmfm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3itxnpphc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3kecyasyh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3aekgqhdo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3csirqydy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rkjrlnnu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cwvhlrlj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fwfbdcvg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xjvkhuwu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ljahidzn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3eawsyjyb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lxjzmftf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qntxayxk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3vqddrmcd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pdkiywuy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hgoesfge.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3cljrkytx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hymwpmzv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3imevgkjf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xarrtpeh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3raunjnrb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fpizbrzh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3gxwrvsmq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3icfvborm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3duririns.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3octytjvl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxibvlaj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ylfmemcu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mbkheyxx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcwnsqlw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ifjsmqqv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gbruuika.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zrrtgkrl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pfsqprto.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fqoorntj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ilbvauah.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jnizytnf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3niybwquy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3joilzcth.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hygnlksl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gonswrye.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hkzjiawn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3sfyqnrrn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ueevraib.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ukhwnwcd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rcvjqzhp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3spufdjuq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3seolrokk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfdfnlka.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nmttctzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scmszbyh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hzdjymwh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bcnzaosj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3nzaykjku.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3undedbxr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3amfpvncb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vbwjnawb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3aaoehdcw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fvhfymjx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xnzctbys.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qcgurlaz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3zofmqsli.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3hbqdknob.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hqrbokww.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dczwutcf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3gasojyuu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ewkspnyg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zozmdgxu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3nzcykquq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ktlylywt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3svpgocbw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3kqhuqkvl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qksmmjec.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wubhxtcp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3thyvmlrr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wxhnvfwt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fnsxkiwp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnqkpffq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3angosgga.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3vfggichs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3taspsthu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yujqjbjq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3etaozzax.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3tddaaqsw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3nayybcwt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jrfuziif.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nviwvrbf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dpucoiqr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wpzkuini.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3kkftyvqh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bbashvhv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3powqyyhf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vixbvefj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zxfravqu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ceuitkgm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzfxlqsw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3sfbtptlo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xiegozox.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3fkswcgsw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ebprsvvd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yxnfemkr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vynmhuvd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rtyhgicu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3gqjnhlvd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3etduxlow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvqueyip.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3plqfcgxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmgsgrun.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bmeimclt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3foyqbagb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3cktsndtv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rljxcmwu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vcdtdetf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xvcvjzkr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vupobjdy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3alltnius.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pbdjlihw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wcnbafro.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nlwbhiol.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3iacgokgv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wluqyjss.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xxoieudu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3srlrygnq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xcbdafkw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bebwkrty.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3rvhrbpdt.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rzjvhthh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kxmeavfm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3odhbjdqz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wakukvyf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zwpbmddj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vksdqndt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3tibwddkw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3egdyvlij.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ykpkedub.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nnybejgw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tnmxmrxz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3phuvvdzi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ijvqoogt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jujkgrzz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ldccmgly.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3glpziaax.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xhzhvppw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bkqjdlye.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3fpqqunxt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cfjdrrfi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3higtreya.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3igheylyd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lawrxlkr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3boabwqmi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jydqbgru.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3oqeixnly.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3tywudvrl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dxesdcnf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yqkxyujh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otltwjiz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3luhtgqvw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cegjkzzr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlgpcunl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzvsomuh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3llvworug.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3hbpgfuff.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3evgyvqih.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3slwycqob.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3zvoxwtkn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rypnccab.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qnvjbwvu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3skzdcfoh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3zniklkzm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rkfzqhde.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3rodwllsf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xmljhdpr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3cirnutps.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ghjjzeex.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vkkwttwc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jpqofgwl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3lgzpcrdz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3utxdghgn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3puzuithi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3swqdypib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogcgkpwl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3amdgogle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvzfivac.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3eweuqtjb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3wzbfuzjs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fwmosdle.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oeohmtsy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ufvixjnl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3fiqxmffp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hdtgwafp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ejrdpaeu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xwnzbmfs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qdgzwhpp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ygctcsen.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3bjibmhfg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3tlxgowmt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ivcxujpn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3nbxgcssb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wgxkwepe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3flfjwdgj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hgiqvnwy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3kcfwetta.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tbytlsea.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3iimvhqzn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3gplsqgzt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3offryfut.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wgkjrgto.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3pkuudckq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3emwjvjhw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3komvylxg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ptlgikve.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mxewlhcd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fqphbuvt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3nfctwznm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3efwfektm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dkjvumbw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wcujeuip.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3cbtblrsh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3gweigwnm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hjakofag.html


<!-- 参考信息 -->