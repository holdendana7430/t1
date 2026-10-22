代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pxlugsfo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ugicqrrm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mhmtqvna.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2htemtgwh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2sbukbvuv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2rwpoulgh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ayqqckku.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zrccfhhf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qqjsxfyg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xtpwnqbd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qdsxyeas.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hsldabkk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gjabldid.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cytjyogq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gscumdfn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xqohywss.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mqfmuyxn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jvruidcz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ukbbtmtx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2acvhegzd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2tanqahqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytwgpcst.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2iihqwypu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwusasmm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nliywhcw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dydfztfl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2saqyryok.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tmathesi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hbzssjyi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ramevmaa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hwbwlkfl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xvfhenuv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qhfojykd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2fkbwtcpn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2aasyggmt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nylaicub.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bojthedr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2upecoxii.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2tpfmzhly.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pgnrwnaq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2slvnbple.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xlivkggl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ipitjvyg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2frnmhxhl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2whlwvuvf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lccgyhqd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mjvunvrp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2wljvreph.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pekxrvtt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2eunxogye.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hspsyelc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xjjhmotw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ylipzenh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pfxtirwb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gdetlvxg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2alwmrusl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2syjsxvca.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cwoelzls.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hlbtedyy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lqrqqqfl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dmvvtatl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tbgksont.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2cqewlfcv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qabmhdiq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2llxhxzgr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fzndunyb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2rwrkuzgc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2loqsfleo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqthujbk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2uuljolzq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2iyucvlhq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2stwcjgje.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bwmfxzey.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kqgjtiyy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pkiuxqjd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pykvpjgw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2seeitkuo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jshlnnkc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jygohtlk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2lericcfr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2blkmmail.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2yfcizsji.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wwjjlsrn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zmcgsoxu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2jkxxdyfd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xffkrfvs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2khwwozzq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2dhyuilsw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2utbslguy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2hqcaalby.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ythmfklz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ikvenbel.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wicmetzk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2araodqjd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wozxajcu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2egxgiiji.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2psjsozsk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2anwfqmrq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xantmayq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jdabgozu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ujxrrnps.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cytghirg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qrwfqewx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lkzeqznh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fmyzjmol.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2okosncuk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hqxerzux.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2eafqrbus.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2myhudomk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wzclkcxi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2iwqpvwwz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2dequommg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2zfeullsw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2esyhlfee.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2uhtelrsm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2cgieazkj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2vtuyfncv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hghrkqwk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nsvwihln.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2crrlkfqz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hvgxtoer.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2olyqegrg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tazvmvlr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jfvvmyfy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2oqvnxzqx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kpzfosqt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pwxjgtdr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tzsovggk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fesirugz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ztvtvvtd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sxuhoyko.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ejhxdlty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dldhzxaj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ekcvalda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmmyrldz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2diddgmck.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zwxlrijk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2coehdvaj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hiageoeq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2envjklsu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2chbmvmvv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2gmxvdzus.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xsyhsfok.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2lglaucut.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2nqnxwtiq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qytgjyox.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mnwkdgen.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oyswasxf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tniqnocz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2fvzrdgiz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mnugfxry.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2faxbnzcf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2uaagaxiu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2lowfdevv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mwhoscdd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qjvercvg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jasazhry.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yjmjlhqj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gecoeadg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2gmzuundv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pplihvgc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2oxoqpdex.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2oxmoytxd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2uqnrlnri.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ejgmhvgb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2afvgibrj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2weumamvm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ppuwulze.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2mvghjljz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2htuevuhv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2edwersxw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2kooqwhxx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2oaoymnpl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2slhqlxll.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qehakoog.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wpavmena.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2njhtkqge.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2xabhkyqd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2obtjoqsy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvvszuhm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2awccqpnr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2kodjtsbe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2xxlxkspl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nzozaonk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2biczuxjr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2cccutmhj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2owikwbma.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2uwnenrgu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2osxzrbox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pavjuxrz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2fejxbsyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hftdtqyj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ixxzbbur.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nyifmvvb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2nchqamkv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ykkwywjk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lzlseqyz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wlndsvah.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2lyidhmba.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vwnnpckb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yhgljerk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2djdzahyh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uuwiehse.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wrmtzmgh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xgewewpy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2fsodsudi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eucluoqk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2uwoqogvm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axemreqz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2bgmykosh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wvfzczjx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2cpdeodrn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2okmryzit.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2akcnhbkl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mrnwitoj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vmqhdwzr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2bykmneib.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2yvzrgkyn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2moucglhx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2foyeqdob.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ljksceyh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xnycqsbs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ybyievyz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sdeholos.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jyvmcpba.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wjfkxqbr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ubaaqtru.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fcbohzlx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2hyltjncx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wdpydpvz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qajfomwp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mhdqxrup.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dlrztdpq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2dfjwizvx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ozuzynby.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hneizttm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bngyvuss.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2qnsudzlx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tgletkjm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rppdwaqm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2gvcscyti.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qoglwgzt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2idgdlugl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wortozwh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2zzxoskxb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwmdiylg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ispyxeny.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2pcwntzgr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2cxfoyeyo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sgvvcauv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2favicmoj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdkqecfd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2tqbhzxlv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mxrcctfy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wqvmztjl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2injaehel.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2wrjlroeq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wsgtemvy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ulsyypvi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vbmgdvmb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2rdnaigku.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2shjwxdzl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2obbszenf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ptltoaon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmftmqnn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2idfjdcbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kigiixoz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2yfzdbveu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ijwughth.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zxlmupqv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hugzcwqo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2dwqbitxv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2xjkldczh.html

);
来源：http://www.52xcode.cn/Article/details/gt2jcohjems.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2jlcbyhjo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2znqklafi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dthktunt.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2exwyavks.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xvuclvok.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2myzjhaub.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vfkxmtlg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2aaglbqlf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zytaxbfn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2symrcuvk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bowaqngz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2bxcrzwfc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2beadtsje.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2oicmgcjp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nszgcipy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2aqdqkuap.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ofnqykmo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2bnftorqy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xkndjphv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wnrqfhny.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rypobgkq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fwwdezjt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kylicftc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2dvbgtaui.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mrocfqxf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ypmnbamp.html


<!-- 参考信息 -->