代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gtbajiflm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gekgftckp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gxnfiydrj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gimuladxi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gjpawixqd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gnqbjmvvd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gjgrajmpf.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwzubessx.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gcjsnghcx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gczybuqra.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gooyyeekk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gvwtbpdpf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gqbegyxug.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/ggqxcqkwz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/guceoyelv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gddtmybpp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gtuqqgavf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gjlgghskp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gzdfyobxw.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gwmzewhig.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gakmzviyo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/glsobhelp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gavemsfoi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gqyjytatu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gtvujocrn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gedgjnqnr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gtzotgsee.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ggfanmlsd.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/geyjjokdb.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gicfjpxpu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gkqhztdxv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gfnwyxzii.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gcolayolz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gwpositeg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gsbpzkdfz.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gixlourdx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gqcuzwvot.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/grdbaitah.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gjhlbrytw.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gunxgeqax.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gtjukzdzm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gnpwzhuum.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gfkrkaelj.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gpvvbkbnt.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gcwayjhjl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gmvrmxqrd.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gzeniwtdx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gypfzgbpi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/glovmdlrb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gdvlxdjye.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gizdgyduz.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gpukcekkg.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gouqcpreq.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/guuedjaxy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/geaaewztq.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gfvvlhdba.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkbfzjgwl.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gwqbzzzpe.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmkdgakfc.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gcghhskbz.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gbxovtuhh.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gamwugsjz.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gajpjyojo.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gwufcmyvm.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gpagtbhbn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gypwkfcvw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gddjfupqw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/glfeejjwj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gekzgligr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gzmrsxbfi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gmjvybsva.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gsflyhuqt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gmtlbpjst.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gqbwhhiot.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gvtbzhwzp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gmlwiblrr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gaplfyzyd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/ggxhqrulv.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gtnbrbvqx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/guepxwrig.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gprxaaauo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gwhuudung.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/goylsefkq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/giuxnirow.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gdhbkmdfd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/grjufxvhw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/grebqzmqe.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/ghqhzyeip.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/goollbfrg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gqxuucrjk.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gminisgqe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gckdthghr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gpkabwrzn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gcdhejcvu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/grzpgbocy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gpsiogdfa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gmuqbfoqf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gcnmtrxhw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gyckezdhf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gmznveknb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghivwhzbp.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gvbhmyzpu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwjwnfuar.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/grobodbgt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gtwnplowi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gbyhxyldr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gawbbkdxj.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gjbottqvo.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gzmjpuzsk.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gqvrzijbi.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gicghatwm.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/ghkebvtmp.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gsslduegi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gvasditjp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gcfutaimd.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/grkriwtry.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gjuqegpqa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gjkkulsjs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gdgehdvmm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/ggdvxqnmm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gsvfydife.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gfijwjnqx.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gldwiylle.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/guvupssji.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gxllsfydu.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gsqucjtbx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gwzshkqqf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gceikvhsx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gmylnyvah.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gxcpytdea.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/guizgzxko.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gfdbqlqiv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gpcfuaimt.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gladwpacc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gzvhvictk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gixhyrdhv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gkiikmobz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gwlkyzfdu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkgljowdc.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gbzyxufbh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gjxjzgmhl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gzcgmpuwn.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gfpyefbym.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gfoukdcxn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gonsgizrz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gekuorsww.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/giewakttu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/ghziwcnpw.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gxuzbonxq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gudzgmjvl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gogztbaqv.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gqbzasygm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/glezxzzke.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gavmhhdwo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/glqitrkwe.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gwhaaxtya.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gvkjqnbtg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjmmghpsx.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/ghbnqtcgi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfctguhqb.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/ghhcqeipm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gvusvsxym.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gpsnnxauq.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gchwpmbrq.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gjtejcrvg.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/ghnnbsvlu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gnwdwuqkr.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/goapafzvw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gnsspvgbq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/grfonuvlc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gpjckitpe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gmulwvese.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gyqcnatcr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gxaocrpos.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gvnyzxtuf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gseqvmmdp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gpegqrxvw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gpsesiciu.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gqemqvbyu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gkdrejpvu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gnjnjeqjq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gbsvwpcro.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gynidnkyo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gcvchbmpk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/guwndmhkx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gjkzlhnuk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gdyhxlecm.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gvcpyvaaf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gzruxjljw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gwhfxorlb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gfsehtxhu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gicmhdixr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gnxazmuah.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gcnawcogs.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gjdaxxoee.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gnongoeiy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gbalvivwd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gaczckrzy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gjvynorco.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/goommgyce.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gaslguetq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gvymvtukd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gzceksddx.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/ggoxnsbkz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gmnyfdrtq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gbkxkynyx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gfuwijgoi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gzbkhrsnu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gtdgwnqix.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/ggitigwrq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gsxdtehye.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gvdtqlfwo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gsjfbkdrk.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gghhuvmkv.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gskjylxnu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gmfelqgkp.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gagelshtz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gozcavcin.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/goowhgwpw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gwesanotf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gvykowqdc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/glcuqbswy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gkzucmisc.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gkfgkgpok.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gugfojnho.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gehguzpby.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gwwowqnbh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/ggaqjkhvw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gyjpyjclx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/ggbcqhlgn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gtglvcvwu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gfykftofa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpxinrgul.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gieauwgby.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmalmjmwj.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/goftoukrj.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/ghhhkplxq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gyrumofqu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/ganeoxvvl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/ghyamnhrg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gwnerkgke.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/ghgvwefyi.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/geegiuybr.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gfwqksqkd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gffyfagbq.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gqxgtrhiy.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/grpqfoxiu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gsninnegn.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/guvevgpbc.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gagtbnmhx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gjchpjboo.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gsoriuxvb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/grxukawog.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gyrurpuuk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/giyqkvjsu.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gmpelocpc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gorqjzncg.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/geturnadx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gpvvomclk.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gslgimkeq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gsqfupybl.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/glflbjgfs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gakgzozod.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gdnmfvldx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gguudtsdr.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gptrbfoqo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gouofkgud.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gowxfndhg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/grqmqsidr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gopfpzkqw.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gcvjgrmzq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gifoklyyi.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gqkpenngt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gfyorpdvl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gzhduemup.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gefrlrkzo.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gioqfnakr.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gumxgevkx.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gzrmxozti.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gsdseenvc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/guiavwcwb.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gymbspvdo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gastdnbxg.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gfzxsfxae.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gecmzjgim.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gdzatagzg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gaxuwofxf.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gqwtpcwhf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gtvwpclkn.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gzpwaclvq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/grwpjrisw.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gbrlzalch.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gxfmzujfh.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gmiuxzala.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/goygzhbae.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gljgxsyds.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/ghctapere.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gasozssho.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxhxxlsnr.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gsaifflxk.sHtML


<!-- 参考信息 -->