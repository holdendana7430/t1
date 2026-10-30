代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoqnpuve.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fanxiaobao.xyz/Article/details/gemivxkdf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gasrniamx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnltnftta.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsezyahb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/glbxtyfiq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gxveqefgx.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzkzynqz.sHtML

Ruby: arr.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggplrfkxn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gicpizdjp.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/gqllbvnzm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fanxiaobao.xyz/Article/details/gcjavxikt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdmrfupm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoqpymum.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gtkgdgiho.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fanxiaobao.xyz/Article/details/goipbwxdv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdweqeuq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvigvhis.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gduroalwx.sHtML

[N04] 斐波那契数列
来源：http://blog.fanxiaobao.xyz/Article/details/giefkhvjc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkhxnesz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbihrugu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/glonegkyx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gbxzgflev.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/giyltpybj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fanxiaobao.xyz/Article/details/gemodsuxc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsjdgtxc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gggngagtg.sHtML

[N05] 最大公约数
来源：http://3g.fanxiaobao.xyz/Article/details/gkmljfoos.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbblnggv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gosfersor.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjvnjfwur.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtbznylxv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkvgkwpd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoqmlkqd.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqqcyana.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gypejcywy.sHtML

[N06] 判断回文字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gojairjsx.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvxzuwfd.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geswjnfup.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/grilkuoxt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gdanpktjk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgrtinpe.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvozowal.sHtML

Ruby: s == s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/goyouganz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/giynzkxtl.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzjgdjqy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fanxiaobao.xyz/Article/details/gwirhtqjd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyvaprud.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fanxiaobao.xyz/Article/details/gxngsaqxi.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwksfnbw.sHtML

Java: // 手写 HashMap
来源：http://wap.fanxiaobao.xyz/Article/details/gbkmtannh.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gndllbjqc.sHtML

Ruby: // 手写 Hash
来源：http://3g.fanxiaobao.xyz/Article/details/gbarnmwxm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvvvibwq.sHtML

[N08] 生成全排列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytfwowlh.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/guxuthlaq.sHtML

PHP:  // 手写递归交换
来源：http://wap.fanxiaobao.xyz/Article/details/gnqalxozv.sHtML

JS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/glurpksfx.sHtML

TS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gfebfuris.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbplwuyd.sHtML

Go:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gnmwswher.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxfeqcph.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnldevuv.sHtML

[N09] 栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/goykvydub.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/godojgvdq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwyterco.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gttqojykh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmbtstci.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gbjmayuzz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fanxiaobao.xyz/Article/details/gzjkyzvzg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gokzohmtz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fanxiaobao.xyz/Article/details/geikhqttc.sHtML

[N10] 链表节点定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gfppvbenf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fanxiaobao.xyz/Article/details/gttrmcwgb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdxjgmrkj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzifjdddb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gywotecfz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfvbsnddg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaupetqg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fanxiaobao.xyz/Article/details/gnwdbffgc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqznyseht.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/grxnciahs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fanxiaobao.xyz/Article/details/gpoinjbux.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geswsbtsi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/grqjwoffk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcvyhfax.sHtML

Java: // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gbjzdptib.sHtML

Go:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/giaqaucyv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fanxiaobao.xyz/Article/details/gzrhxpdin.sHtML

C#:   // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtgtnpxx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbnysjwp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gbngbrmda.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnhdpgfz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/grfzrtumd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/geakbxtmv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/ggghxtitt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fanxiaobao.xyz/Article/details/gmoclmebc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gvchzvexb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtfecqdv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrjcqnje.sHtML

O. 并发与异步
来源：http://baike.fanxiaobao.xyz/Article/details/gbatnudwi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsjcqhgpf.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gotcvuuqp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnjqblyx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnravlgy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fanxiaobao.xyz/Article/details/gfhnzxkdx.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqspstjz.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fanxiaobao.xyz/Article/details/gkndloljr.sHtML

Go:   go f()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrnnixmv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcterjcq.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/gidzvpduq.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/giloghooq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/govfqkqns.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fanxiaobao.xyz/Article/details/genzokhhj.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gljttbtsf.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gjahcpdxc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gdqhajspl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjontqgb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/gnesldhue.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fanxiaobao.xyz/Article/details/giecmqhev.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvqoynfm.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogeaoxfo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fanxiaobao.xyz/Article/details/gyejqfloy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fanxiaobao.xyz/Article/details/gztfjacwa.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gucqniipx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjecxdlfh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwooemkvb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnomuwayp.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gotbelyqk.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmemgxoh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fanxiaobao.xyz/Article/details/gayyodiix.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwggletj.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmymrtle.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsscdcpjq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvtygoiw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaivvghdj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fanxiaobao.xyz/Article/details/gzlcjgwro.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gsjmyuyfe.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjkhyrpi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/gelcbbpnc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcwmpblq.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/grrnfeove.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gvsbclefa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/gthgzpjkc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fanxiaobao.xyz/Article/details/gkxitsmyy.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/gqlbcdsri.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjmqbfuc.sHtML

[O06] 使用进程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrmamhjz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuefodlz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gswxuzmqt.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gaxgsdcov.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gvlpmttfd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fanxiaobao.xyz/Article/details/gvwqdcbiw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fanxiaobao.xyz/Article/details/gforfngte.sHtML

Ruby: // fork 块
来源：http://baike.fanxiaobao.xyz/Article/details/gzubizevs.sHtML

C#:   Parallel.For
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvowsokt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqcjwkbhp.sHtML

P. 常用工具函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjsazooib.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuutfags.sHtML

[P01] 生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gxnbzoymn.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fanxiaobao.xyz/Article/details/gwutppqsk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gmmwaiegy.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golashxdi.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzychjty.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtytikhzq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gbayiotgq.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaztaytd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/glfpapcxw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmelgvxil.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fanxiaobao.xyz/Article/details/guiqfnwkk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwekynyda.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdqanwdt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fanxiaobao.xyz/Article/details/gwhczjkac.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/glqsgccmg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkympjxh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/goisvxska.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fanxiaobao.xyz/Article/details/gzobralxj.sHtML

[P03] 生成短随机字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gbhfpswhb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuxjqtzh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fanxiaobao.xyz/Article/details/gnjtcdeon.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gltdotzht.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/giqmnrmfn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gmxhgtitj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gowbhnbsx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fanxiaobao.xyz/Article/details/gxnhaopda.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fanxiaobao.xyz/Article/details/gioqgldgk.sHtML

[P04] 求长度
来源：http://baike.fanxiaobao.xyz/Article/details/gkwvhpjge.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fanxiaobao.xyz/Article/details/gftxoexwr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gselgyisv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fanxiaobao.xyz/Article/details/gxtbratcg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gepqwetnl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/gzwyqtriq.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpfqtpkb.sHtML

Ruby: x.length;  x.size
来源：http://blog.fanxiaobao.xyz/Article/details/gqrlazrew.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnasjmvjk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fanxiaobao.xyz/Article/details/gtayqbpof.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fanxiaobao.xyz/Article/details/gatgqcbri.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fanxiaobao.xyz/Article/details/gikhwikpl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fanxiaobao.xyz/Article/details/gduuutbiu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gqaneqkcu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fanxiaobao.xyz/Article/details/ggrkyrcrv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gmogovwok.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/gjusoycbe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcdnlqlp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaclsuxt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhycocmp.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyqvkxyku.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fanxiaobao.xyz/Article/details/gtkfmvjfz.sHtML

TS:   if (x == null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtfhesqx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcrzhxyr.sHtML

Go:   if x == nil {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfzzvbkqw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyqzhoie.sHtML

C#:   if (x is null) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmcdcvmqh.sHtML

[P07] 防抖与节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxsxbzke.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaoaibel.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsnayddp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gyrxfxldo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzymejahp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkjvtpytt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fanxiaobao.xyz/Article/details/gmkmzpyft.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fanxiaobao.xyz/Article/details/gscxcohuw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/gnbfkfrvh.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fanxiaobao.xyz/Article/details/gkwvnsgoh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fanxiaobao.xyz/Article/details/glauwzrfm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gpnbkjenz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fanxiaobao.xyz/Article/details/guasvmclx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkmjusbx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gblxkfpzz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/gxqlpygfh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwznnrze.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fanxiaobao.xyz/Article/details/gamtjdgfr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guvohoobm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/geezzissy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrwptmgd.sHtML

[Q01] 创建表
来源：http://baike.fanxiaobao.xyz/Article/details/gklwibtqe.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gfffbdwep.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gkbsnzwyz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gflqxuxtr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gqlrceswm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkxkvqdi.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvrspooe.sHtML

[Q02] 创建带外键的表
来源：http://3g.fanxiaobao.xyz/Article/details/gncrvtots.sHtML

CREATE TABLE orders (
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhklhyjx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/ghkucyjkv.sHtML

user_id INT NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gxqjyzdol.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fanxiaobao.xyz/Article/details/gocyiudwe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfrvevwa.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gixhlaumo.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfzfrpfi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfzurqcx.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gljfvntsc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghekaknmx.sHtML

[Q05] 重命名列
来源：http://wap.fanxiaobao.xyz/Article/details/gxfzimexb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/gpvjuaizk.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gryjxgbjx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyvsiunf.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/grlumgaqx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gijqwkuqo.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgalraej.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgtvcffz.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gwdvkwihq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzcrfayb.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/geytztwqu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/getalwuqv.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gyflbugqv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gucgeskbe.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gsbkweang.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gsyqqfqln.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/giackyqny.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaqpfsco.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtimgbue.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/gwohjndug.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gopwddvys.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gqlssyuwl.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfbyajnc.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamzgvied.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gotsjbjzz.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgbwgnqs.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/gqvmnohmw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gapyrabtr.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/grqnbtglr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkkazhyu.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gksgmueoz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gddxofhsj.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwpmjbbz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/geiukdmeq.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gshqirnfm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gbwqyllrj.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gpnmnnahm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvttxitn.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gxrjxctbr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsamnldd.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gousygcif.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwueloig.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaiimbai.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gmcjtbrtz.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gudthrudw.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlqiwctg.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvaisvbi.sHtML


<!-- 参考信息 -->