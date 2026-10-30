代发 wailian999

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gyrbnnzsg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gxfofvcfy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gjsmwqnfc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gvfonusfy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gjuxhsezx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gqnvimqdh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gaeoyletw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gjpjyhwzb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gmpqpabil.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/grnkkyhmi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gwfjgxxpg.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gxhwzshhy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gxyuwtvtr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gigsxpisl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gfcjjrzgf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gtnkibrih.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/ghunbnbdo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/giwliuhbs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqoewxkqs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gugdjxuul.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/ghzewiulx.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gmgpbewvg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gezreurox.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/ggldkgomh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gufbmfari.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gnqhptbiq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gkscxaxrg.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gyqkjurke.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/ggmosgmcj.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/ggsenflap.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gecxjwdbl.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gftopxdsg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghotywtpk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gqzvzxadf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gzxadnrqf.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gdgzgvcws.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gpnazwbva.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/ggsfeobsd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/ghvnkfuzr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gdwkuahqr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gzwziswuh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gjpiewcdi.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gajmwwcvn.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gzkndivpy.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gdtwhedrq.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gbdofkfpu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gcwhoawin.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/guuewwyfv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gudrjmdzi.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gfisrwikz.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkoefehoy.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gifkclgos.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ghbugskww.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gczjjstam.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/ggozhrrql.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gdpmyalkh.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gjtlozhid.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/ggnikvfqt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gevfnfpur.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gldqnoqno.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gohnaxoxx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gwickqqjy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gideaqqph.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gskdgoriy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gewirrmsz.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/googdjfem.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gtkxsuobc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gfmvtogvn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gaugbzgiy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gdhnmthrh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gkaklzksb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gknkelccq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gslmddnkz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gguqavhso.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gchgdiotk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gighyhrqd.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gznxhxcpm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gopcrgmqn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gyzhhrbwz.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/glzlgcxvu.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/ggnfwqnju.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gigxtsxib.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gaqeggyeo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gjdvqpkeu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/geaibtisd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gvuvnbrou.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gnsipkwsm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gitkyubre.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/givnijacp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/glmjxizcc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gqslnzjly.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gfutwoubo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzxhxzwph.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gaxxhisfk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfzyllumd.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gjkplevus.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gehtkjjev.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gebucyjkn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/giheapyfr.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gndlwaphq.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gvuvlncps.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gvjoiujgk.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gscomytaa.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gdpylthca.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gxcwypsgz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gpppkhqpx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/ghuaaytxu.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gsrhcmzwm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gnsrjotac.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gyaopjmhn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gyheofmjt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/ghqsyntts.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gzzjrqaoq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gzkjnhwwt.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/glejpwioc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gesxckjmk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gwicebnkt.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gcsusinoq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/glaslobvn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/guzwpcdgy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gqwvuives.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/guzhuwwyp.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/ghtoxsjko.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gixpbujms.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gmjntitod.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gxzckomom.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjjsrdftn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gwayluule.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gqgichive.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gmozzlckq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gseoqhaft.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gtxerjcbc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gdysdluwt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gdchytdwy.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gbmwhfgnx.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/glnzwqnsp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gtvyxdzdz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gqikrelex.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gkeajonwu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gwqekuvmi.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gltaslzre.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/ggmvetwlj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gonobimrn.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gsvnaawyq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gilaneopo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/grgzjryqd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/grzizzdtq.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gdkflvkxf.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gyavglmcb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/godvajrfl.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvumfltlb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfbyuqteh.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gmjzwpopa.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gmwvxvwlj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gsmexclkm.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gyscwchdm.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gqvawopmp.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gcxeblixv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gbtecglwt.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gjuihviaj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/grnmckqtt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gskblmzvq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gzjphhctt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gspmnetkf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gcebhipij.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gwsmtcfii.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/galxnazji.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/ghcnoeflo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/ggsnxsaay.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gwzehknqp.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/grbacwlnm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gmrywtxbe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gdylzutev.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gbqxjpaft.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gmlhbhtlj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gqcefquch.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gamthgcvj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gymxuyvpj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gvyquvqqp.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gmhfmfuvo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gyxjrtmme.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gthegmyxs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gcudslkml.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/ggzbazdjo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gkznnqleq.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gjuamsajo.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gmibltciw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gwknydhnb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gyrftlbks.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/grvubedsg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gswihfzts.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gbgvimhhh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gagjjjsyt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gtwyrdjuw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gioortmjf.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gpkknmcad.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gophscdvs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gixsjcfaj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gqhjlutrw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gxgyrdmfm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gswqctzff.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gjequatvh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gwyadvvez.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gnktsvywe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gnkpgnjfo.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gdcttbszn.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gqayibrpa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gpscfctbf.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gihglhuek.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/ghifiiqtg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/ggzqogwup.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gqsvuzpnk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gdpjbobzj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gunsviqxu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/grbkntinu.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gtwcgudfh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gynmnkvkw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gpxbxmxto.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfbuxzx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/glyrlznnw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gyllggejv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gsavmltao.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gqyouskgq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gsdkaldny.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvvabkdac.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gysuyxsrc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grxfspczy.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gbbkougcl.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gbakoboeb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gqxluyajb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gqcfmnezl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gmtmrgevw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/ghnwepogu.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gplkfcezl.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/guyyrdyws.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/ghnddbdrd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gdkonptfo.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gtlmkrptm.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gcbtvbxue.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gfbxlrdyr.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/grycypzju.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/glqvbzfgu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gfqvlwxgs.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gmayendep.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gbxrkpgnb.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/grgbjqrgq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gfuisrukb.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gfvenmbeb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gzwyugojf.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gyusgzpdr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gokoenbsa.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/ghpldkxsv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gpspnitqv.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gqfbwkvsd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gtcfvjqfl.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gengfjhyl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gpefdckyk.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gfkyzwhsg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/guwarlrxx.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gdsiqpgkw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gimbgjywu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/govxlmowt.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gqvfrpgul.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gpqeuzzfp.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gwjzqaqek.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/glxzedqpq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gxjbmgfbb.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gewvnvsuu.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbuxgdfei.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gcwqmkfdq.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geodzildt.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gvunbovqq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/glmfqleae.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gzhocgqsh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gzyrmyetd.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gdfaioxyw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/grkwjrddr.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gfapykxdw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gmnhavijk.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/glkzfqflq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gceqeullz.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gufkhbmux.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/ghyruutcz.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/ggtfotusm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gsstwtyqd.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gucrbclfd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmrfwfepv.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gyqlklhmq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gcyqfnuuw.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gcwrxzoav.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzjqzbvzv.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gbkmippvu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gqqmzzjth.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gdcnqfbdd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ghrfxqlnq.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gxplmdbem.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gohptsend.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gcwukmenl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/garqfcabc.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gpusjqrep.sHtML


<!-- 参考信息 -->