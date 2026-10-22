代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2aobjjtgp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jwpoyjdq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2opocbwem.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bmtkvpka.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vdrpfmjj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mwuwxlro.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2soyyfdgz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ppwwxbpw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2juzxypfb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2htrubbmy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qhyxluel.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2inuckqiy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dujrylpb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rzsblxbr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tbyowynx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hycgaaro.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jxjauidd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuyiijlu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cruegcad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aowlvlbb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xahrvkcb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2walqcpgg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2glevogfw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2orpamnwi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xmmhiqth.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2guyhxknq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vzrxgnrd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2bchqocpg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2usmpopjg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tasmjijv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tdqwsvwi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jjuemfvu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vgncfqdy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pmvjgrny.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rfzysqkl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2akebkcke.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ysbyxxpr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2reqvvjbe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2sswyxvux.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2avacwmqy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2auflmerz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bkjrjymv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dbiuooec.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cburrdvv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2omxcfbjn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2pikdvqdm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rsjlxxzi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ggxxcyls.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qklkcodq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2osmakaaz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2koelwjno.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2luityatk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2reivnqlj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2uasykczf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rjzobtfj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zhidfvgs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2tqtqhaif.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ilkjmnlw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fszdixyf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qvqbumot.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fuzzkjar.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2amxpypso.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2afnsozog.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gjjaqeil.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2lkvkfsxo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yxbshtvi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wslyjiib.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ccfngevf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2otuqhuef.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2utgaunzl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rkffutoa.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2afijabzq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tycdsbci.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sgzsqkxy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kqztxzro.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ksqrkgez.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2tuhjjapp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vlpssmzv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2feuyfxqo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lguvyymz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2uclhzyvi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2iwpfbnjb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2avhvxunl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vbnuiyhp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yxjcrqtg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2usqawlra.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2roxeiaea.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aactwqsi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2afkjzmbg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wzgaolun.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xjfgcops.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ceozanni.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2syjmqcoa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hdaunxof.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2umxgygsb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bimapxrs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ppjzttkr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2okpipmvh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ezydbckp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pdcynrcb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2tbcedpty.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2fvolgqig.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2tdplgbun.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2bifrilts.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2rhbkrzvk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2uorksuxb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ogumfjet.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qphxcxzc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2opredztc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmoelklo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mhvqvopj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2taltfmoi.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2txhwcaqv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qofslpim.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gernhzyi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gwkxbihr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qdvfdahi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2dotgsnrv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lrhkzdna.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gjsnuzvx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dwrsozzl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2tsgbslzh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2htqqswmm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2haspscvx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ewdnppiq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kfrcqsco.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zrzuuqau.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qemulizy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iunkrfes.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2eechmtou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asdxhfah.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qpcwqtas.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jxxfrigs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jdbnmqwc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pcnkuknx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vgfvjqzl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2srxbfewf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2majhwtia.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vlrlpeco.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2uqtyjjam.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ewcmfwxx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2axbaumel.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ntybephu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zairhogk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ijstvcok.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2drlpanyi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2bmmqzcwa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2pizvznqu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2uybrzrkm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2utcfmbdx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2fjtpwasv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2iyghqcch.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jmisccgy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2oafucvkx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxqqhihg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2gqkydalb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mrtyscmy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ljvmdldr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zuuqnlmo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2sfaeydgx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2nzygqwiq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tispksfa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iftnpslu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2rkabahlh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2gsohvijw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dvxqxhql.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2aqiiemou.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2cypzxnyi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ynigaden.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vqqqfanl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2njjixtzp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lyytlxse.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2dknlcrvx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jizsfuon.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2eukxlbzm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2nmippzik.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qkxwmpuy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jtxpfogc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wvjdzqxh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rcohztiw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ijabsxsk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fczcmkdc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2awoevpqm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2hcuibann.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uxujjhuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrotgzvx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ygqelyvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyxmrecv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rpixudix.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2exoadtza.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jtqxeald.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2admkofkk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bflxrhfl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ixiketku.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2hnbushym.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2jvmytilm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2kheifnoo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2mqwfzycz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2fntdkufc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2icmcaakc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2mcnrohul.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2hrzvjpoh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qjqnemgk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qjpkgyxq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdyrknkw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2pukkbvzu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2jdawvvex.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jamyccej.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2wozkpjro.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bbimansv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gjduyyny.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vngimbau.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2daoyqtsr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ffmdpxmd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vlfcjxjh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2gkwjxdoy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2azffrosb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xylycwby.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ppdjhlzm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2geujmbxd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wslsfnzq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2klopmkkh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ytwyupyt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fotxljmi.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kdfgzpva.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2dbtvwyqg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fdopwpqs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vymulypg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nfwxkdtx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vnmgwgbu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qlcpqbyc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jwhmdmab.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2iquelalx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2oerslnsp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gorbodvu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uknjqebj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2hzxiuyyd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2uudykeom.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gqkksbye.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2fxrvewkx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2theraefl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndzvrcmq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2lixbqqkl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wbigwsea.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xbndksft.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sxvbfapj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cycpwlxp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zvgpbbbl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2fjurdmbh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ivjzizsz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2tnnrdhno.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qfmbzdxx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2kbvoixyr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2kdhrwkuk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vjvdbrxi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jizqqvyj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2zpfderau.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2jspxemgn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2cmrmqfkl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2fxmjtzam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpvbgzje.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jipqvaou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djuymuca.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ewxbdkpd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pyabdvdb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fudvlxcn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rjvmxhig.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2xfehncfy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rfoctxuk.html

);
来源：http://www.52xcode.cn/Article/details/gt2tmmiblle.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qbmejtxg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2grpiyvmd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gyzduvhx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mawfelhz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ksrycwic.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hmvrbrdd.html

);
来源：http://www.52xcode.cn/Article/details/gt2cispgfsr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hohuvijs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2axeozuhr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2jsfyfjry.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2fewnpykg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2bolgiwkf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rdcriqes.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2szirpdhr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2cwtnncby.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jzrsfyel.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2exknsvah.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2tqcqztiy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fohosahy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2fmqnwpib.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nnraxpmm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pykckzjx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2edconwxj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wklodeyd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qobtrqxt.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jbnlqgey.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xzwykosu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mtgelbqk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2lotgcoxp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pnymsskw.html


<!-- 参考信息 -->