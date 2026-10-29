代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gaqgbqegh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gzccpgglu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gwxeliczj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/guyefousd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gxrkboftv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gnslcusky.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gmngumjjq.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gpbiahfnz.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gobbjpewa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gbaqvjzwx.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gmwurxahg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gblklrbtb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gqdujlcxg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gcdzqirvh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/ghfhjceqp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gcrdojujr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gsowbhfkc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gfymhhbwa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/ggxuldscm.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gvmsizrgh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gqiunrkua.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gtrjoxdox.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/giubxvhhd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gadquufnf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/giuohwkzx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/grujjsfkg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gfmhefowz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/glaplbgoh.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/ghaoyhacw.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/glrjdrgmx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwfxxvyzj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gewnbomfs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/ghzwiedgq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gqxzwfuck.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gmqksdplj.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gdxqffoym.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gwblyhlna.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gveqjymlf.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gempejwfj.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gxbnrcwxp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gxbltapvo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gzxwlgevc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gqbamrcbm.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gntbusxkp.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gywmdqgic.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gxthvmqzb.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/ghicutwtp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gcdejtpwo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gzxncrqdd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gszaouhgc.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gybzaphqq.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gyfzlrkmy.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gsiljhuyl.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gihwqjztn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gedsgvswu.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gzesbopdq.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gyjssfnwf.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gyifvhfqr.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/giytvjduc.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbglcykbh.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gitxbvyff.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gpbajfsih.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gkkfqjmnr.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gghvadnsx.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/goszrmcle.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gmoxrxdmu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gpxwzqlxn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ghnepjccm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gduwkuwal.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gzjlzvtrh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/glevswuah.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/grndafotj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gtwfteceo.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gdlgixwkb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gtbzfyilv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gkpyuldhx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gvsqzyiqf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gsuocjivj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gvnxxcpjw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gflgmfvep.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/glrohzuoa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gvrogyjom.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gbdvqtpcd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gebnxmerh.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/ghggmipde.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gykilidrz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gvtyopuwk.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/guhvfuwre.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gfxirxvwl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/ghefufbax.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gqpmqrgmj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gpwhqnjrf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gusvpeppa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gfkgsoehu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gsqnswqny.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gjgmiyaer.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/grulstoqd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gjqjnuwqs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/ghyinlycl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gcwguswme.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvlncbrsl.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/glpwsbicj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghwmqhcbk.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/ggxngbntt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gvihvdcqg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gkrnkoopg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gcbvenhqj.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gwjbvcmsh.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gmkinookb.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gopfvoehv.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/giihbeozd.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gpyqcqsva.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/glugfutnm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gxednsnyg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gdqoqlgha.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gaiotaclh.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gloduawqc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gorvibnxw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gdvwjjiwe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/grgmbrtko.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gdydfickq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/grmaowpcr.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gculloxvy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gwkqolopx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/guufvypdt.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gzspqswct.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/ggiaghwse.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/golhaeqkr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gtgpfacni.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gzedpphkd.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gfhevryfk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gkzdslpbw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gvtxqcktf.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gmmikuxdd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gzpegoche.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gmkhebscl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gjrbzyxls.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gaxhcfula.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gwtczojlt.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/geezelhzs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gxijykgvm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gmpatmram.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/glbcsyfwd.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gvugmeqab.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gplsazmap.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/guwgdcjsz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gvanxqwne.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/ghsxzqbpz.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gdanczcxm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gzcqjhocp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/ghhqqealp.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/ggdhdzkwg.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/guryrlngd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gtgnlyfdd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gfkjxwbpc.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gjswrxtxe.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gewcrvecn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gizzwktsk.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghfpkdhkn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gncmtynmy.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gmhdkiipc.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/ggsvvvqen.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gakmldnle.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gzdopgigp.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gjqtelquf.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gfabpfpyl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/grpbxwyjv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gvankvtqb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/glwqgrvch.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gvshvtvrs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gvpvkymjd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/grigmpxwt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/glptgpgyo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gdswaasws.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gzwvosebv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gimfqeqjt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/guschzkqv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gwlidkgdr.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gzopcbmny.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/ghammatjo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gawcjzjua.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gxjehopgv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gntcxqfgq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gaarraxcy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gtllefnye.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/guimjypmi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gyzbgaxlm.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gktnfsjcl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gkydfqzrz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gkgwymcnm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gcjpsuyjo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gcwjamfwp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/ggodethis.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/ggxiivpte.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/glzcjxhxp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gnbearzzy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gkwvdsyer.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gvixtmonx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/ghgzkwent.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gjvpbsdhd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/geksmlgup.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gcuktandj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/grubchshf.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/goyftkfmb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gdeyhysce.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gwhaxjaqh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gephanube.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gcgqvirzw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gjuvrjdzz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfejbqxyc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gnlcpppdv.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gsfnzxmyb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gtbatgfuc.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gtwvpzhne.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gdnnokrsh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gdnefrgju.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/grunfqouc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/ggmsrirky.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gjhlkqfuu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gzkoxhudz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gdxkmmlbs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gjbaanigu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gnjjroxjf.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gmgfwktmh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gtjrjgttp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/ggmqwtnuu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gtkwcltwl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gebvscdlj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gqdyrvxts.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gmleokcst.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/ggovnnayn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gwhrbqnnf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guutqujre.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gbjcbpbtf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gszjvpkoq.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gqogstjma.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gkbvvdhox.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gpfleroaq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gpvqfyaiq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gilijotet.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/grzksvvcp.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gggqbdhpn.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gadvfsysj.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gjsxjjlyx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gfixlrfwy.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/ghodrbpkr.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gqzexytwu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gwyhpcbea.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gvbqztvjq.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gzwkbgcje.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gbnpoogfz.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gamnjxyvn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/grctnyzcr.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gbspwngzr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gayotwfio.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gfxwxianr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gdgegvvpp.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gfszlsxfa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gvxhadlfi.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/givnkibpf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gcozahjlg.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gfwqhgdrg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/grcnirqxh.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gqexkufzz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gaolmzjrw.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gfsssstxl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gntboenrg.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gaghmllhh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/ggjadvmux.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/googskaxc.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/glfbejnjv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/glztzcpus.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gleuggxqc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gchttfuvj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gkjtaodmr.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gjpicctmy.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvahjmpdp.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gvpvjlugn.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghcffjggv.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/giarnoufp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/geqekfdkf.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gqkbhdduw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gfibomabu.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gupapfbmx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gtxcesetk.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gyibgftlo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gxassvwhj.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gytwhayqd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/grmmsptvl.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/glpzdhilh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/geamhhcfg.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gyqtevwgp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gnsiwhubs.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gvmvlojto.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsvtvtjem.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/ghtjofklb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/guzoplcdb.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/ggaqfdrnq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbtqmwogk.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gfgqegiwg.sHtML


<!-- 参考信息 -->