代发 wailian999

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jfknskyk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3svspsrge.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ktvxstcp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3orzxvvyv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jixuxuwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sokoqxar.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3lqibpoby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pyhvrrfi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ekaucxhj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wixkatyh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wladxjij.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vcdwoogc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xywmodan.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jgcjmogv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lkrmbxok.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3aahlngye.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jkoynxqp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3povievxl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xdlctwzy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3wdwxyffc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3znmhprbd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nbebcpjh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3iqruwfmb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oomtwooc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ypgwofmb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3npwsgrkw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jvgnwvok.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cvxfhjgl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ocetzgzt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3eispyliz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wsaueymw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lunwfebk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3iakzktfa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xvdyuviy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ktxczdtv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3yvoampsc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mxepmjtw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpufjatt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yleeeqto.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mzarjudo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrhgegen.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3utxuqwrw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ditlchru.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bkmmtpsy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3kzzmjvlw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ioubaqql.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmniwjto.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3njbideyo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydslfmjl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mfuzwuim.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zraryyug.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3mlzxjeka.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kztdehdx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kuhtktfu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ejipqdza.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3majdvhnc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mhzfblkm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3crguywrt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gcaiaawp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nmxgquvf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bxzjblkm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xhgpugln.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3orupllyl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3atcqbcff.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3fgdsvwov.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3papblxdp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3qjyqirya.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fzxcaipa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hdyjzfiw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3swbiayjs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3obfqlnuy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3fhbkhxye.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3snfmwfwx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3cyyooria.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dulrgvpa.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xgfsdqxd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qcfphysj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cpxmypty.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kcxupqoa.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oieihpkg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dolguiwk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ejuqgimv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lsafgebo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zxhivqrk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3bnupsodb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lfyxgmhl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3yygrmpfb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qgnhynsc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3hepexrci.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3xajmzuik.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3rfvisagb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3kivpxemj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3znartcbq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3eonxwbwj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmxzhjvy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3rkdtdnmw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3agdhdwvf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugytttzm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cwngyobn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3tjyotpmj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3edlyvghm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ynjoyvgl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gcgfhsss.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gucuwqkm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mlopihro.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3txppcmzj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3youqkono.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3hwfssolq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3msuciwyd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3yubpmtnb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yrbqisia.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rmsbpbap.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3aavhymnx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wrktfthf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mmpbnhhr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ayhmemtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzcjbeja.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ckgtciem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzemcfgx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wjnfaayf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3imubkaqb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qglwbaqy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mngiusax.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3axxnbzmm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3cwfvzifd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3azfqwjha.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3elrvxpkf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lpzsfosi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3fyrqkdxc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3nduhujmz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3omgwjwad.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bqjsjkpe.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zwpkyjui.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xbpnctay.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3cfojzsqp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3goadplpr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3cwuzlasn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jcodedoc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dtclcdhf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qdoezagr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3tdjiojxk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ohbvaemg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3upvbyaie.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lrosulmg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nxbrbiqw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qkspllfh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ppmtzgiq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3zdqqjxpp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3aootziba.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrxamrlp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3azfffnem.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3vapzjyis.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jrtxhank.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3cdhmhoed.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cihxbhxs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3dxgsfvsb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rhifxkko.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3woluesyq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3husjwhji.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pjnyxaem.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ptitjgdx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3axjwjhni.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bmpmchxh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3embcsqja.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3xgjypkdi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ekyflwfa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3pweostga.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3heheisla.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nmerioeq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fdznfowp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wtitkyjd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ipgtmevx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nfncmcxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhryqymb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3svxkhhld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljzxsygm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wpfdigkh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3syeuvbwd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3gnygyzan.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xynuxmkx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mamuwzmi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3eonbtwrj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3rqaanvip.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ogeuwuis.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3scyctups.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nlnapmvg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ogftdihr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qemvxaki.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xuqaauhy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mhmhbcts.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ihwyjnyn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3cxmaeplg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3njsvevys.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3sdcyzvxw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3boswxldo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3wizxftkk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3iqstyuko.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zilubbyp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yegouxfc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ppbffcbt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3diwcipvs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3oohybkfn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3uwitdoad.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3pyszehyj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wuxkuzpz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ybbgnczz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jjfwijjc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kqdpgrtd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wfzwtkyj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3bwfuenrx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qulhphwi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nnzjapzo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3foewcyba.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3petygcso.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mrkeceji.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3tinnahas.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hiippsjq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3jupcbizb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mkzwteqw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3otgbdyej.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3peoqjwxc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3pnsckuxo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ycypczir.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mjiurlbs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vlvdfxkb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ulfrsfsv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgkuyfrx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nipikarv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tdmzwxjs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3soxemtze.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jhqxkoop.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3fjewbqri.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3vmfvhoxd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3unixvivj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lrrxkcxw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcvljgzg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lkaekcbw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wxgzehsm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ytrwmplx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3bldkruos.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pyfaelnj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3sopumxmj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ouiajesm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3eawltpxx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3djtunbvb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xwjsmhjt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3frrmkecr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3pfowkpsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqmkepep.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ntijkbpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdcynimh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ladyjqfp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dvfghpon.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3krcrultv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3iuucjxvk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3rgbxlqhf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3buhaakwf.html

);
来源：http://www.52xcode.cn/Article/details/gt3kwfdvdon.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3dapukrpi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3feuvokuz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uenkelwe.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qfaauctb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3xwarvjro.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lmnvtwoe.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vtwxttum.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xhmlgmua.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jrlpbqzz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3wvxwrxdt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ldwsrxmr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3kxiqvofo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lljbbxvz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ennthavk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3mkqacdzf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3nkjcwosc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3aylbysrc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3heorsdes.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xilrecjr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3pvsmbpmx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3awfaykfs.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3dtfoxwbv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3akmmwxga.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3muldlgjl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qgjmnkpy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vaktnylb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jgoitbdp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ntlmlhwx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ktxgygps.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hyxuqxbz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3scypuntv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3uvdexzzf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3plzbnzmk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xvxvfxjs.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vgebdwwg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3poidlbdy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vmrraszk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3uvsgmelj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3aeqdfkby.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3acufxbvt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ijohouqt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jdigpqsw.html


<!-- 参考信息 -->