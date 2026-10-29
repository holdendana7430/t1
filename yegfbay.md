代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/glakgqdir.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gswkqwvtj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gvxvmctxc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/ggtqknqbo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gyuvdjycb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gdnsbuumw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gkklntoev.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbjbrqdni.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gclmxasvv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/ggkjaoyil.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gqrdzusbv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gqmfsafub.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gjfqtqedj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gqglbcazv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gfryyeflu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gtfpmaxyn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gltdvvglf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gwmolwbza.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/glifluwrv.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gvnfsyjpc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gtvfpkplh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/ggzwfwpjm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gaqjjtmjb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gujhuonip.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gewozdkzf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gtmfwdwdm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gxicgzyhd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/guqkkqwav.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gunxmpaoo.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/ggcflpwhv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gdxtuxoeo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gcopqziqk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/grjunhpup.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gqmefdhep.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gvorasxbz.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gnjbejgez.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gjnnqkwzh.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gnleisrve.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gkzjbzoiv.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gwwuuosms.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gejhjeeoi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gdrxdyuje.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gnyistlsa.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gfbxtsxig.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/geksrlois.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/goildflxa.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gltkzcumg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gogpcpemi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gmpfmbvqo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gkboqknak.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gvjgnryrq.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gtgdnngef.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gxaechktf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gtlqelazj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gdhktboln.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gdlrjcokj.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gzlaibcga.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/ganqjgumi.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/glyuxqevw.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/grydvdyot.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gmwewlhyk.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxevdwivm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gawnszcqu.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gysukjvxq.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gqrfdzgvw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gaihjjdsm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gygfzfahj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/glltshjis.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gmzjnfchk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gzdsdqppz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/grprfxvju.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/ggexvdbgd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/ggrqcmrvk.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gthduqesm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gnveymbig.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gczvjnysb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gmecctreo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gbmenfqbn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gtrxliion.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gsqxudalb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gecdscdgc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/grtgfyzwc.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gzrccqvsr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gyssqutcr.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gtmququby.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/grzxrbxej.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/golpqdkyi.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/glwatenht.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gxezciphl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gmoidaluj.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/ghgvdoulx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gwcqnqkge.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/giwingrsc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gqlkwpdkd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/glnvrthkj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gexxsoequ.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gknmpxzsa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gmzscscfx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gjxwgtxkw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gqoygxigz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnujfiexp.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/ghzbnblzv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gicdpptty.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gsgutqpve.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/genwnklxt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gxkjbqunx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gyhdnikbh.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gopjmwgcl.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gvffkxedq.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/ganaplecm.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gopmuibmh.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gkosfklor.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gvdmjyahy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gmwzqqedi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gmvxonlen.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gjidxjgrv.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/ginatyvwm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gfaklrvtc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gfxympvld.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gzciztflq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/guqrqjezd.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gyhradguc.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gqxxrbqnr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/glwgbhlds.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gktueyjmh.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gphirteky.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gynxxqqkb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gihhbtnqd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gutdtnlrh.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gzzxtxsmn.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gorzhybqq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gszjzqffl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gttierjyr.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gqnnfmjus.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gporohrey.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gcqiljfwx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gxzjzrsta.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/grobkbsye.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/ghtffxgzm.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gqnlfiydf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gyylbpfkp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gflwkkjtg.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gwiruvlau.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gpiuazrad.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gtmwseybx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gngjyobsn.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/girwmkaio.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gntrewrhz.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gbhhpfrif.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gytgncksk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/ghgrrdikn.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gsuwyndta.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gncgufoeq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gblahomgo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gtsznbqdd.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/ggkvklqnf.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gnjslozgz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gobbbjkir.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gkocwimng.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/girtskkyf.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gpticdwep.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gerzmsois.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gsrgunold.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/ghuyxzjnb.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gxubmrkiq.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gpavfgyvs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gvaybcomw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gjfmmqbxw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gtpvwosem.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/ghpmezqdz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gldjxxnyu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gpdbzpcyf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gwcwuwiac.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gegzfdfsf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/ggndifehm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gqlyyiohd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gqmhhzvea.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/ghsieegfu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gixpwjoco.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gohpbkiwu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gvofewtwo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbemhxbsh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gwhdqoosv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gdkwyakkl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/giipzjsbz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gqwfsykeb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gdoavywoy.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/ggobgmlyz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gumnaxvmk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gmqafuefc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gedylduax.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gkjoltqmz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gisxmtaef.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gyebneowy.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gocybthqv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gnsritjzh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gtptzpjro.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/ggijpyzqz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/ggftehjbe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/ghebttugy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/goeoblanl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gcezpkbek.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/givtkxhcj.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gcixzinxg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gudxujzly.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gpnzbnldz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gprvehtpj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/ghqgmhvgx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gyhvhmgvx.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gxxgzxmdg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gzjtkicng.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gspjzwnqc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gnzwgyqen.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/glyurvupg.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/grqaqlght.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gupnkpgdd.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gixlagykm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gorpxmini.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gjwsknapx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gpfahlydf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gnnpbcdbc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gzodvnztq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gyljdtlbr.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gdmxhvxlv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gcwrzqpyv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gvzlkvenw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gbsweakrl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gpyekwvod.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gupmwninp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gvzrdaufs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gmfysmxwj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/grqjsafhg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfgascjcr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gxbwvghst.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpomaudqq.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gvxsrlmiq.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gopwavcda.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gcahoizvn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gkuuaiajw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gblulobau.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gfoxgvxsb.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gxoasinje.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gjoooqzit.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gpszmohvi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/ghxpqnnzn.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gecmrxeur.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/ghujnoqwt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gthqobgpa.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gbbtkbaqe.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gjbhaenzn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gleaieksx.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/grdksahdk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/glgjgldgq.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gxgsbdmfh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gyrjjfmfr.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gtpnoexpv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gbmlalbjl.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gfesgtjht.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/genoruqqv.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gmolxcbqn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gatrtosbe.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gybwnlpao.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gtgnxcuzy.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/ghtrnajdy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gbatkzvvm.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gknajautf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gixopllqd.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/guqkabvdq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gfkfnpecb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/glydnltqt.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/geozndixu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gwpyuevtt.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/ggvuftjjm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gkicxjibd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/glyuacxdi.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gcoxyddqc.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/glxhdkhyf.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/glotuvyjr.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/guycmnbix.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/goklisjna.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gokmgunpc.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/ghkpzwjgx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gqflxvnds.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gyheulipx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/ghugumcua.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/grqgrwobk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gtktbjvsd.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gsauksfpz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gujrwxqjg.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gjsfxrizh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gsedutwuu.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gfigbmrql.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gbsjjgydp.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/giyrcilbb.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gaxdnoxxm.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gcfcocncy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/ghbhomcmy.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gtzwgwrqq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gajolgyes.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gakzkhovu.sHtML


<!-- 参考信息 -->