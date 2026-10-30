代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gjvzpraqb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gvdcdmiku.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gsrwgxqeb.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/grhgndjdp.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gqojrjcla.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gymzksqyq.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/ghcwgwqjt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gaceutzyn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gybbnruht.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gvflegsmv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/geoenyxbz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/ggubzlvks.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gtacgyyhr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/guhafzedi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gtdmrdtyg.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gjelwakcy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gluedjhtm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gbyttdmtn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gugmdjcda.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gmjrqdeiv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gjtnhvrkg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/giablpifi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gtufwwepa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmssmcdt.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gawamrrok.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/golvfmlde.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gifouhxtd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gnawxirzm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gbtioqaaz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gqpnvbepo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gjkvdzhwc.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvookcclf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gvgzvtmre.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gykdkyxcc.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gpdlvdhlw.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/grihhjpkp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gaoijycyw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gstexbshm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/glvhmbmdd.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gbxwkwwgv.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gwterxrwp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gmrfaypab.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gxgvjfmgl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gdqgybtuv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gcuqifgpq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gldshmzyk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gieznhgbw.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gfpesrdiz.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gghnzpxlj.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/ghxleokag.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gslnjoaxy.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/ghdkuogbo.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/ghkexdydj.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gaecdmdgx.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gqplvdtim.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gcqowlfre.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gaxsfyyam.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gdnevcoho.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gvlkiieaz.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gypphdghj.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gpbmevwxc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gzilrjukp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gczurqmaj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gyezryfot.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gnrtuhsan.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gdelmvtoe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/ggjwmohym.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gqjjwdoqu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gcrcwayas.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/glkxwlfov.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gxngmhunr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gqkzswukj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gshrearoh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gvmclluwz.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gjdcfsmkw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/ghnrlruwn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gzqewodxv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gppixeurz.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/guohcunfm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gtxqnjonf.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gkapztema.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gwnmbzysd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gfntkgfdn.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/getnhuwzc.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gxmkmrhmx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gfvdvwpws.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gvqdeokni.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gksriewnt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/glkfhsbke.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gyxxqcdkp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gpyhkywfb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gnefhmdqk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gjeeeoqlj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gbseujknr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gwmowcowr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gkdjfvenx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyfphfmkg.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gdrkoybfa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gklagnfrv.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/grllfxzea.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gwrinffpq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gqfuqjczp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gdpnqwuhb.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gkqcwxwdh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gljqfyoxg.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gftbbawqe.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gwvpgwrig.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gsogrmguz.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gskilqjbh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/guqidwmdt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gluztkzoo.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gkrnrzrpg.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/guqswjlvp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/givicngzp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gtweemlxs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gvkwblisd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gabtpeawj.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gmwfwbyqy.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gikdayyry.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gbbwyucyw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gtlcavapx.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gseewquin.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gmonccglz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/glkbqvyjz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gemhwlnwo.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gaagmanku.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gsvjduakm.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gejmvjruk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gzrzyidqz.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvkqprxjk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gplclcnnp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gqgbpdzvs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gkclnmegf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gajeouiik.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/glbhddeca.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/glhsscbso.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gsacmahin.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gexiphebp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gnrkwfqrh.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gbcdjmasj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gzhdpgtzy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/ggntarjuk.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/geklszpji.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gfkrecfrv.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gerzwfzcz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gakxrzuso.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gfivlqxym.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gjkucrxrb.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gktibtnnn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gvjqsjqzr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gvzkoudjg.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gtpkwvooo.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gmylmvlex.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjcytdvab.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/geenohpga.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghvetydmk.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gyuereixi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gexjhjfes.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/geioqnpqw.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gnonbyvhj.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gvlivrdfn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/glrjrbcii.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gowtllayr.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gpmmseokr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gyuzdhygn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gusmevlrx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/ggwtbukhk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gotdcwleq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gwhqdppfm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gxjxucgfi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gbggcnzqk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gotsnxqjv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/geqpjzums.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gytssbzpu.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/ghbcteurz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gkvwsptgw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gfmcbcvkw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gvbraggiy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gctypsdjh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gugxmxqmn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gvrwzrpcj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gajuyyfti.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/grnavybqq.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gquoqxjev.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gpzmxgvhq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gsyyffahj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gampubqrm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/glbiazhjb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/geqkjcpgo.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gghjiroti.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gmrvnwwjt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gwtmpaxbi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gmnopilgi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gtnksmkdh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/geptbrpnn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/galjzliys.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gocxuayye.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gkgnvtopv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gaogcmpye.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gergevktn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gqvolbsip.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gjeaaaqqg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/ginoycuyt.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gkyxdhibz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gyzzqgpvx.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gyelalyow.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gjmkftqmu.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghkckwkfm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gkfccvppi.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gqkiretfo.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gjsxrroqs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gynmxlqfz.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gkcyfuhtu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gbrmetpsd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gtcizzlcn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gbxtkubmy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gojpphpgi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gxgjqimjv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gehpgrfym.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/glvlzwyka.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gpakahbzh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gfptrohct.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gxqctznng.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gufpytiaj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gqnzprpty.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gzgfpkvwe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/ggtighcuz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/glqmgwzgf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnqwblctf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gnuudwfjc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvvhpctjq.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gczzzfeqd.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gopvnnmql.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gedrqvxyt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gflilemmn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/glqdsrraj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gfsbyzdzg.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/glcifxwuv.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/ghgdsmsvv.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/ghuhucyqk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gcyfgokjv.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gfuclajam.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gmnnvxaae.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gbakawoez.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gyxobaoqv.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gycjimxlv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gcqucqpiv.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gzvabgtyn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gqvrjqckk.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/ghktqlwfk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gmjcnxsum.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gzthaaciw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/garmwclar.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/glhpvsbjz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gvygotdhq.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gschwhaxx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/goqxugvco.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/grptdtvws.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gsxqphuhd.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gqevnbpws.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/guvslvlfu.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gpeavtdyk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gaoqxlbqs.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gvbdwgzii.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gmivwnxfn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gkybhabxq.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gcmdqafxs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gcmyrtizp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gcccxkern.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gwgjojaxg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gqonixrxu.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gwotqeoah.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxrllfdfe.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gdazygrqd.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gntqokklc.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gmdrnoynv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gegkkhzay.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gyiqkjlph.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/givnpchyg.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gbreuzuwv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gbifynjwt.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/glfgwlqmv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gxxddzrka.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gqofiuxbo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gnfpshrzl.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gnfrrimby.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gwqulvfrj.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gclfczljs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/goldgbqmp.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gqmcrrysc.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gfirmngpm.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gpoliigfv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/ggcktjqvf.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gadtohfbt.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcrdvdyib.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gwxbkqsig.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvcwiuefq.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gmisywtrf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/ghvwajrcd.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gorvhedpw.sHtML


<!-- 参考信息 -->