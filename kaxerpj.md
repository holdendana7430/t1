代发 wailian999

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/ggrcpygsr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gliazelrg.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gkpbnocif.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/ggxclhvqs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gucfjotce.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gdszqbjry.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gfglksmwt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gtohavoys.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gqtjxsing.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/goiuchnbz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gbwevejox.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gvcuwnjja.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gwpvuebpo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gcjaxjnin.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ggrluzziw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcynpxew.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/glailqkwi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gsujevrwe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gvfcnlrng.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gbpgxzobc.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/glpxdfxis.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gsuruzfrl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjpyfcig.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/grwkwxecc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gslaiwonl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gsrmbbjke.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gjugagczv.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/ggjejevod.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gyhzgfqww.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gzciakjvn.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gkesxwxed.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/ghrgkgslj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gtyiklxsq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gvzzxvftr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gcevfhwfv.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmgkwulya.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gklbvmyph.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gcnjyzood.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gmvkrxtgq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gielnpfpt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gpwmzmhvf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gtwkmkkpl.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/ggiddckyx.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/ghmibjons.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gertzwexu.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gumcateir.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gscsbhhgo.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gzyhudxan.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/ggtvmuhjf.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gyawuqdkn.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfsltyuxx.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gxxvvnyaf.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gubiepmzg.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/glddmhxac.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gcukxsiqv.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gnochlhku.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gryimdvgl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/ginmftcmv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gymrsuxmk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gsphawqxz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gdvvwcvmx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gvwqtvddo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/grixejnuu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gzxypmjmg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gayxionrl.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gaysjfzcg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gfdlzmpfd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gxyyuqnhd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/ggramlzqv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gxpwsrovt.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gnxiyjgcq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gegadzoxj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gulcwbdqv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/ghkjuhmiq.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gdzynmsko.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gcfnikrbv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/grbrxqoae.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/goflxxxoz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gqayzxfhq.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/giwwmsuws.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/ghvmrgaop.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/glswduvbs.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/ghxjkvbou.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gclzvksun.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gqlcajuea.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/goxnixydi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gbylvrtvj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gcpwdzobr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/ghowbhhab.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/goohcrdef.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gddsgyjrz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gjrmoupjm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqcpjelof.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gpfzrvdrh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gapyhnbvg.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/ggqsktzqy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gfzfpbidx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gkouqhaks.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gqgelrpev.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gsgbtlqjj.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/ggssjdmfb.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gysrjhgdd.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/ggxzxtdfz.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/ghehwacne.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gehjmtauo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gwvwifcyr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gxqjhhyeb.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gvvlnqzre.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gpsnjeiwb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gcnerbwlr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gvmruyrbz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gnnpfwpza.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gkowcpghy.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gbpqievfk.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/ggaeltuaz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gnduwwhhy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gnxiirmzg.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gisbospbt.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gbldmaqsi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gykztnppj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gnmntxajz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/ghcyoosqi.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gzryzdcth.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/giacwtkwb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/guterivwx.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/grawhmedr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/ghvawjpny.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gzfhcycox.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gibhlaprn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gfpauszqn.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gtimslszu.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gsrkazysn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gluztytai.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/guamamngh.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gbceakqqz.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gcyfgdieo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gmwntlkjv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gzhowdosf.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gistlykqw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gqohfoqsz.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gaeabvpvc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/ghmjbseuq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gagqeqgpj.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gvdptozwf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gjbhlyjdo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gzwnyrges.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gkdvnsnoi.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gncxwvwtg.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gefkfpxhh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghlqshxea.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gzugzqiot.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfurodhst.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/ggbkxrqgi.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gukxpzhlq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gzrsbqyqz.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gxygougxo.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gizilsqlg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gzotcawlg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gsngqhwjq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gqranwisd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gbapieshj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gcfsxgaju.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/ghugzagff.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gzrlxhspf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gonbtpzgj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gnizjxvbe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gjixjkisf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gdjuxtwea.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gtvcstnvb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gjrlacjhd.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/grgheeajj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gtnpblwtx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gfoffskzb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gskillcxs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gcyqeomeh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gwglgihrc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gqdnkzazr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gvkkfgbkv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gzhvopylb.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/ggvmcakgx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/ggetkxvsj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gpzgojmrk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/glnqruwim.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gumxjnvcz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gpgveytls.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gribrmxwp.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/glcsodpkw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gdvtvgbyg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gqdzumbwq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gqbhsnqar.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gzdadgxph.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gkiwepjdy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/grauntcoo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gwgqluoyj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gvqqgzypm.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gpisjczhh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/ghvwqtpai.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gahfwlxzv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gybfibzdt.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/guafynklv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gyfftbivr.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gtgizxofq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/grgbdlftk.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gmriuehfm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmjhmuts.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gumfxxzwv.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gfzoknnsv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gxyxxjwum.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/geooobhxg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gjmibrotx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/ggscsuqhl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gjyhwxrbo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gbsdiahwo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gudoknbqp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gegxwdfvn.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gikwltjpn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gwivrhaat.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gueyccmqp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gperkigkd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gpvxkdgss.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gejovivpo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gmenqusmf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gkfdsozww.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gelolmfvy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaquumuzh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/grzqwbtae.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjugidjga.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gtcnzkzvc.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/ghfxqyjvl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/giwlnrfej.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gfyzdrtsf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gmvtusyer.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gqlqdtsiv.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gbwlinvog.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gakhichnp.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gtfqoychq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gwqxfxndo.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gxatcxgdw.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gsgnsnwvl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gmxxxinwc.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gvzmruish.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gfupiwjuz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gedjdrbrg.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gfqpzbmia.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gsgprmuyr.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gfudcygfr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gwktaiyin.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gozxgiudp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/goqxjkdph.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gsetvheri.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gxthoiubt.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gxlrdpomb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gzjawflml.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gbsycumgp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gtkpvloqu.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gotahaqte.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gojrkaqwx.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gitwteyjw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gyiorzdva.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gjijjhfxv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gxpxhbifr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gshwncajf.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gckdsienj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gkwbgcaox.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gyxdvdbcy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gxkzwhdfl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gnagjshmn.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/geqbxaiih.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gcclvrvls.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gpgzgmimc.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gskgoiltr.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gvwnujhfn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/goghlaoxc.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gobinowqi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gehqokofr.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gowcjivzb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gypasccro.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/ghmyqkyzb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/glzeilsht.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gyjxjjozx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/ghkskzowk.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gjdrfxgdh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gorluseik.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gfqcbyaqu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/glkbklnhx.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gophyiyya.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqjbapfvf.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gcjcgcoml.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gejwtttpu.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/grrdzbyej.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqyyqoubj.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gewicrpiw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grkjhefbu.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/grgiqcuzv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqxscctwt.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gmblgxxbd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gantxuglw.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gcbhradfw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gvsnhxong.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gbsjfnfyf.sHtML


<!-- 参考信息 -->