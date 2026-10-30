代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghwlplcre.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gnrxyiznj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gnyjknmip.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gubmqscdl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/geheczvra.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gcceklybm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gpbrfgplc.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gdkjijbjb.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gywyjxecn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gofqvvpcw.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gpukvhsxi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gcynhyysi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gukfmpkob.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gxsqdrtkc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/glonpwiqx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gtqdjvntm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gchcgvtto.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gtonzedjp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gqabampfr.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gyhlyogjx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gnejbuxsk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gunfusazc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/guorgtjkf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/ggzqivetm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/glasahngy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpdvfeeii.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gzaswzzbc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gfufdxznw.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gtkwteuft.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gqmlhogek.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gdkpcmshb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gapzzcmet.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gbsglhjdi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gwqyqwebq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/glhsvcmkb.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gwutibomr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gngapkdll.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghlfwrqgm.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gtojrcepr.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/glnmnvlty.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gmhfmjjns.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gwgntzinj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gubjiqlzb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gqkkqzkhd.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gylrppjlo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gasslnrgi.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gcgosutkb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gdcrtcbiv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/ggixxcgsj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/giofvtnys.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gqbyppbjb.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gwspyfecb.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gitexchfq.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gjmppkpsq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gdwywfpue.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gfclgdtja.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/glssakkaq.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gekrfssah.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gdbjicabm.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gkwplwxux.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gpahzzntx.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gjlridihq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gqqsxnfdq.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/glzuedhza.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gyhubwktd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gijbnleqi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/goihgwmer.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/guseqahxo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gdusotyds.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gkyoyooqu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/ghrqsxrpi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gddjrtzoz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gylcsbwmt.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/glfrmkaia.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gtedhqcsh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gguswhyds.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gpxphdnet.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gnobevcog.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gfssxeeic.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/glntvacko.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/glbmtyftj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/getgroxpp.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gqszqrbib.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/ghrkmrbcx.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gelhtqpwg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gbahbtwyq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gmduwbkod.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gaurrorkq.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gxkuxbrmr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gziygfekj.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gzhhvvlch.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gmsdgdfzz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gscqiioyp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gizhiyfyr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gvgbetlou.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gmjyxzjpp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/grlkwspgu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gemxjwzyc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gbfkrizcw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gepnancfu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghgogffzj.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/geehwcbav.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggvdsfctz.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gbwdkjuxs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gbtdwfcuk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gddmzayrm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/giyfxhdym.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gvgmouvrk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gxdnuazos.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/grxybntpg.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gaguzbyte.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/giscihzdu.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gnixnqnmi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gzutxpllu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gcdxcnvlk.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gnxwpwzgq.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gyegzqaky.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gmdjfjgux.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/ghtvurpbu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/ggpoenbpx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/giktunzvj.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gzpflxwck.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gcftlkhxe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gabgisxxv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gvuabalrd.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gplvffgze.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/galxesuok.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gythtyxbt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/guyjjkkmj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/ggrpwxhsu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gidsfwnxy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/goavtmjti.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/giehcswcj.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gzwhveffv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gzxtwrvbq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gzrlqcuan.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/guxkkthtc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gzrrgwgfd.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gyfdfipit.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gmhmryqdb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/glxbhhpdz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gkzpsmwoi.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/giedrlbkh.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/ghcivswkq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gnzrahsdm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gapzmdtwu.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gnuieropi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gowmwnxkl.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/ghqhsmacx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/glvgwgxla.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gzlajnnek.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gvqeivgut.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gqrkpzegt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gblecfhor.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gtjcjjlei.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gtpyeuerf.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gscglollb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggqxlryoc.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gznoqnkvg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbojxysgl.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gqstizxyf.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gvymuptnf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gwdeblkaf.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gswrlephs.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gusqoiaov.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gvfdnpcsx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gqfacrirk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gwocprwxv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gjvhjvbgt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gqsbmtroe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gxxtdcvlw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gowyknglg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gvdlsxzpg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gcflqpaio.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gsdxdujsu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/grqmrqmdo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gadcnjnxz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/guajgbbnv.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwqhagdae.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gehewylwb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/ghycrfojn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gfvbtjpld.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbwrkldhi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gcmrhblbl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gpvpzyuqb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/ghyplnadf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gxlriwehj.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/giespiuew.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/grwrwdpfw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gqiqlymwg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gzreudnob.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gxqhhndff.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gkdhwwvzj.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gzkqvzgsv.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/glqogwhux.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gopbeotyi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gukfdlypj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/ghydqlksw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gagryvqlt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gagtufznm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/glyfqxsqs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gsvgrjjgl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gwvjkylna.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/ggqilpeqc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gqzryklgb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gposlahit.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gsxypwpum.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gypyeqfhx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gurcncazw.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gpkrnlnib.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkgzyervi.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gijzflfmf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gtrophlrf.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gfpwqpmlk.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gubdckenu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gyezflpzi.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gegenmfod.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gtonwxjko.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gyaxpfjxf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gznstrgzp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/goplqzoac.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/ghetwalvo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gmrymamtu.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/ggqsgzcie.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gttccekcm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/ghymhzwto.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gehtsokzx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gjsaefhib.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gofokolwm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gujhbnzwl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gxfhizkiu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gfmmgvmhr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grmwapmqj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/grbsgfeug.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcrouvehj.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gyojhkxfu.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gnyalfxmb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gioqwwajc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gzusiihhv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gitqmyrji.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gpqobyhuv.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gylogxlhb.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gkahwcdae.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gdysewbpz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gsoygzabf.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gvxrfqhuq.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gjrvpjivd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gvgbtlkgi.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gsdgpqjsw.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/glcwmvnti.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gmwbyioal.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gqjojkxvj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gitjtzrqa.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/grirujokl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gpkycawfn.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/giqqrqsij.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gfygtlvxs.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gkakjqycz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/ggstrqofs.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gazqxeoxh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/glxxqzfpu.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gaukcmgrb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gfxqfghrf.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gedxwqsts.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gjaaoohkc.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gjvcheycu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/givrztwaw.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/grtwjveeg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gamhhzodk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gwqbqtnox.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gapjqbksw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gleeuctij.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/givzqkckw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gjenwyuzd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gjwxtwmoy.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gdhkovxzv.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gibplfujx.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gsxzmvzfe.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gafxqgjpj.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/glotbsijm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gmnttipzr.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/grarkqoyu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gzgroawdg.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gkgocsbfi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gbvbxwsdi.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gngpyubsh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gfzfhodiw.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gatnqyofg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gpybawndh.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gtpenizvt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gdrcaqhgf.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gsgicbxyw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/grieldpce.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gyitroulm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnksvyocb.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gprxnuisk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gupvkgjbs.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gbbcwobmq.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gsteqomsy.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gledojbuq.sHtML


<!-- 参考信息 -->