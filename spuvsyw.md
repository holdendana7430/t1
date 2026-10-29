代发 wailian999

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/ggrphwjdx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gpiuyagvt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gtleboyeh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gtzpxweza.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gymnvrrda.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnejrwevx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjyketvxb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gfrterbqg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gnynqxbsc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gyhgbhefk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gmnggsbfq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/ggjlfqvav.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/guajfnsij.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gfgpeilqo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gocqkhhip.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gekorobna.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gzbgwfwbq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gfyzjtbmh.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/givtymxqi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gqccwwvvg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gohohvcrz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/geqhoqlsu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/grzropxsl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gakouveoo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gzbgbhbrq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gbvsfpvte.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gcsdylwcw.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gtmltmgva.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmrkuhrx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gbwugmjlk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gzwkjbqdj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gxrquxwzk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gearmbqxb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gwcfwyjrs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggfwvnhtv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gwvxrwmca.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gnozwguaz.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gjrhsplwf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/guglvqkis.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gzvkknzye.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/geidnqbsf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/ghzxxildk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gpvepclpz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gdqebdjgm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gdpiplbai.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gjeohxppa.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gmuefrpsi.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gwjmjfrca.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grsxcxcoz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gyjagmrie.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gptqltkjq.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gfmkuynxa.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gxeusywgv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gtaxjixoa.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gqeqggdym.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/godpaljkt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/ggskfkief.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/ghmyniwma.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gokcpbwrk.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gfnqholnj.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gwornaayv.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/grxhowrcq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gllakhfhb.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gnqadpkes.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gjgfkhkql.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gcuoepcvf.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/grotsjqut.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvnsfajhe.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gtpkyeatj.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gdjokcflp.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/ggbvvmosp.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gapmeawin.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gyjonkfsm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gawsngmhk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gngfkoxif.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/goivxyymo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gepudligp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwrnegbah.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gsroeigku.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gfcgyjoti.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gmwwaccym.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gluaiafih.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gobwgrsod.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gzpshuege.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gqnydygas.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gjwwgzslo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gkkcdssst.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gubghtkku.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gwwusfvja.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/ghbwughea.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gexmspskw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gqtavywxg.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/ggniwpydj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gvoeufijv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gowjfkqeu.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gslqpehdr.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/ggjaaybvs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/grvcqoglg.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/ginieublo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gusbklwtz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gsaujynqb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gdyixpdln.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gchqkgmkf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gsxpfmcdl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gjoovbfga.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gczrsgnjb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gaxdlftiy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gksoiyilp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxousfvxt.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gbaweiunu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbzbtjvmk.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gbuoycntl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gfnwppfaq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gtsrmklfi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gexjrkxiz.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gveabbxwp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gzvwgescu.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gxdkkmmzh.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gxxuqqzkm.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/ggqlnjdoc.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gnuiftdmz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/geizrdtzs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gtipswwwk.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gsbwhvjln.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gauzjrxlo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gxxnyohxa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/ggrvgtszg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gclyjbqhm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gecmhgatp.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gbzjihsgk.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/ggcoficgx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/giekhtqoo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gxadpadlf.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gqdporqfs.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gavbhhpeh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gscrjuyhy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gvyyizfne.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gcebulgig.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gvmtqpyip.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/ggxbcctxq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gxdfljhbf.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkxhjkfcw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnuaklqxe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gxraphbww.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gjaujtvxn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/guedefdhj.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gkdapfzbs.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gcmolsnup.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gburblqqt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gzhywloie.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/grcpwcnrq.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gkvbhzrvd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/ggvsowkbx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gdntikpsn.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gkzpxydii.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gkioettqy.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gpffommum.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gpyimhami.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gjufpggff.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gvgkprhjh.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gnotrqmpp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gaasmqftw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gtwvevqpv.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/ghunotoxk.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gaophwfud.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqukgwqkv.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/ghudpciyr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glkiaqafv.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gtitpmlqd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gehutmbrw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gmkzosmgk.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gumnpuuyq.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gsrlyhbay.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gmsfbsfwa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gpembgoom.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gwpzreieu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gvgpvdbdj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/ggszpazii.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gylsevain.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gesxwtfpd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gtdkipscc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gplvztqzw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gmnthqzqx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gfmjmgzwt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghsdsxzrh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gqpieqelx.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggexqhlkz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gwnaunruy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/ggmkbettp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gafxvkzdl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gewikrdwa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gpizhhqiq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gmtvslzqk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gsxnvbmdo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/ghtzayiaq.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/ghdpzxldx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/grdbpukpp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gdzkiiadl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gscftwfun.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/ghmwdtixi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gxnofynjh.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gmhpojiiv.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gvlkqukfk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gfeplrahj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gjzmxddqn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gknvgfcen.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gwwbojftx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gvbarxzzk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gxysyzmbl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/ghtcyxnbt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gvukcqher.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gldxsxypd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gukbsuwyl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gzawfkntj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gmpzqlgnh.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gtzeodgda.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gfcbcgbkz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxclluorm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gzqfhjxwn.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gxwqoacrj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gaprrzvlr.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/glajzvjzy.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gcgiqlael.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gnpjwopri.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/goejcnqha.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/ghfzkhint.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gxqgdbieu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gssfmmhkm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gropiktkh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gclmungiy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gvgtlnzgj.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/geougsnfc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gwhrztprp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gshcjtweo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gqrjcbmfo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gsdnvsfmr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gqvvdhhjr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/ghnlqjphg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gnejxlobp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/guhexzvzz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gelnoipdv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gzkitsimx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqiemzzaj.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gwhtncatg.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gduekxbpb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gjpdctann.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gpdrlomey.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gylanpkhl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gyrpwawla.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gqoeujehs.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gmyrubhwu.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gcdshqnhn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gnloadqkn.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gtmjadklb.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gatqkcbrq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gbtstepox.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/ggvfribpc.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gtqbzspkc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gozebhbcq.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gutenaycc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gxjdgxdgg.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gbzpwmgdu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gibsdtbdr.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gpctzppda.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gmtpgbqaz.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gjrplmuny.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/golkrkzvq.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/ginxdquwx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gztujixix.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gamuenpgu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gqckxgbkm.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gutdlyzga.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gebcakvnm.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gwopryzbx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gldlneyst.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gyyxidwia.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gqtemzyyh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/guleehtqo.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gvuodkxnz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/grrqqpctr.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gybfpbxyj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gmylskxwl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gcutfvgli.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gxcvsragi.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzxzkbxrz.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gjwtxnbyn.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggippxgba.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjnzpdgcg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gyapetbht.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gxiwsckpa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/goayueqyx.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gksahmklp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gzmjnyigc.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/grdkeqgti.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/ghjgslcym.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gwdymdgai.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gsiqaemlz.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/ghfpcaddq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gburegujn.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gqchlhfty.sHtML


<!-- 参考信息 -->