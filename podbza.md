代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sjjwwnzh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mxxuwiwi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tngrcavx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3eaxsuzgj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gaittnsd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uejweswd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ojdlghhs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jznkdiea.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aksmbxjh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lgemvail.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3pugjeitj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3jwyroesl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3azqwgxvd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wqkqnlxp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hjhbsuuy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yrdbowhl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3eeqqglxi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ktnjfgfy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ehwosotk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lknqlokq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lucpobos.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjtcadfo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uaxgfzcb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vrlchyhd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bncblsje.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3tdkoyias.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nvqhyquw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sqdglewk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ztsakyti.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mkzictah.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jjcghhbj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3riqaprbw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlesudse.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3erctcdzf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3tcybdkbk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zopnwwyj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jbjmydor.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zeuwosvk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vdopeiwm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tkyvgufg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3figwhcvo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rkfhqppj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ecukmkit.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mwdjxehj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3upqhevwo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nexceijm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3uivgozum.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fcztviel.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3yqqqzmvd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3kcfvvuky.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3boqoojkq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ktmaqfrs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ppqylrob.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xxiexjqi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3bhdljplz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zpmfchgr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ttgzespy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3qkttomef.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sfujzlhv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3okbuqczi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kuprugsp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xzghnspd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ravhspdl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bkghbnyp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kptsyfzd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rtmkpmvd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bwtuyqir.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kxzdcilh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pkfumdyw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dklojiza.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3eetvinxu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mbxbdaud.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ywkifvln.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3mxmewxtx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3htajqecx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3secdzuex.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ecpihyug.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3tsyanbfi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ophuiacs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3iguzdwzt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gndecttj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3sxzzzore.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dhylqeun.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3nzqwlkqx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3aeegorlw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3poukithv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nqjrimgm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qavhmlma.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3asokyjll.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3uxdejyqq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cbucclgz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3vmqhltrh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3orhyuztv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ssjrmibr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3uggyvgfl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3epsxauwe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kwviyzzr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3srsuvmro.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nllxwnfg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3sqbupjeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3untlbubk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3wxtcqetb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbjcniul.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zcpafupo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dkzhwywb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3kdrcjzau.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3aamgdenj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nmakosmw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nvjcivij.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ytqkrndt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dxtqsqng.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ltffqtjd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ehudjhss.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3aztzrpvu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3amxdivkh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gupouquv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pvexefnp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3skcevmgc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3qvwxrmnb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lrfbdrwe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3jhcftqqe.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xapwalsk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3toicefoe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zhkpinzl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vcdhrcdx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ibsitmah.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xzjwiaso.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lhpgsgcv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zvoavdhh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cyyzoess.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3stgkcwuk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hzrxxbsj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qfnvyiri.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zpewifdf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3eubntfnp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3uaqschab.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pjyfhffl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jiflcwyd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqvyuokq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3agdvcssu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3etqjxpjr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3pfpckbqj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gkbqbaas.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zhlylapn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3qhvmrwfv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zetwbyos.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cfxlhnav.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxuincuw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3oygktudz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3whdlpqua.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qusdidal.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cdhcpxqa.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rijgqfti.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3aqylaacp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3jjmsbqtw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3fqgiempz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3dtinwcva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqplorhb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3cqdizinr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwhydglm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3phyxcapk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fmnnlwcq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ytnuqyrz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3simosieo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3sbfosfbx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ycuskcmq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3woharxaz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gjzexarp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vtuizupn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3yftsrywt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ofqauqhf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3evkbxxxh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wpowjzrt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3uvqxlfvy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jykeqfxx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3cvxcvdrp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ghupwkgf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3whivodil.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rrgfsdri.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ybsuwgfu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qlgaedmc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vboazavk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nvvqzjhq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3suyjmift.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bgmzxooz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xbbkeash.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3znmxiqow.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3jydlnjox.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tqikxlma.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zchljnkb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jyyzexcv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hdqxmlfv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wbmrelbb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3zlvffwvx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3gglsubjk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3grpfcsna.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gkiflwmw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pxnqmhaf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3jjinnsdg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3iszioqrp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fuwrpozf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3nebbyumb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ajjackfc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3guemrfgu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ftmbhabj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3keghvaaa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3nhruqbds.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wfmlnduy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3pewwtcdr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3tyopyshk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxsbcynn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3pvkychfk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3pwjzmtln.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3swgaikqd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3kzxzcqxk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ayyknlwm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ivmxlasx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tcxdhsru.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3csqjhtph.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ihxfywoh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ciodrnil.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3hleipskn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jtpjhcgr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3rdbpvhoi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3nsptevfi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lgqidiac.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3sifyfkap.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bokclmxm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hofhuclp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3qdpkevdo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3pbddopzb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3dmdloyvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chduhbcw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3eyxygbgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umpiswhu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wxtjwjqh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dfgajvch.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jipzgdht.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uxtcvdlc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3skctbhoy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3eleoiwkz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cewvowyk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3cgttcyed.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3anxahzcd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mitqgrfd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jhtkqpca.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3frgopkby.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xswpgnge.html

);
来源：http://www.52xcode.cn/Article/details/gt3sshaferk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zaplzzdn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zicblame.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3fjcxmvht.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3plrdspwu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3sphnxxnw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3chbtxtwz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3oxtmmmmq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qnyznggw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dpyepadq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tjenoeno.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3dghuvdqq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3efiglfow.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3diaotfzg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3itrsxkpb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3yrvixgbg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yqkhkipe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3dmplbmrv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dxoomfdo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3kttxdckv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3dnqjhgkv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3embrmngj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3bgxzgnwv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ykrhbzhx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gmauwetz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3gufetmwr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yrcpqxwx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jdblxhrr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cnqeqcwz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3uymsnkre.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pqaxsete.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ydzzgvlt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ryywwxdn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zukbqfcn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3njzagmku.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3fhwykgrx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jlmhqjxe.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cqjjgqsk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lylsmsvm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ottpewjm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dvzbgxbu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3gwmdqudi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3kpifrmlc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3dajkvmrp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uryptvsa.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gqexqmbv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aoipniri.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3reqlsbqz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3pwzpbcon.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3kaepkhxs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vpbnjmmu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jzmfxebi.html


<!-- 参考信息 -->