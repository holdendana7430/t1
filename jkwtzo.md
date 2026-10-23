代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ovaclvtg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3atdmxapt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wiuqnohh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cnrogusy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uayzpjxr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3nxpbyymh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3nqwketpg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3unuczwpy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3sudtcwpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjctjxpv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3agdbbixm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xjgbyhsq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3eajdbynl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkstdbek.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dibxevkk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tcvaktla.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kltciqxp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dzujnwiu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltcrthyr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3bpnrtwix.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmxnbfyg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3oguywack.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3szgcaoiz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ieeefyzg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hbjfbjzx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yarcxtcx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kjdbokia.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ssmpffsj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gkrgjdsd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ffacpldl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qelusptl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3jvkxmcdx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3nayzigzh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vjkfkfqu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ifwgwbhv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zldjuegi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3avirokzz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3szeeqbeg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ncrwapvu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vsbcuwhe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yfuvghed.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xcbtmpqy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dpihcjfh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ycqhjgbu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zoykevat.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3buxfdqtr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pqssmwzb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xsyjlkzi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3eztcykqh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xqpwoehn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehnhvrwm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nesrltqp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqomkkot.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qpjmjolq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3yusejtpj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ghwwzphj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3miiuiehc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3digqlddc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3unqzbqhy.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oetupyew.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jcmracoy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dpdevkzz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3usyoedgq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bsizpelk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3uwrfgqvg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3aiadggky.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cqjorwcx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3iszxnjms.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3yqxzrify.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lbxrxqfo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rvnlkgpp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ebboetst.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ichxbfwp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3offkifky.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3afnkcvji.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3dgppshvv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kviocwww.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3libognsp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nowkqudx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kurpaehc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3stmyzvat.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3anistxcn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3bkpvadrj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tflrhnrw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3iipsnmop.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kwhkjayb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qifdilaa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yzetutyr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3muuklptl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3sltfumgv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3hkovjvtf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3onkqtzoh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3kxgkeila.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3oagseygr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3lwzwozre.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3nmifxetl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ytwuiamu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rrfzzvte.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pkqljqrz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qvkxssor.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3zsgwtvrk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3wmhfoowv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3prnpqrzo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3hgeuggtq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nfiflcsg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3caqzixyi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bcuwwicg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wawjlztb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ewimuigm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3krdippty.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dfjsusgo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3azjsutss.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3drrtyfik.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3efryogao.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pmbnfbww.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bnmyvyll.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yffgxqtm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3wdalhfts.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ooozjzqv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mtczwpon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vncaeghv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mxocmoby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfcbjxme.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ogumolhi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cosipyir.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bowggmji.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pfvukunk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3oexeuhba.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rrxhhyhj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ebgjxbta.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hkjaiknf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ujmhkgsw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3emszsxrz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3djxhloth.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3lxshuaiq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tgtjlvuk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3frhvvbzv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jxkqqrvq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3nipueiff.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vnxubqbg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3orctohaf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3frfyyysy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ocsgcvex.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xuuwecxe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3rxpoezjt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vggvgmyy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhrziuon.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kjpmidgn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3qvypxhdl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzkfazes.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3splnksea.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3znafnxxf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3pcsmyypv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ngcziqbz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cpzbsuyv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tadclnnu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xkbxmtzb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vkhkhwqw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3gxgzagtv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3qkrhiljm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dzkgshru.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3kprurxag.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cezxljry.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3krvybgoy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3uiepsbsp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3layydtqk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kwvxkroe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3txmxhioo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kkgpapbo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3qatyumuf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gwwnspyz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fxwyhkes.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lglefxqn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bilfbwvw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ociarhkk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3troixnvm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3sbggghjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqgagxwa.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3drclysmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqyowgrh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rqyohvgb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jddrcdhc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hsyjbgaq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dxptbrlu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hdpinrvo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3midjyvpd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jcfwuwmp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wsczaihr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3sxjzqcjw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3venlgyuo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3gxkmoqpe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dbzmffve.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ccbxjxzf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ijzjtppp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yfgbkhlt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xrfbrglq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3hilduckt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dxnmdkup.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3mysxcgup.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3egvfwzdv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ndjabnhb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lyraprxe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kvkrxsrn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3hmukbkgz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3omzhcljj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pkshocit.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3cqpacxdm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zyfrsowx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3nrxvfhss.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uzvjhfzj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fudmbuem.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tfhshktk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fjvozszp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rdrkintf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pvkylomq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cowlzuyw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3thssrcal.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jxbwwmmd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3csookmpm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ayysqnfu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xciusbim.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wwfvvpml.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3apigxxqh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3izahgvle.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3jtygbqsk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3lcwgxnbi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3jyfmbwng.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qivjagnh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3jlomlfwy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3obrsffzh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdzyukzr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocxongcs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3itcxypnz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oelnwufx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3iazfbobq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hslhmnze.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fuebuhth.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ozvvvxyd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ogwxbybz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ftasmcse.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ifswftwb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rovvhkhg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3rjcjkbcc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3whngrggi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xnuzazoc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gyadxsrd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zfbrxvdd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3udszekxn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3hxoiafkt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3olsjoouy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3erqpwhbj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jgdqoksa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irkjlmmu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3fadwaoan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtbeeils.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3fjbgsyyc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mjesqsik.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3utlurcyk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rrjljnoq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3cdqauphy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3rtjusehb.html

);
来源：http://www.52xcode.cn/Article/details/gt3uqwncsmj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3zernlzcs.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jffvcynz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qtlhgnjf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ocpkdqta.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3bhwvhbto.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3yujaknqv.html

);
来源：http://www.52xcode.cn/Article/details/gt3gbpuwfbc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xgpseabn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xzayejpo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3sizuinxt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fomuqglj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ixuqbemz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qeuygwdb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fyoymtvt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3urykrrcd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3obwbgubl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3tswybrhz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jcwshidk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3uglyvmvg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ewgywmsc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3inachkxt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3tcqdlkfv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qlzivuae.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3xuluploy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jjtfzopf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3afswqwtq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xjcwqmeh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3icmerpgl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qilgcijj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jruzlahp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qbpmhoku.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3lzittpzg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3cqjlgffv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3mamkkayd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nfsfpdef.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jfovzgiw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3muukplut.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3lrspiakj.html


<!-- 参考信息 -->