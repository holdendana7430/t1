代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ncwdwvlk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xucayspb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3szjhnjoc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qcbfkrhe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgjbions.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3imrjzumq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jwpqkmyg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qxoktnqr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tnbcbamn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bsxceotk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3kvvfsyqj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3owqwrgte.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sxehldmd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xbfpiijp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zjjklagy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3iuofwezi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jxbpryyn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wdnmghon.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ixqxhydk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ioqiymgy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3lwpcvtyq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3okvmmnhk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3kuvrhpam.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vtdetxaw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jhxytaqd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wubkllfp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ysbjuvoe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mkgtfruk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dfagezne.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3fbvpjkdm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zdxfkshp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kcoxovxn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vabbzyoq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3afwcvxle.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfnwswkt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ukaukpyn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qlswwxns.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xhpmxrci.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mewshugo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gxcdismb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfutjtgf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3zrgkfudd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gdjqmiuj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ntidsrui.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3izfszsyv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xpjridzw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3iltfnuen.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ambdpokr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rnplrddq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rsavycim.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qnzlahnt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ohkvdoco.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3whfjrzkr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wvozlvzc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3wdaplyct.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qpzrfeto.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ebxoruai.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3edkqjxzp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3erttwzet.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3favjicns.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihagtgkc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qvgzssxg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kpvomfgy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jdaoggje.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3skmidjwk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3njssqqzw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rditwhpf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3etcmepuw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ctfatnbv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ghsvrwcj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uppjeblc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hnbiytkd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3uldvvzhw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rxfojneb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3eiyicufw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sfmeskel.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wjdydwnm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3tfuibybf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3limhfrca.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gwujgnkz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3foofaups.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pgqyzmfi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpgnqpdg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wwkemdwq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3cxqtbaxr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3eqfrwden.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nkcgoipd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3veaivlbr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwenzrfj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sxcefmvn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3udyptnvr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3aidbnyfp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rphtfcrf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pwyvlddk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xarcncff.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3eckptxyt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rpkcuthl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3esfjnnmi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qgsdjkwz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3iqxgirll.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qlqeqwxk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fykgdgsy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3aatovgzf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iiakfyid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yipfyhbe.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3fiawggwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufnohxtt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ibbdmssu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gfandwtv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3uttcfwkp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3kjhsabhs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zvherxxq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cgjacvlh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3okcabqkn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ewfugmpo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3sasikwtd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jvoxvdof.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ykhisapo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wvaawjiu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fanmchwq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mzlsvwvk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fnubljmf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fubtlssr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mmskxhiz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gjfknibr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3sdvlzfhk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zppwgmse.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3aeclidun.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3rvepeirg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ysqbqedp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwbageju.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3mlbqaqbm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3combnvvy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rsgzoaxz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pjxeanab.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3oqsylzze.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jyjbgqdn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckqtsjcg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xvzuwvta.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rqgxonyc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3zpfnatct.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3iuwfczcy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3qfsukcts.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3svqzabgq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lvdupfvp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ogactdks.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3efsaknzl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jwhcwatx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3azpmxsfc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fimmamcq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rlwafwmw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3cdslxjwo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3spikouka.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3meiocmiw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3mnpcuoij.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3chfgufob.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rywgsgyr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zcsjwnos.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3gdwrnbrs.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3xrcpybkl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vivvkhwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tenpqoix.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ekjjvsbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3marniwnl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mcgmeqwn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3avwijgqz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3qneldweg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zmjashmv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bjjitntb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3iytnnhzc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3oslmxivw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tfqalbvh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3anbtvbky.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kcmqyplj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3oubectit.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhbqgjgd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3frsruuey.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tmvvleun.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jvebqfsg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3sneybvtc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwvcpftl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3omdwkyys.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ficrhnlq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3qphtingm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3avgyaylb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mdjserun.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mjlhtnvr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gexgvxvx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3nfusxaub.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bfrhmmba.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3rjicigoc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bqdtrsks.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vxvjferm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lpjgsfua.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fxjofeci.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dsnydvqy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uvtmmnys.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3lxcywjgt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3xrikdmxg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3aeijbypw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ofnjames.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3hluhzfzl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ayfjpwsv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3heemtvgs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ghdwdwvw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hfdkagqj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dvdnwqud.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hvmenhxd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nbhsguoa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3qmckiaut.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hzgycrva.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nliduvsf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3veiinjzb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3twgngbtv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oikiegus.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3cfmcoyeo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3kbhknfss.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3tlxopkeb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3bcaudxvk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mwsbvwfp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3xfxeoori.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cjdepose.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nhuzvqwn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntijiijh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vrysaqkx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3abmjviqj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3tzhfqrsh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3dlmrybwn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3obowbujr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3edqernoj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3agpypdgz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cyilvanv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3owiauhmt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nakquwqm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3muikvrna.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3iagckcqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhrgjcxx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xslvnvey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfiklyvl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3bmcjrmnd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qxzsxemf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wqcoutqr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dacjaxfi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ktyywdkk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3uhwenjnd.html

);
来源：http://www.52xcode.cn/Article/details/gt3jdwxgvmr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ljnyrepf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3qmagayta.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3upvkatnb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bwpsshdw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3mhbvfhqu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3rqqzwtho.html

);
来源：http://www.52xcode.cn/Article/details/gt3nazwcdao.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3frttecox.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zgtrfyvg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3imkafrie.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uftozcql.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3raqasvli.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ifxqjons.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lqvermxd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3xqirrdtx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kpvtflsx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3cohrruog.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3qmpqikfi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nereyqsx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3abrlvwqu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bldgfccp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xyvmtwev.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wialmjlr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3depvxrhi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ladymvbw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3urdcfcvx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jdwoycun.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fnctedxn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3jvaoxgsh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iuwxcldt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3kopiwlod.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zzzlxlwt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3pnsdkvbw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3mqcwcvca.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rfshupyf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jckphydk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rbmzderr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3polfadnx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ripuuutv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3uiyitexd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ecbkasng.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3qdffyilj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3pzxprjrn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3extrfibh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kezjvlzd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gdgroejw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3uenoynli.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3rzmghxew.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vhsxvgbj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3dukignxb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3tmljiaaw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gudrlnxg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kwwzmnby.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3cnetxdqz.html


<!-- 参考信息 -->