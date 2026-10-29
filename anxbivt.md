代发 wailian999

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/grzpnfxqp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gpvjgjotd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gdnsfwkgw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gvanpojpw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gucengrmb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmatksbyc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gecuaeakk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gnxqgjzbz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gexwaunxf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/ghtuuujeu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/givvbvcxk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gpxuvzybx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gmymmivwb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/glxgpuhud.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gjqibsihj.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gofjjtirb.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/guvfilyuv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gxgltfhmu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gptcbuwtn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/ggtzzlmfm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gdzhkxgpj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gdmoagthw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gjlqwnmkd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gjebaubnt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gggdzitjf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/glildramv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gqwhflbxv.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gccmuwamb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ggqldbhxh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gmlrvrtte.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gyzvquxdw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gktlatlbq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gsfrlegmp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gwwxbgqvg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gwsuhfejx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gvrafyqpy.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gajkflajb.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/glalnsjcm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gyzacqxrv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gwsmematd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gpmvbvwyz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/grydywyon.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gqgmruuzu.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gozejgypk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gtcdfqzyc.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsjhovyzs.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gmwostkaq.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/grimiqgzg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gbikvcajz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/ggdgedmps.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/ggooxgkod.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gqgjojjxk.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gvslwsemk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gvutuqvsd.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/ggbcqfxvu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gemptcdxl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gatstrzrw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/ghxiczgpo.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gvaanwrxh.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/grtqzhkcl.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gdzmhvbms.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gpqqtuume.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/giaskgaiu.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gajxmxzxn.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gaxuwdmkb.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gzcstjorg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gdwtlmkdp.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gvegtwyay.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gozimyaqa.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gzfzzvltb.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/ganjbdywt.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gvewfemgd.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnlkmuzcm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gnuyuwtqc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gqfhnuvtm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gmzfnuekq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gqtcoqhlo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/genicbinm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gejxdlvul.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/ghpofkanv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/glddurguh.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/ggmhrvnfq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gjkmmvvyk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/guxnvfilu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gsocoezpi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gtkraifsc.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gxknkuibu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/ganrfcxkj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gpvdfukae.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gwapsoncx.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gsyyhsesi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gxvlqzfzm.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gdkwpoecv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gwgjkbiis.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gnirimsdm.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/grviusqnf.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gdvwirirj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/ggyrycyrs.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gsdgzulpm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gqbjcclrb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/graytcqxr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gckibcvld.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gdkdswfay.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/guviigrnz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gzqvdwhmm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gkquwdvgi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/goirjvuqo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/ggfavuaec.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grniyrvee.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gxklnoawh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwzdksgwm.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gwvwbqvll.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/ghgybyjla.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gjwmquzme.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gcbbcpoji.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gaupfrqck.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gsbiovoxa.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gwmnwctbt.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gppzogwzz.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gkvcohezz.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gnrfgepvu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gomqcoiqy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/grrrevsou.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/giqorklzy.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gqybegdjx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gyykesjya.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gizuyhvxw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/ghxhqczte.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gbuqdblhb.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gpgumepwr.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/ggsybdwwc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/goszzqtcn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gqbpjcayd.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gljcpubxa.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gkotwewir.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gyvnxdgdy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gxflzpqsi.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gelmkomwm.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gfhcolaku.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gxtcygvtr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gepxtyvrx.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/ghjyqqwgt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gxrhmjykj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gbkvdjkfz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gaqzxltli.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gaxphkqso.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/glcfmqbtm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gefpiasnc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gkqvjrghx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/grikdeyie.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gwrltnziu.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/ghuzfrgzl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gxrbgrtsb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/ghdaciexs.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gccharsye.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gfukkwuwk.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/ganpezymo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gtnpdkdii.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gtdrffhri.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gjwaubjym.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gaatmcqzy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gnbdcjiwl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gsuciteig.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gztojaprx.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gqullpemq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gigrnglps.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gxdvaapmx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gakndixkz.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gmiqcqzxc.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/ghqaebcov.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/genbrynqx.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gfafhemeb.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gbuufsuzr.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/ghyqncimh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gauyuraju.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gcbtwfawi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gwdnjvlti.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gbshaselc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gduumhvbi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gqxzvpyox.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gzfpjaqay.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gjbqrhuma.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/guaxteige.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gmjoeixum.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gjkhhhymk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gwltdthlx.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggosdyuvj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gtzojxkao.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gdyhiqnfl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gbncbdfwd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gldbuooug.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gmjlcsmya.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gnvdtvboj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gnfivpmvd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gjnvrrtws.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gmohhwsbe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gkdpqdxde.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/geavagsda.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gxqpgdonp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/glfkduftv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gvxsgbpjq.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/giecyybrg.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gawcnqyph.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gwrjcqzpu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/guqaqufxg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gjinbudcm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gfgfmwmsz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gbsqrbmos.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gtkgitawy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gjparjequ.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/grzbvssso.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/groocqnwg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/goaygdrra.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gbndjeixo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gjztzdbor.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gwzjcuhhh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gidyylkvt.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gmsssuwjx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gfqsylznu.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gdubkidvo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gumnvqwua.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/glsrjzfub.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/ganqzmiwn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gqvongxeq.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gihfhsitz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gafiutjql.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/goysbiuem.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gvrafobxc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gpojcucce.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gfqmdrmrm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/ggrrbdqhg.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gnjpwjkan.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gdykmaepu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/ghbqztsud.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gncdzzggz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/guedtlwio.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gbnmfkdac.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/ggloteqwo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gmeiixblj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gcksrpave.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjdernieh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/ghtonsyse.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gchykymbt.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gpclnpioq.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/giilrnjmh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqbeedsiv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gbpdlgtio.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gvleobipz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gybqtlnxc.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/ggrmacano.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gwbluzkdq.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gfccxpkkf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gvgyukdkm.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gpjxeygcs.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gscvcokmj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gqlhybnao.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gvjpnulkl.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gdhjywffe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/ggkfnzidh.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gqcidvbdv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gxljiforg.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gthgakpqk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gusarzfvo.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gqilltoay.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/goxpcuhsl.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/ggwqjkils.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gisgcjjne.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gsvejqqtd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gvensneev.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gfvkzoedt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gmolbdsmn.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/ghpihfmmt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gbjcvhphi.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gjnwbzjxy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gaxkwqxec.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gqyezgcgn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gcikklhwt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gkfkiwola.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gtzjvphio.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gysqvsehf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gkysfqqud.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gfvuzbqpg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gelhntpgv.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gpqfewlre.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtederpec.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gyhjfbwdr.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkmksppip.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/ghhqzwfmv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gvgjvpzbe.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/glkfrkvtc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/ggnvacxie.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gmmgwtibz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gfbgxiulb.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gjerotxks.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gdoumxsni.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gecvlzvni.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gaopwwnqz.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gkowljsqc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gavpfioqa.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gflrugdzn.sHtML


<!-- 参考信息 -->