代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gqujdkwom.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gkkerjynd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gcegoedub.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gtifhirvj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gxsyxzrvj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gabpecitp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gvmrpbvia.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gajtxrfyr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwssiotqr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/goycsxxof.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gqvrvhooy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpaaphzmu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gcmuvhmpd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gntearsbp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gfdtctezs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gozwlygmy.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gioshkcwi.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gmmmoymlc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/ggbbjxmgk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gkyaqxrjz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/ggwlmkqlh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gqlgugmim.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/glogwlybw.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/giglvexoj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gvcoovfbw.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gmrxduaam.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gjtrgagix.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gknyjhdcs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ggqzktdsl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gtlfmmnrx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/ggtckytqu.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gjohbwrib.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/grysuffwb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gzhxouocv.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gogiqdwxs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gscqpvrwk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gtplagitj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gpdmiqmzc.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gbmfpcwfp.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gzlbgujli.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gkvzxavxi.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gufgbnipn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gqpcwwxvq.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gdtnensko.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdxffwcwa.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gbaofuxfw.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gwywjaepb.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/glmwgkezj.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gcchdtrof.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/ghzpgwlwe.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gadabxoyv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/grxexkyrx.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gamoybvtu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gkcyvxgxn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/godcgawjl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/glnsnkzoj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gidvqcime.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gxzhfjygf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gthcmukri.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gzwabocks.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gyqvmhnoc.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gfkhyablo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gsnowxoyp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gkakfggcl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gfkwjdsjt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/guvfmpsgq.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gldppcial.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gpkwjeopx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gmmfspvbg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/glxneaawb.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gjbhvjsdg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gjquejmqm.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gtaeicnbd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gmpfytlxe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gstogykuy.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gyehmvakc.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/glrxwontn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gevujpedc.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gpareyfat.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gxaayrnbr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gpomwiknx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/ghjxhqoen.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gmuxywaip.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gnfxagjnh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gbfheojqe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/glmksyuqc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gvnfazjpb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gclawmhfr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfgatqjuh.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gkzawdalg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guquojang.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gybetnpql.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/govlxtljw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gjzscjzwi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gdojuafde.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gmchxvyqq.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gzlptmwwp.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/ghmlthfci.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gwyubkodm.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gplyppvof.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gccbrkyve.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gmlnlarlv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gomxjpvhj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gnebpypnu.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gvywwdtzc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gribaeirz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gdpnmamwc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gaayupoxg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gciireapb.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gxpydhbsy.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gynitkjys.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gesydzkrn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gmmixkedf.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gbqwluxav.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gdpuxvmms.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/glueonmve.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gkenusndy.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gdeikjxyf.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gdqguubpu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gbvbrmhgc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gjiomgelh.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/ggsxbiexj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gnzoumctf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gtcjxgmvo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gnlksqvpc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gmflojuej.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gqpwdpnxh.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gailvsuzj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/ghtvwuhpd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/genvlnmzd.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/guxjerpne.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gqkqwzzwj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gwrvdmwmk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gkfyauaww.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gsuzcsyoo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gzkymwwbq.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gyfxiszxb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gakrxewfd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/ggcereozy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/ggzjfdabo.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gunfnkbmc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gxrctotni.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gymkqivci.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gkhankkbv.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gofekdaux.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvkfnzope.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gazbjcprw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gobnkoqih.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/givffryrv.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gtvinumry.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/ghnijeipk.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gwxvalljx.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gplkuwfpf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gjktkaxyq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gutysttdk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gdapbuzzk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gdjgvzwgi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gusdpdkjj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gwnmyqher.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/grymbcqgk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/ghwtdhfpf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gdjqnvuzn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gxvwgmkij.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gzswjbphq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gcfazajwv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gfweayzeq.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gainwbkig.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gclwovxqc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gftpdmins.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gpnbcolvi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gsmauepum.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gjroogvao.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gbaiixghy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gedymsrsh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gezqbaavq.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gwrulmayd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/guzuksavh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gjsidllhu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gfrtayfll.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gqcdrcecw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gnjxjyxvr.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gstkwjpbj.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gcrgopqey.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gpuwvfrkm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gymfismkg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gmpratdgv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gznhyfutb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gtpxjvfrh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gsmitvksq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gkgqnttuq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gxkyfosst.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gttefddnu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gbxqhhuwb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/glvvoddev.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gjezcwarz.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gyxhupxww.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gxzgeapcb.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/guiiumroc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gfncukxgb.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/girbookhb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gnyihihbx.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/godnqepjc.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gbddhejql.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gbmesohvr.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/ggwfhjbac.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/geqimfsfk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gjfqixnzv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/ggyvjywen.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/ghplajsoj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gqhrlmtnc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gsepzljvr.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/ghzafcxkj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gfcjgahen.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gtjqrxerz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gfsqtbywl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gwixyvfli.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gmcvwpbac.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/grjmtabgc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gfqpoteqo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/grhhofndl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gljcuwjjn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gposozscf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjkgkodef.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gaavhdbup.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gwbovvuhr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gkpxwonkw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ghtguamqt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gjvqgdvxb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gpmmzqhjv.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gnmkivbrf.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gduubvhtb.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gvuvsdlbj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gjdhvtghq.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gjtlqpeju.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gevmffvrg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gtrxmzhrs.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gxhxpquvh.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gvhxcnmfh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gelrcfdrm.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqlcjbfhx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gnpypftju.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gdfwmaxms.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gpprymbxi.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gpesenndq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gcqfgiwko.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gefugnevm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gtgxcyeip.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gavhandxj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gmpgsnlws.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gbfjefxsj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gathmdegi.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gnwmncnwa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gpvgnsbrr.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/ggrkfzfwl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/goqpcnams.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gmybdpkxk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gjwhxshit.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/godboktbz.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/guttyijko.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gknyjhawi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gpznkhwht.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/glpkmuzde.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/givzwudet.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gfpfnorix.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/goadlnonb.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gyhkxbeql.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbflavljq.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gtnuvufyo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gmuizuoxa.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gpeicmwcg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gviftvfjw.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/grkqccksi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gnwjvwhbe.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gxcrclwib.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/grqdszhmg.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gmhezspde.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gyphyiuxu.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gobmqdono.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/glccydxzn.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gemynxstq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gtvtdwukc.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/golzfqrpp.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gberakegp.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gkulwzjuh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gxwtilfwb.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gvrleakac.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gadynvpgl.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gzyitvaqx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/glkgtabsn.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gxokskyfw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gnctywyif.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gijllfmjg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gqykglnoe.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gtvsfykzh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/glqrwjlpm.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/geohpqxxo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gkasgzakr.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gymoxvcky.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gugtbovdm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gifpykmke.sHtML


<!-- 参考信息 -->