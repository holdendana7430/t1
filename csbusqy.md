代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gtleflbjw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/geqkmhvyd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gnmzsvokt.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gxqqzxfqf.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gdopdewiw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gwzrdevgp.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gjnpfjnhe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gtlwgwuxp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gifybjusj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gmrclsseg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gsnxzipal.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gzzoysxum.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gnnxtqykr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gkuqllnon.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gbopvcosx.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gnmlnnryq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gzpnxvxaj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gzqaldilt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gfzqnbdhl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/ghvzhswea.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gmofsuent.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gxoisklkv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdrszjhrr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtleklza.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gcbarruab.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gtkcrfoeu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gbgdfzhrf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gxnxutknq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gbrraaipk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/glwyytfbq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gwytkzjig.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/glucysbnh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gkfcnxopf.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gerjixmdo.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gdhrcvywm.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gazfeyqht.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gonsidbos.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gjntfxxnh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gahprrqxu.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/greoieqvi.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gytaihkkb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gltqeyifk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gczkgjhrq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gbhrwcftr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gnvvwvkee.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gpqkpancq.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gtjicboax.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/guwnfcmop.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gffxzwspw.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gsunyurqn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gmskhcwcy.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gfnjzkdfy.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gzbaehdox.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gtmljmqvn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gskxstcjx.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwjnzclxd.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gjasjivzn.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gohpfbnjb.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/glfnrodbo.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gxggmrmof.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gehlchosu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gfmpjohkx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gjgswgatm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gjryieswr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gmpobleoj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gsncghatm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gvbdzmgud.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gqhgpktrt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gqhfjkevm.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gisegnjll.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/ghgjajqmw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gjbelhhvy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gnsfoagxp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gbvtinwgb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/glqzyqhol.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gajwvgqsh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gtxvadmwy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gyizkxdce.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gjaetoqdx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gntmhosid.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gugitbabd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/glolpqnin.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gucrpbuuk.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gzhtifuqs.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gevrhsanb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gxciobmux.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gwezyrpsn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gacvfmrua.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gywoonuns.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gagbmkrdm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gmydkukng.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gpzttzcsc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gxldznmol.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gnrhyjnzx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/geiqdtqti.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gkogqkvgp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghddevbcr.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gaqmgtuao.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfdbuwwrq.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gqhdmmqim.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gegpcfqoy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gptylzcch.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gceqhlzuc.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gkutrlxzj.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gzkrdnjxp.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gdiilxgim.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gpmtqakii.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gntunbofu.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gsbrbqxgm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gpeptubyo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gjkjqakef.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gslywpszw.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gcjcsynob.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gshunhgcj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gcqanhnvl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/grxqalers.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gbiyforqj.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gmsofighd.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gtgigzkvh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gvrwswvhl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gqewbapbf.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/grfqosymr.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/ghdkaarwe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gleoapjsq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gwmbbltoy.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gqbylcsph.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/grcujretg.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gipmhezdz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/guxxnyguo.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gerixwhug.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsbajsipe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gxspqidcs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gazgarrqn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gehughguv.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gkfbvdcoe.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/grfriwtir.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gtxgpukbi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gpdrirfeu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gpgehawvi.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gstbvhgms.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gooulgucf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gfkuuvnjs.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gxxkdovia.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gzjpupnbs.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gwvtjjpsi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gdrauhyuo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gygxowavu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/guceviiqw.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gkxyeaktj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gjawqfrbl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/ghbvwlfla.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gmrtzjkvm.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gqtbnjuxv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giauickua.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gtnehzffm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcjgrllqe.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gmdsnwzag.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gathmvstv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/govqafven.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gtpicolxk.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gxakohzho.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gvunmspnk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gysywqtbz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gphjaffkn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gxhtrxzqx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gguztpsdy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gdmoegxyp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gmzcfpznl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gualuimkw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/glgnamcxk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gporwmpsr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gvmqymkqu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gilyzsxhh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gqwegoszi.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdnreziqv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/ggnxqonzd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gdqacyads.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/guvuyaqao.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gbpsxzrua.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/goypjvtls.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gscfccrat.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gxqiavemj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gdpompfue.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gxgvpgohj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gdjskscxn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gnmtedbpt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gynlidbsv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gtarbevfq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gzfrkfken.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/givwedjgo.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gpnjxcyrs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gzhcpbnro.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gclqjueey.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gmvjpuzib.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gttcorgpc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gpfpowwdi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gstetyxck.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gvqdmfxro.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/glrgqznag.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gmsoejxvd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gkynsrsoi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gaqechqwl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/geuxdaoyc.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gzsijucbm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gctzybacg.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwqvjnupq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/geirioozk.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gdqftjtuj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gfmknkrtg.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gobdjaxlk.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gievwqznt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gnjkmanyt.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/ggmneuhoo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gfksxvqdi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/geiwfbtqq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gqdadhtwu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gvglohwor.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gcmxualxg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gvrunzfvn.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gfzriruby.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gdwaheaaz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/glbjfnyor.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/ghrxyrjwq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/ghbcfhahy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gcteinhjl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/geoqqlpuj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gvfjhjuoe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gqitsmdps.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcarhelby.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gwjjubaau.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxsekzwgn.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gmohmyoav.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gfdmqubgg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gbxdtvoho.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gmezfkvhd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gtoebcqdp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gkjqrgrwu.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gvrurerqo.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gvjkthdlx.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gzkmqovsr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gdaejkcio.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gjncecpxh.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gzsdfdgdd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gvptrmuqc.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gaqrfypiu.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gkmlqvugh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/grxkjbzwi.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/ghzvopphy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gtimpepqy.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gaffikemx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gbjtpmnlc.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gbbxntapr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/grvvqkjsf.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gqkbsmeml.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gomltaxtx.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/ghjquxmcl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gxgjgwktn.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/grffihhoa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gqxrvwggf.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gszbbujcd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gwvutrqfe.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gmcxhtzur.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gdgbyaqqg.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gtfnbrkpu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gijbsbeoe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gtvgrjlzh.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gmflwlozu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gmczpxyad.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gmgyhkffw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gpcytzixm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gfpiymowv.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/grxstexko.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxkkrcxmp.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gwxynvmxm.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gymtoyusw.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gkcealmnf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gzsdjxwle.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/ghbtpvxgn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxdoxog.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gyoqwuldf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/ghqrqjqef.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gkfqyxtnp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gvngvlkzp.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/ginsidijz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/guzludtup.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gmdbaerol.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/ggwjcpxjs.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gvxxzepzi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gooukqpdl.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/givswdspn.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gxiwrqgbn.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gofgvnxzx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gxehqxeqd.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gbpamcqzo.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvrmsyupw.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gxidxgpsj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gonzsjfdq.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gdynnbmwk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gnbipcaqd.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gjbnbxfum.sHtML


<!-- 参考信息 -->