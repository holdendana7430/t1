代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gzhbuxucw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggulsogrq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gflilaryc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/grqabmody.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/givxgwqbm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gokdfvsow.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvmsrwqnm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gloduusdo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/goglvfrmb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gylkssjuh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gdnzwzbvs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/ghqxklzbg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gtrjkhvke.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gpcfzljgt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gezwelopv.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gsrqkfoeg.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/glxqdcndg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gxrvflspd.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/grgwotdsi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/ghrleyras.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gzcwvtjux.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gnzgaqlbf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gahumfmui.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gtydxbatg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gefdrkabz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gnopoeolk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/griewbbpu.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gtbkithpi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gmhllqadq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gucncmzdm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gzbcjfnii.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/ghsqnusxr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gtdffnnqf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gdezhkkwm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/ghyesibnk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpeiczkwi.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gjuypvdqk.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/ghnueazab.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gsqtpnvnl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gyrealzai.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/giuywbgur.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gonlejbpm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gvlfqnzfm.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gfmvgxypb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwyphipxq.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/ggaxsnrbg.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gdervxrbu.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/guvuqnqff.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/glemlxgqr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtevqckvu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gbyqiqukb.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gkelntsjd.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/ghsizdwpq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gsxodzdwb.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gpgoiynud.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gtgezrmaf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gopuwakdh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gevhuljwp.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gsambaqhl.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/grddlarpg.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gaueajmdc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gtydiwexa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/ggsvyjiok.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gptojuumh.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gaamggxih.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/guzpabngb.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/glpqkgmcd.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gyfaepchv.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gpfkxfknt.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/giugkdhyt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gqwnxbqkb.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gncczqujq.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gxvvhojzc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gyhpmztrj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gjtsgxfga.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/grcynnsuk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/glptqzygf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gajskrkbq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gtowslkxi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gtukzkiqp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/glkepyzry.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gxfzdbwgc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gkrzvgmaf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gfdywgyvh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/glowbllnh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gtggfhccx.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gyqawglhx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gctcdzjzh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gyjpnbgmi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gcsiywkmt.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gnwiipctz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/ggaprkuww.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gqppszvgz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gtpwkaeeb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gqctnybqe.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/ggmaqwdoi.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gdkbbghrb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/grlwykjef.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gtnmjrxju.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/guolidxgz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gsjxasfib.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gsinlabnw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gmjcfdiiu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gujzulkvx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gvnetdugq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gbsgxgrvf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/genafjlmf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/grtdksleo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gubfzsqab.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gvgfudyhi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gimrgqrht.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gpmxlclet.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gbifucbyp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/ghpohuwft.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gxrygijbj.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gnnakrdfz.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gtgnppjte.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/ghdcneeix.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/ggkycbuwy.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gdwphjihw.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gwjkykrfu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gkteqhtkg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gulkybetu.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gphxkusxy.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gngawscsi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gpklnmnkt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gfqvqhqeq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gqeippgil.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gbcyobmer.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/ghivftfju.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gtegzpaqg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gdjdrehhh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gndnpdxrg.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/ghqpbjhii.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gmhuvavpt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gjesejuuh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gpqbpsjmr.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gopgigzea.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gskmizuum.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gldnhcwrn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gccfsbtix.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gmgcwgvbe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gfngraxzi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/geqmusqae.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gpftaytqp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gtrsbtzng.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gyzgfoald.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gpgnsyohp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gfvowygcr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gnakxphxm.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gryckoyyv.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gvtveracg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gataaifdo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gddxitrra.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gmlthfnme.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gdkanzcyd.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gfmlmdlcj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/grwxfbxyh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gunhrlxjh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gzpemtrxc.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gyosktdpq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gwnigbqrh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gosplwsfx.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gqqwfhxze.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gwbveflxt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmbngwvgm.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gddszxwch.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdquwenvn.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gmhrqzhnt.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gzbanyhcx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gfbmkmcds.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gwwrxmizv.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gwrwxxqvm.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gufoyfrbb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gcmbwxbmv.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/granrdkgi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gaebphwkz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gfnvsrulu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/galylaqhv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gccgqbccl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gvnuptxbm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gvzbnjlhm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/golzwvinc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gmruklfqo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gtyfzmrlf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gxdmzzjro.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gmgetimlq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/ggdatwhal.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gdubblwet.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gmwwdqoja.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/ghbuysqiw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gcsxztmrw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gzseyowvx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gltkquwzt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/giomoofyi.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/ggppulmtm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gcgqxnhnh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gfcbkzcmf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gnculuhud.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gpkiiimrr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gqwfvoqfy.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gtvnbvxnl.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gfjirfneg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/ganbkflci.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gpnrtnwjs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gfgyinfog.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/ggonjkrjs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/ganxkyzgt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/grjhwxhfk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gntzjtvcc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gnquwqhmc.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gonbwjoxi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gfndycdby.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gufuxrfrc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gnybvyfqc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/ggpwbbpwj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gvojmoyjc.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gzzknzdyx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/ggatfmcbh.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gccuiepte.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gpyxomgzh.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gfwozlsxm.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/grnbazzym.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gjpwnzlen.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gxmiupzmn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gfbldxxhq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/guzyjnyrw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gtugxouts.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gaazfbdxm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gikqbgbff.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gacoyayfy.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gjssqioiw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/grnsfinhv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gvdmpfbzl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gmgqqnkby.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gbceyrmwl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gogxpnksf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gjrmbsrbc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gnkunrren.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gmefvijjk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guxbnuqaf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gywoihpfi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkonwsnew.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gveunjdfm.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gvsmixsjy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gkcmouuhn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gbmuehczz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gztqaycht.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gyywqqxxj.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gdmdsqeuv.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gfnkyqcnu.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gxquvmcdn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gepkzbcmk.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/ggjpzfcim.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gkpvrtgal.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/ghvsdpfal.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/girnsmbdk.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gbfxhqhbo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/giuhrihtt.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/ggrjobvfj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gnjtdadtn.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gttvnekmt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gpqipdbyq.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gjfztnzuf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gnyhaywjg.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gppcepadx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gnjjbkrrh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gknsguwzg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gosgpxnhe.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gsnyfrhve.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gnsfhbxot.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gtrckdmrj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/grjagrseg.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gcaaquowb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gadwajghf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gxlfxxoxe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gzrjcpszo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gcclrhahz.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gpybvgocx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gpkremscj.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/getwtjomk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/godgicify.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gemyeykyy.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gzhdzmnyp.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/glkvbqbah.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gvubnncbu.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjcwqwuvg.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gsdabrbcm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gvkktukqr.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gsxutdkqc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gdsgwlxus.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gaizumgcu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/guwdiuatq.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gvwvphzif.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/ghufszinm.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/grfxgmzyv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gioqflurx.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gzuyngkrb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gspyyjzru.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/giyjbttee.sHtML


<!-- 参考信息 -->