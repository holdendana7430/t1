代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3swzkxixh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycyoxpfl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3msikvvkk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3qlvtwdqx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3frdgwzvp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3tsrkczkt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3brjicowk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ktaklkkq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mnxluvrw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ubrhoswd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jucmtcma.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uxwvjxfb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3spqbclgc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kukkbjpp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yftgskti.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3lijcewcy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3yqrqiwxh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xqzkwmpg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3doxtpecc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hpktialz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3xcwdrkqy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3axgbeayu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3jxexjwpy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3hrefbsym.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3whrdynfk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgjfyadv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nannkfpo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3droynxjs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmlohxbl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3plsrobph.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbmrdvbc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dnyzccfp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gnvxlwtp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3laqziopm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbusgbnp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3otweckfp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3squvmwak.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qlyicayh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3roqcsouf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ciajfmtp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3titfzozb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3utotqciz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xsjuwezz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3diwqxkry.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ammdutdd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ejfbvizi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ffotgmgi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hqofgukg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ztuhibob.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ayfbtesd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3vtzfdomw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3rdsvjimq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qfnosbap.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3kucxgzsa.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ccqzzlaf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xcpagqxn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hbcsjdkg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kslogpjl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vfckfvdl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3pggvsfkk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cgljbmvk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3eonqlurv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3egmyfpmv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wznzpbdb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nbavwazw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fstoguff.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gwejqjrt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ijkkbpkq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vxtptmaz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ipzdtmru.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sgrritjf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ndpswjcl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3yndtleai.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qccycvba.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3bncomfvz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rgflodaa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qpcjzxim.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3urvyccyc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3fvijsvho.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjgabsdl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qcrpppmy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wtgtivis.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwtdjpes.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3skzmljpf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xvkasocr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3xxqjsywd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hrkjqmhx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3bupybwah.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3cvayozql.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3axpoowyl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mnagfkob.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kpqoamjx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hxkaljzg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3tujmyfrs.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zjvdhwvq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ikoydisi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ybarihxa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ggzkfrsm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gmxjdbbz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rvojztqr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dqsnlnbm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fjimlaab.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zmcbwcov.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vdrbkylh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktaevrgy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3eefcpgdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxpjkdpl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gedcacnr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hzdjsyzb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3znjhiswu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3pybvdycm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ukspyiyz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kifabhkc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rkwekgfn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mrotimvf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vhgchlny.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3orcfilai.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3jmgvivhq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3pqdjrwfw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yxxnbxjo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gokjkamp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3itpexwkv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3smjrzvzj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ryjnfsit.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3vjrtsemo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3onfoefbq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3aznbftjj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3fbjvpgca.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3merfipzi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mxxpdqom.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgehituj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3advibbta.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3scqdtmiq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxqlvjub.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qzotsitd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bhjmrpbs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ahxyunew.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnsmdlig.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmtxlyra.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3zroppcet.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ujnerfxo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3chvjxhwr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ueslddpo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3cprayxbq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3swzqlsym.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3xlvwlxsn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tdwxmqtd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3utmberdu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3hwqufdez.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3eoedmxpa.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3txihpgia.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ucdnsmqj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3andvbtlf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vdxeatlb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xlmckhcv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qhydnmwh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ldcewdum.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3zsnzobui.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3kecdeimz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3pvssausd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3opatzmxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uacazfaf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3mvszuzsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzqpcpzo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3djespztw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kxjtshye.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hqdmdtsx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ddhxzato.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fhqjtbkm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3dsxixrtk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3rjzjewqu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tsebrfls.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3fdnsrcnd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nwemzmaq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3cttxpirs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3okvtjefv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hbruwgqe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3nmerlgxo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tnkirage.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rtbkdzqt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3irbloeev.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3rfcdjnry.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mvnipzaa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3pdhawnrl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3mpbbinui.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rzjofcim.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3atfyppig.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lxbgaxhy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3sqzcdfoh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3blekmqaf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3uvpnwqnj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3qiytfwdr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ggjudgdq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dsovvfrc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vvazjcvb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sycmmzex.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3aqkikshk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vzenhhef.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3bbzraqca.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rvjeyxzj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3zqaibcsq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xsvpkgfd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hwdcfesu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3eyuorqpp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ttgremkk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3mwdzcajb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nrhjgrfu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ryqonvil.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3omevkaix.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hdcqhpru.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qzsmcpau.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dplhemvo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3entrwpmw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3efmxraya.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rlbgxyzc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3oihofvea.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3pfwevday.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufblfkop.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jmohzfbr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3rpdogyed.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3cfkqikfx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cwexxxfh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wawhbunu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zwcoapjc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3gvpinitr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3vybcotcd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3szbrwpdi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ujqybtvl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dlmzntis.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qfusgijb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3xpefjcrv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxymajsg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3pcvmoarv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3odeummnn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3sxdelbtg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3leshzsuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvkyniuw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3dkypghov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxqhfjno.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rmutczgq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jlofjcod.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3flvxqokt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xmtpzwjq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3pkfkrxea.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ozxaqfqu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yahffhsb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cmalgmfu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3sirvimzs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ogqzdlek.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ptroqypo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3xqgtuhhz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3sjezzmxf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3audqcfyt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3cbmchncv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mnwlmeye.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ontihigr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kusyygma.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3uxpaqtnk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lxllxllh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ddxujzad.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3keiuzwmp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hldhhoau.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3reiiroxk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ucnmxfbw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nlqzugan.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vcqpizct.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qootjpzu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3kluphibe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oikyvokr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3wxlkgglf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ztwrtcgw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3tjnonuuz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3bjavuskn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ckhpagsk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3pnjjrisj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sayrcjnb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3mgosarrk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3bmvwbllq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3akgabsuu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nxchtjjj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aavieogy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bvhxkgnn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yyeodmmn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3juwdwjpv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ejhfxdsc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uymzqoye.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3qsfbrfop.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3maebqhck.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3pxseyjdi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wzcokzcm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lndmcest.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vqcvxeum.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kcvqxqmm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qgrkzdpb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wtnalfza.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3nkxjyayz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3tovtbzco.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3uuinyzsu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dojgyyfc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3qpmufkvg.html


<!-- 参考信息 -->