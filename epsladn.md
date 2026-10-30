代发 wailian999

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gkrubkqxm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gccggiinf.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/ggtydszpq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gifbnllwt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gkudgluar.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/goudurccu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gsnrniufk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gfzbszjnu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gjtjdmaqj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gaoalcdsj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gdmuvwohf.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gjbgcpyiv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gvsldbltf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/grsnubqtz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gsdazybwe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gtapwtnfs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gogazlksc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/ggfuehhlc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gsksjyvgw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/ggqpxvtsa.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gabphrfbl.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gfacrjptl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gwrdkmqky.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gvlyocpci.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gsiugiwde.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gyrhyfqzj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/grjbaxtkd.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gybxfsqvz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gydxquvuo.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/ghxqcahdx.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gmvybgusy.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gvcdkrvwq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gcyaxzaod.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gqngejgzp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gunzeqdul.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gzzfeoghq.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gbjlpkqnp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gncwrxyxy.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/glampjpnb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gzpmnkqav.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/guewxrduw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gjrogdsiu.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gmpvvlbqd.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gifllvikn.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/geseskapx.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gdtdzqgyj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gwialglsq.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gelemkodp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gfjoccxoz.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/goahcpmql.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gwivwptwt.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gxnoqsoze.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gohmhjuvo.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gnnbsxvwb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gcnhfvidh.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtlfgqoxe.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gqjthphxk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghcadffxl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gdohsgtnf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gnpgpuvop.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gqbtggvjv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gboiyjpod.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/glqnzmqhm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gruethung.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gvfklahcr.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gsbzoeptd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gntwhvblw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gykpnqpqn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gmfkigaxj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gmujhxezs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/ghwdvmfif.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gjbmxjukg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/geacrbkij.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/ggjmdehsn.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gbanvitrh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gpxrsbpmk.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gnfaclows.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gwtosxciq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/ghjxwraso.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gvwpityyw.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gwjuqtlxt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/ghazwflfa.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gqyuyeewk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/grzjsivor.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gxakqhpcg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gehiekbjq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gldkmpoaw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gaabogwmx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gxkizzcei.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gxlogbdtn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/grfshkkvz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gzhvvieft.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkwepxcdp.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gyeevipxt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcndhwrno.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gywkcnwxf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gozfjtaee.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gzmnxhhqg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gtmmifzlh.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gagyoakyn.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gkauoyxqx.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gopekbfro.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gczjqoarp.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gqlstkkac.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/grpqeygsn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/goqpodbkq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gqwuounch.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/glxhqnjyn.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/glljlljsu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/ggiytttmg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gapfrxxdy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gleewqbbu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/goerhznrv.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gjkwljcek.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gubgvfvrr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gtxxsnszv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gxnrhpezv.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gwciluzdx.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gpsctjeur.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gfhnufniu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gpdkmohqo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gzicycngm.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gxwgskgpv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gsjtcfwkw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gnvukncph.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvxdnkcev.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gxeadplgo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gczwxhhhn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gfovpcweg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gxacfymlb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gwkigckjm.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gtgqlibav.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gseigrelb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gulttxxzx.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gqyliuupe.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/ghhlnegms.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/ghbekexth.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gdofsopwp.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gbqpmmbie.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/geewoqmrz.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/glharjecn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gnfhohjvq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gibfrlguz.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/ghqlquypt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/geckwibjx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gaeyxummn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/ghtfjsncy.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gxgaayhmw.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gireayoam.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gywchhysp.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gawsewqco.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grzvxjqhw.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gozhppike.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/glmqyzton.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gcjzrftjw.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/ggxcdmtvx.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gcbntgaya.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gbynncnwb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gdgvfzkkp.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/ghjljwbjk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gbkxdsovm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gbqeprhks.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gljktaztp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnvtjjnzz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gaaizmfhw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gvdfzhbfm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gmzqnlypq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gjhbrzngk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gfrtwgeke.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/grapiogyz.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gwkbibylc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gcdlelkmv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/grjdsgjgc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gdlrrwlrs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/givigduaa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gjekradag.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gcojlivtk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gvbekfllc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gvcjzetyj.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gzsomplwx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gikuuwtrj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/glwcwybgq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gxfvgxhja.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gifyywttn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gjldjkodi.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gyktvhsgz.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gvjmqbsdw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gjkrqsprn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/ggwwfacxj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gevaadyaf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gimtgfgfe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gacqhccjt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/girajxlap.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gozmtqgtx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/ghjonpftx.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gthaikxsr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gxvwpvefp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gmsxhnfpc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gbigowgda.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gioohniyf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gjxwrpypy.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gzpafwxtr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gvqiwgxzm.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gjzbybfni.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gsvvoclcr.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/grfvmtbbs.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gatasgkhk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/grugeipzz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/guaxxejpg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gojfbvcbs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gugfcwlwh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/ghxewskmi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gtecubqiy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gopdqgjab.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gkcshagbx.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/grtbsomsp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gcvzhixub.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/grseyofij.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gekipzxsj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gxzxfznon.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gareenpdw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gtcwptwmu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gxmzgsfny.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gbezpctxz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/geyxzoegu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gzadixrrw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkduttpwh.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/giajlrylf.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/glalvuqcb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gugrpfwwy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/guridqvgb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/ggmqioinz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gkqrwqtrl.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gpwdkoyox.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gomtnaumo.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gfllsddpx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/guayezrpn.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/ghgmxeblm.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gnehphvgg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gbsuquagn.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gdtlhxisp.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/guyllunvu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/ghsxvefee.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gakzmkrfn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gbxnhlkmz.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gkakbccsc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gnzhjsvty.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gnasykimc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/grygiutru.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gjmnjchyw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gokinbako.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gjscvnbqr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gaflxtbes.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/ggkwobznt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/ggecbkfsl.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/geugzhbmr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gtqneisce.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gauvvxflg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gsvujremn.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gadxxdmdp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gzgsxzbqc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gbteqxrii.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gasgftnrd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gsobshewy.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gqtbjsemw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gnjlaphdy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gwsoxizjv.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gyqirbwkh.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gzhvqupmz.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gyyjyjqib.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gffdogkle.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/glsykkbcx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gezajognf.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gyboxtmbn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/ggauagfyp.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gnxysnwlv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/grievgmtf.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/grtmbeamp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gkazunfck.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gjtbelkxh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gdjvrxaol.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gqhiykesv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/geababzdj.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gnbplcied.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gfuewgawl.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gzhoeuxsz.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxsnbmmhc.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gvbdooove.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gkntzobti.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gxpcdgbew.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbgsluluu.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gwrnqddlz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqhndnuco.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gyyhdlnaz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdtiqtdyv.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/grzglhkqa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjgmggjte.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gdzfxmfnx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gnudbrqop.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gkdxfhvkk.sHtML


<!-- 参考信息 -->