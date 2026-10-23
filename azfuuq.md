代发 wailian999

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xllnngnk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3wxxvetfl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mqacquzc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3yyuyyafy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ptzbdwye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctqybxum.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3enxpuekp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpbuljvw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fcgvqegm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iejvrrac.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3olezbbsc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cznnjimh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bwubkamv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfkkzxai.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iuvdcoff.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ajmxwdqd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tadbcyop.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3grkzaefx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uiibmvzr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uptnpfzs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3inzdyxdm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3aafcbrow.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3gfqvrenq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3iqzwmzne.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jklamljz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dwskcgrf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gyxoiggb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3zgjnygst.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rplsyvvl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hkicpavu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gwyyyenz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ypvhqrxy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3mwxmpauj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3apdtxsow.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vsuptlih.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3kkmxjdsu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tccutosy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhihzend.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pwrojvpu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gxdznkpy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3etjdzpso.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ictskztv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bulpjmzv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fpgdofpc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3upkklbun.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qrhvhxdj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdizpyie.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaqrifov.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgxhukir.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lmxzflsh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3hrzsgkqj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3musgrlmm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jftdawqn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cfujjjry.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ezllfzjm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tofxmaxc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jujudamc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3igotflyv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3srmudoyy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ctontuwg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mwlgdccf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3srwganqh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ryfvmvrd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qxjpyuxl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3muxnmoaa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3relmmwiq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ouulteau.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3pobjzybp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3roloqsde.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ljnslhev.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3fgrspnui.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3bnlvfiek.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fnlcnyny.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qwuxeppb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tkohimpk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qewqtkoa.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jmstjqec.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3foqkebaf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3djnxnxat.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ukjvpvlr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xunkdmrn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cweqvnjr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nvuwjnpb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3empksghd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vwkaoyqx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fuhvtkjd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3cbdpfrum.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qliaczvp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ncwcosmi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3lmzkncwh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3xxfnnxyr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzcghghp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3syxwcynh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3faflwdma.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3hedeylya.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qavdlaiy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qztsaazg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3eatunymn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jgjkhtho.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3fbvyjonp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hsckvwwx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nlgzisfz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lexxzhvu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ibimteuq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3epivndws.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3maityrgp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rbvdryrk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fbnqwooq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tshukdvt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kmzcpqno.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pnhunilx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dtngbgph.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gkbzyxas.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3omurnhip.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ktszcacc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mouyurkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnglbbvg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dgqpjklv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayeftonh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rlljrbfg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hplfoxle.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3wjmanfer.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3cwuoxjes.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fwtdgvhh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ypoziwce.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3scgppquh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3prkgxpsg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3biiqfqpc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3cvwkabhd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3cjogouce.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xhboamfd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bykizpbv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kupgahad.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zqbehvfz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ivyzgnqs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qgidemjx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3fqrwyrgx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wglfewpj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3aldovzrv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3maszokmp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3werrhuka.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nsdiwzkb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mkvcwpvh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3nmhytwfn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3loosdpmk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wtsdsrwt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hbbsxbdp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hlxmvcgs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ysbrroot.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpgkwixg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlvouxqa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3bpcrkytm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3adsgcwct.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3oowvhkwo.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlrlfdyg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3inznlaam.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3llsjzzkw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3yxfojiuv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kvzhqvbz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dbddvimp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rsqwcdvg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3qjzrorpv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3exrgqcmj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3eobbvxrz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3fzyongvb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qbcgckjv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hlqkfqmu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vmuezpni.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ftwknwna.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3uxopxmuv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3mrbyebwp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ccvthvru.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3iolgbxnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqeihtxv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3fktoslof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqenyiih.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3frgbwsbq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ymcellru.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3sovprcue.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3naswrrlp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gyqadwry.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3grwcjyaj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3epmrynpo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gjdapocz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jntctfmy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3vnbtjvpg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3gjnjslex.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fwqanhsl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tsmnzbhd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3hueyrbvo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ovcksywg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rctqdoik.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jwvqeqne.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qzobrpwt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nzogonar.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rijzgstp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ounnbtrn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3sqwdfqzp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kfgsqtab.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qdbjazww.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3iqilttov.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zilenvvv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3jrsyettq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3dqrxdljr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3vbebikch.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vtsokrmh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3unaqgcmm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qzrrbuig.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3eqsacqfc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vaqmcakp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3rhtdptqm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pogbwfuv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3pizpmaik.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3robvypkg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xnrgbrgn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ctvzwkkh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ksjulmhm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3owolzhuc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rmqpnrgo.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3wbpzawqd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3dwuiagnk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xaakelgd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3zheezxlb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3esjokxqu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ofzyxzgp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3qouvihoi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbjunnje.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ktpdczhz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3gaeiixyp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wggaencf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ovbpjgvw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kfmjnhnw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hnprnrbb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qrtwyyru.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fjptmseo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ejejxnmi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3lbvpenkb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ebrjjsyq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3btsxgcfy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3lfxjtlzs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mkcvfkym.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3vzxcckrm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fihwpcrd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kkcxrpzg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3sugmaxtt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3lavlbrva.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mrqnlfpb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3lsgycati.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwaxtjmv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3eycpqcvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pytexlza.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ycxkmhkw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3pdcwgoxr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3kvyfnxwp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jjreqpjn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3lxgaawoi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3klfnbtit.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qakrhmkw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zzuqulmu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yrtwrmdh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wbegztie.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3iavblrgm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ekvimkev.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3rijvjxrl.html

);
来源：http://www.52xcode.cn/Article/details/gt3dispsdlx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3nfclgffk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3acnzuvqq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3pyenmbqj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3noamjpcr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3epsyqlyv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3yqjsdqmk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3tcokfbkf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xvwskrox.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3jjckvgcz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cmqkrzvq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3hdnpuxxk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3obmncrnd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3itjsxljv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kgvjabdj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3kenojwrn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gtotuqex.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3abrkbbnp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hrvxpzdl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3jmifpyie.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3jrncoxkh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3dwwcifuc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tfrzvjek.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uinkhrkr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ebswmiki.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wimhwxzn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3tsoojtuf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vnqtnsrq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ddgphxfq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pfcsaxek.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pzqhhvdf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3jdwwvatv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tjxcwoif.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3xaxrnajj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3oljdhzec.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3juhhmcdy.html


<!-- 参考信息 -->