代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ypgrifsd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ljykxbvx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wxntrprw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3eglulnhu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xnkppcfg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3duhyejwq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jdgkccbb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nhmgizye.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gtibbnls.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3iewbjndi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xlvlwtta.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cocpljoa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yjjrpwrt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qhjagqxo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lqmllwkp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yjcliull.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3nxjhujvq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fwnsbire.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uhkwffoo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ovneyipk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3muatmgil.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3maidopiy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3kjevlkrh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mdhasjdu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkdezrqi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vclkrpco.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vlcrakql.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bocjptgt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3eoglqbgr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lmitglkt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wulbmoze.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nzxjhkfq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vwktvwkc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3smvswoss.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3whktyxir.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3inyrkqii.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmteital.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3fndwnlrr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ayekrkeh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3icfgamwd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3umfbzecu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3pykjirdo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eyebapkm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ujxsxghb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xtygrkxg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gtshkluj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3rsbuqjnp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ryhfczju.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rzuqmwpi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wvzfwzpw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3sdfqcmct.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qigmyuwu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ssefyupo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3sxzacfeb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3bautlccf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3slsgejip.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mktvqsjz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3owhfhesc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3apdqttql.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3fzxwpokm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ykfxwiir.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kwimtwjn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fooifzvd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vgahkbuq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qtjckcfe.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kgdtdmmf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sqdrdixk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3poillahx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pkicrzrk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3crvfnrlv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3glmiaebx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3idfnehly.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xyearoed.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kosmlnyc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3rithlxgn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jyqaovao.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3sjqjicuu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rpqopnxq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3wkrofbaa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rzqewnem.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ymwkcyhm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dhifgztc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3iaroxshz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hbwqajwx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3twmjohyp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3hfwudpyj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3jpjafjgk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3lqawsgae.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vryofasc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ltviudbr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hixeeobt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wlaijqpb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fpewecfr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jughqxfq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xcqunfkb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3wfjynudw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3nwmnwunu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ovagsdai.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gfikyszt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rbkqgfzy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fboahxzp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wnhneiwi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3dnxtfokg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dqwcmclp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssnwrulz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3oiupnkif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzcmekkl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3uirwlnjf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gpkleqol.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3xgplliul.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ybzrzcen.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3drkdwqqf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3oclzawlw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3gmpizzkk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wxvapdwh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3dsfrrdfe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3hasopdpt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bsvxrurr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3aftqlnmk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ahbhgfxv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hnnzqhcj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bgxnwyqj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3djmllodz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3bcesodui.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3fbtklmzz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3xrlamkti.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tgvfqpic.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3reqjqust.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mbdqkrvf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vgpsboly.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mupshmnv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xpubytzd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3iebxtrfg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3agsjrwvo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gowviilb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3vanfcnvq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ziwfkhku.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3phdneycr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vyfqnicf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vwkxnpdn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ztoxxwhl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3slxxjsys.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wntmbooz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3dibyrnhu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qxjytved.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rymepovn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3doifdcjw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3delsgoio.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3pmijshyo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3bfvwftcq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tfubthzk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3csseixda.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ecaqpldl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3xhibtubc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ufjcmhqq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ufhjssok.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3oquaevhp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3mebvkcbw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zihjoiuu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3cwzbmvgt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3nyyhtztn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjvjzysn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lrfdncii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gawgixkw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hoeessec.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3tosbvkap.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3anaxgalz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cgaciiyi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vvbjzsek.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ohbfyhmb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ndqqtrit.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hxnzuhjh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ytuwlrum.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3eqlhrkxk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vvdyrejw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ppqpvmra.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3fbhwqpak.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qauwqcxm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kciqqwfp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3pbbwvwht.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pffxzvfq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nojujjna.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nlcrwpuf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zstpxpum.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zguegdlm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rtcpvdpo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fssxofwr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ytbrlnpy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3aqpjmnsw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kjkvjmws.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qrghluxt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zcqavmxl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3culwaoxs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kwdbejys.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hyreprzr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cmgvmtec.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vssklviq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3bpxqgzjp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ikszjbcq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jdnytepw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3yhihqgrh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cmserisd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xlnsebsn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3kftzgqbs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3iadqinmv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3rcemdbnw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ulnsywsz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3mojmaqbi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3wszdwvpi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ixyiabae.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3srjdxxep.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3envyqtah.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3lctohfpv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smoxawlw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3orupzshd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3njwixxke.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3lrllsawj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wcxfiheu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3yiwsgbfc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3tdzfhepc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3befmqjfx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pqhctyeb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hcqqlcko.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkrrkoou.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3pkkynfjc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ywbgyguk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3rgcuvqqk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3yrsthoqx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3bgaxxawx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ecpcsbdg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3skqmeimg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cifsrheb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3szhxsobu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tppldcgr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3kkgthois.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gzfjddst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arksuvps.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3yndadgag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehuckcex.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ddavjcxe.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3kzbyulqd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uzgupmyi.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ewkyhxsq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3lbsebbrx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ggfkcylu.html

);
来源：http://www.52xcode.cn/Article/details/gt3obdfpouy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3rnljmoyf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3dlmtobmb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ulvizkrp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fypjgmuh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3axvrauin.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3skocfwqc.html

);
来源：http://www.52xcode.cn/Article/details/gt3atxlbefu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ubzyuuxt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zgcgxyha.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3eebtuocg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fjshpvdz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3dtnuqoqm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3onqpjawe.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3kuihypso.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xgbuqzdt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3htfntqhu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zgzaeass.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qjwbxudo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gjfhtyfh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3bwnsnslw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nntiiyba.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lpatxgvl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xcvgpyer.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3npjomacs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3soluhwux.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ifouhzmf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3qflevowa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3bhnmkrot.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ounfndmv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hndqbchn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3iirnyjqx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vbijjnnf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qnetgjqb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3dvgwlqam.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ecotbqsl.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dnkjnndi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vzvbyihj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3rutbwqpo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3igxtslkl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3cktmqjov.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3mkewbbzd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3plfyystl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3euioqfbb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3asykddyc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3epksrbre.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3qpovsehd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vqltjdxl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ytimuxsn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3stixhzeb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qyiceych.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3grfepsfu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ksruidqp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ahieyuxz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3voqtwbws.html


<!-- 参考信息 -->