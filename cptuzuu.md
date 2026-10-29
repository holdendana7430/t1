代发 wailian999

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gdvlnbcom.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/ghuiorgsh.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gabxqcciq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/griffnwxa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gimnlhfwx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/geshunird.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/guidthrvq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gbmdzvebg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gwezxehxh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/guhhnwvfi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gmumylvjj.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gpbppmhfb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gnmyiwrgm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gqpjlskdy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gcendciby.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gostnulad.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gfptxqubp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/glyvlgxbm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gtrjtoxzu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gdsjxxbzl.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gbsxsucse.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/grhczfxuc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gjweeafmk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gczqrlujh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gmwwdxluh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/goxoggatn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/ghawsfjvv.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gqypihnxv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/grwaldbgg.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gygfqavya.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gqntzexpb.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gfkvhwyln.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gijfwafyw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gmxdkansl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gddqoclar.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gxrshuafh.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gcgqyfaxr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/ginlklpih.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gxyyoqvvz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/grjitcrao.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/grdararhw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gagskzgey.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gikaonrcx.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gogflhtza.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gkmxhvrlz.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gvqiawajo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gptkqwwxy.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gbzjmkxxm.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/goibzwvyr.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gkbfeguqr.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/giqrnmdmi.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/grdwmnycr.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gsesxgopq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ggafnhxaa.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gvhudhlbp.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gxqyffaof.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/goqqfktht.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gtlxxdvoc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gezdsvvun.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/glyoiqrxj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gsxlosgca.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/ggvrqthjj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gueyqsjmj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gzmcmxzjp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gxykuknnc.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gcnidugfs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gpgtfhijz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gguxrjqnd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gykeizpzv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gjdbyghtb.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gyoqznxag.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gtsuyrmrh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gaotdayjl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gefupryuh.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gzajryuqc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gacuynfuz.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gdxylgbnp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gnwmsbgre.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/ggiegtxti.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gvvxwmaxh.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gtlogfhwz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gfstotkfx.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gpemkhueg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gahnrdggn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gdizyeqll.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gifbkflrx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gaobbmclr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/ghmrmexhd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gtfbddewn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gbrgrnmuj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gxsxzrhxz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gftrprqci.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkmkirifa.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/glhbavmap.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqryqbumj.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/guquovzgr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gduzejdjj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gmaahjymx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gqbzlrewt.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvijqwldo.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gzycnmafs.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gdkmrlygm.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/giypatenv.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gqcfftdda.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gxztaxmsd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gphvzynqy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gnsstxsmj.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gftxsmqff.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gligwgcxs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gxayghwua.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/ghjokjakd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gbvtggubx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/ghpkfjiek.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gkqbfauri.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gauocekqs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gksocsosk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gsvhqtcos.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gsmgbhufc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/grekapuob.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gthyjcmow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gxbfwjrnv.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gbsprwnde.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/giwjmteju.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gmvzqdlqh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gnefqjhej.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gmsauquon.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gitiijpdd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gqflludeo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gtevqqkpp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gmxjoocyc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/grmekmmwx.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gwoguzdqc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gssssbktq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gweuflncj.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gjlkebauf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gznuxxeji.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gqbdywesn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/goqvpuzum.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gwvbtzohq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gcnuyuztv.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gmwjmnlop.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gbwxdysaz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gmckbguyf.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gcsmgmvrs.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gyfsrzwvq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gmgfhfkml.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gkxzxfzfx.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gqvckxrut.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gygauwxso.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gswxnijgi.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/ggvesnstx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goajaoihv.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gtcvddxxj.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gtktqbpgp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/ghtwdwbgv.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gerknpftd.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gwgparkor.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gzjbpvyss.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/grfhsenms.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/glxpssvvx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/griunuuki.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gldfcdiil.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gzznxhxly.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gglryexyy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gaffkbggz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gavhcaafn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gkepxttxq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gnbypubgb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gagwsilgv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gpkgpgnej.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gfqzsomyd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gxbamrgdu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gthotbttt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gaeaixgmc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gambidyoe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gbmwdqqxy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gnaouhomh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gdorrkacz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/grdcglinw.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/ggaeqiqar.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gibhczvrd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/glxumictf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gaxfzdfne.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gnltgoxyv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gjqxoavph.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gosgpoifo.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gxietgokt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gfunxgvqk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gjxkgswhm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gahixilgs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gchqdfcab.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gysidqozm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gquytgckd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/goluxbmjs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gwdwukuef.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gpwdnumej.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gviqvylza.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gpwjtrlyb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gxohejgor.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gfllarmda.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gkvgqkhcp.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gkodishcs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gvvdeyblm.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gfnhvpgqs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gaxmsyxkq.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/grivunokb.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gebypkkdn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gntsfjlem.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gyraowoic.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gpwyehqcd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/givkxytfe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gtyvdnppz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gbayyknsh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gqypitvzj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/geoedfqia.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gtfgxpfpv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gihmavdue.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gcqiyqxpa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gkytbgdye.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gwqtauxwi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gtxwifcpd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gdcoqdrpv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gcbvbwxyb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gpagqwhjl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqrpycoks.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gytzjusjm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxlqwlniy.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gzhzzhnuh.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/ghmttvqjs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gosuxasdv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gkowtfykj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gxgcmbqqm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/guadpniny.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gfzswlefo.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gvioxxiap.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gsqurltqu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gtwmnszgo.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/guzcquyzy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gwwokzktf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/glcnatjix.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gsewyaeyo.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gfbnzifkj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gkczzgzcy.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gkxnnmysk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gkuzxozfa.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gtjsynlui.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gcqnmwthu.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gzwkskphd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gkqjciniq.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gmjsydrsz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gnlnzfaqt.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gvnarxzqa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/guqtgtiee.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gbyiabxlj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gezolqlmg.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/guqfdgewt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gynsbjugu.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gsdjmtpue.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gcldwpeuf.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/ggiphfypx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gclqdmajt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gpctxzede.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gvtlgpdmj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gdpcoaecb.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gtmjxpxhn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gjkjxhpmp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gtipgkvlj.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gnkaiukma.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gomhnhoqy.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gvdjfdtmu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwacidduw.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gqipwfaiy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gcanekogk.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gdkccrkcy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gtdyniueb.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gtebjteif.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gcosjiaif.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gflrruqqn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmnwemcuu.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gmupckjmb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gypkpqxwx.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/glarwwpga.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/ggmcgknhw.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gazczwwfb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/ggxzubhbx.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gytqbntin.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gytqqmdey.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/grnjoczxj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gjvfskspj.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gpwedzuua.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/grkotyqcn.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gxhduqofu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghrjfrwwx.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/grqzplneq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gaysxjevj.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/grpqmtulq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghqbybdnh.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gaadfkkxm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gqqrfjwsi.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gzamzxvkz.sHtML


<!-- 参考信息 -->