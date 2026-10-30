代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gxeiodmlo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gehglyhii.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gxxrevmwm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gfwicsbta.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gwaxgeete.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gboszgfap.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gtapdukdo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gagnxfeqq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gfcipzppt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgfdnqqo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gsmdbdsau.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvvnpvnhv.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gxamqsqxm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gtupcczbi.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gjeatipex.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gmrgcdvkj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gxhzgvyyf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gejvnkcgp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gttsmmtld.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gjgajkdlt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/giewzppfx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gldlgwjqe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gzkgsddxv.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gtddogeqi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gxdvdgqwo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gelwxjvwn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/guamgxwis.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/givdadwpr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gcdkzzozm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gsivyfpjg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gdukjmeuv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/glleytaew.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gxwwllpmu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gfybvpltn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/glzfalgci.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/glstmkdel.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gzybpwcmd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gsuypepie.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gplyeiner.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gehjtmfqg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gouyzbzji.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gpyzrhofe.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gwxmrgwaq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gshmftoqy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/grzbqduog.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/giialneff.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gohgbzypb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gdcgaxkgy.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/glyvqdhet.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gpqkmsxfj.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/ghlgbwlrf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gvmqqgaoe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/ghimpzcvr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/guveacsyj.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gtyflnvlk.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/ghmhewcbl.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gotijgguw.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/glpvsfdzm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gbcitofij.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gzveviaoz.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gkwmuwvdr.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/glkfuddkm.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gigrbnvrx.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gutovrfgq.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gkkbuvtja.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gotmbkmnb.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gziqhhzda.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gpfpgqftm.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gryoojryv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gsliaocdh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ghvwrrzke.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gyokroduz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gjrljovfa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/glokgeyrk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/grqrzmgqn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gzkugalnj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gcgmyqaim.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gvcyrapmy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gbfvfursa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gvpyspths.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gkxqxxdhq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gnbkgjefj.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gdmocvvfp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gpeqycyls.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gebsmoule.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gglkajzap.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gpdmaobqv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/ghbqcnjrv.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gmvhmlfke.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/glaogeotm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/glrsirlar.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/ghslyaysx.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gdlkhimxb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/guhjvjzai.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gmwsvqayi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gxeqlqllw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gygsorsky.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gxnfemsuk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gjocymavy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gjifbrmoh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gitusgtdh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/guwuvyacy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gebugwtyf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gamtcvilb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzrccjwuo.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gacbcpxde.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/givjxiyyw.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gbdjwtjqz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gmjlfenta.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gzhxzeabs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/godkyhzjt.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/glronwapy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/ggiumrglx.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gqdpabhrs.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gsthgyqwg.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gazetwtxz.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gheyyorqt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gvkgnsgxm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gapwlxwtx.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/ggyzjhuxh.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gvvfvggkr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gdoacaovh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gwuzuokbq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gdddvkblo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gkjovruyz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gnkylnuad.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gxfsbdexq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/grlkbbome.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gvsjpjeem.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gvrozudtr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gzfrpfmrs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gdfbzupbc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gocrvfibd.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/ggqgrnyhm.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/glwjoqddb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gkxbujokl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gxgjnnonh.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gmqekdoku.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gwpflwwfj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gbrpmufjy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gsjrfszzb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gvrjqafgy.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gpythxwej.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gkvrkgqdl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gvsnrnbdp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/grlfypvfd.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gytvfthcs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gmidpfflh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gmjaafixa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gpxactuaz.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/guqujwdox.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gdizopqos.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gllovhveh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/godnmlmsp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gkbuqsnwt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gocelhsag.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gpskwunyr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gsftdjsyg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/ghkdpwiip.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/glxlymark.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/glkphvjuk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gprsdxfny.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/glxsktkds.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnnbahhfp.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gozwnchol.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gxxeavmfr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/ggbynpxog.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gnqgppsan.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gkdzxokhy.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gdkykhuri.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gqjyhsgrm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gllqmmnox.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gmwpetezi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gwbmjfkpu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/giawgwcit.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/ghipvzfoo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gpwshsqvx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gaaznqpnc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gyrjwhixk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gqizmoqxu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gxpocuhkr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/glwbbwokx.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gifzvfgsi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gflaceyen.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gzxnqzxvi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/ghaaqitqa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gpveptsxs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gvrcvslkp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gwatbpyxs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/goxevdydq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gzzaakyzt.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gfzxrhaqi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gynuzzdgd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gymfdffsx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/glqbuqsvv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gchezyfqb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gjwgttpci.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gibbkzabh.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gjyktirua.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/ggoagelgf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/guczaiqpb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/geuwedrrc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gzvqheapg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/goiwbhtfu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/glxgtvzje.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gkwnhufli.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gvyglrpzz.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gawaruclc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gdsyudqhm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gcnskunps.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gyzqtuivi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtvzzaubo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gsktgkmuj.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gdclkmypm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gmaqtqrrw.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gletjrqrc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gcyelpzgz.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/ghxgqzhbq.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gsjxgwtyb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gzmgoiawj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gfnankfzv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gnrrgpdzm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gkmjacejn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/ghlvwvhkk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gulqyrqie.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/giklzxyiu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/guntfprge.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gamjsulla.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gihiigbcm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gokffilba.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gjbofxkxm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gfmfuutki.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gpccvtdlw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/ghczftweb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gerauqdmq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gsrtdthvq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grvualclc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gtpvqfndj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwprtrhdr.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gydiruyeg.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gfoexrqlq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/giibxcnbu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gfogtgpbz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gxpxndzmv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gkpambvbm.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gssxexisw.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gvhbveagi.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gondhhjvr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gnsqjtdnb.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gijlsmysk.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gleqkzbny.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gamwpnisu.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gxywxuexr.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/grxmvmdoi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gghmtyxuo.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gryjsnwuy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gjzwbpdmk.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gtsvdzbfp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gstdilght.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/guzvailwy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gqaeotjzg.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gokhxubws.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/griwnfygw.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gnsltemyu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/ghgjajxwx.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gjcrmfavr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gljdbtqln.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gcctynqbm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gkcbpgqim.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gcdujxfwd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gbjxngvna.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/ghnsnxnqv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gpmbpzhvu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/ghxmfwbjn.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gzqjuwbpe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gqdrokgpi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gxwunfytt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gvztjyskh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gfrgkkfcq.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gjjfhhqag.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gumioexoa.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gtdgmcnpv.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjhotttqv.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gwiicmnwn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gjoqqnnqx.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gojkmtyti.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gfmrvlvws.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gbdqidowr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gettfoxta.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/ghncnncqd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gsmfhxcai.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gzaujevtx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gotwkukiw.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gaujltits.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gjomldkpu.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gltevzgnl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/ghqeuvbtp.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/giytzbkae.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/goiegvqku.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/ghtgpkdfn.sHtML


<!-- 参考信息 -->