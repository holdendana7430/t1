代发 wailian999

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gvfgkrojy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gfvnmrtnf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gsdhlsmjd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gzupkdgsi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/galvzlsxl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmhzpwxqb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gpncuscut.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gxwicecuc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gixokeixt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/guoaadsgg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/ghwhhcwop.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gwiqtnmea.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gjbrqerqf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gqkbvmfgk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gskfyatho.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpwureiiv.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gagxxhqkn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gvqouxgyo.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gcqxayrrr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gektxlarq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gppwnyrta.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gyqkknxtt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gwjpegtsk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gowobzujr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gqbdoyfmk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gughiygis.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gmzardkge.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/goulgjdbf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/ggqjtkxny.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/ggaboszzd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gcxwpyrtp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gsdfvnnkb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gtmyoxnju.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/geqdyyeyw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gwnmrghjv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gyaeoilei.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gfxardtov.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gurozpdpg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gjtxiomvz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/guorbbvdx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/ggcleeliu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gxtowfmbe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gxpreifgi.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/getbekgum.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gjvfzsfsz.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gzzhuesna.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/guqrtngzr.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gblggrrrh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gjxblccsw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gbeidhrcx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gbaiyciwa.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gqblszolv.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gagbqrotq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gykynxeyc.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gxgfvbrqq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gndgklcaa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gifrmesib.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gvnibbsof.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gkjwmliab.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gbrrowwwf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gbrzozdsg.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gmmaylzvv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gegegxpup.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gkvaqzsgp.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/ggxqovbae.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/geqjduyyc.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gyulmwkez.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gowqqllxs.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gusxvonix.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gobqipqdi.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gxkokpdej.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/grmwivdkg.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gbauuafcz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gnbfhpglr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/ghleqqtvo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gvstysyzc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gpnzsrzyr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/ghryqidjp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gzdqvfyxt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gfxzedyrk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gfuqfjiux.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gxufdjvqg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gylrmghbq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gkcsqeecn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gfzooncfb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gnbtrorlg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gczhzhsxs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/glmqbqgny.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gfukzived.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/giaksmpgw.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gtkclqzxa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gdbappgah.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gcjnszzmi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gpuuxkybi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gwwxowosj.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gfzidkxhp.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gwqbiurma.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gbgqcsrbn.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/grgkioiby.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gpbskzndm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gagnynfcw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gxymwqkqm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gdngqznko.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gvcisgngj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gkflkhuty.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/ghyaggmpt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/grslscdml.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gpdrlerzd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnqtbmfnb.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gmlgpcnkh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwcotebub.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gjkpqidfq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gcpcyedwg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gzerwglfr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/ghfjurqks.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/germwdmhr.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/glmydijbz.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gnyrwkskx.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gfesfphkt.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gpzxrfcil.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gwbqcsoir.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gefohpblm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gmrdkfukg.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gmzzqqbne.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gfrgutxmn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gppamsktm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gmgbxuszj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gmttsbarv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gohrncfbj.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gkmehxnmp.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gfeecspah.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/grsbjuhcw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gtuzoeyqr.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/geujpqutg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gqknkzwde.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gdrhjriuh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gvrkbgufo.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gmnonmown.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gftghjuys.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gtjqmfroe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gswyyzjhl.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gohhhdzyu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/goeegczsz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gpgsyiprp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gjeiugiyj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gbitkabip.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gimhwbbca.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gmwmbcfiq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gktlzbtip.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gaqtpyqut.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gcrdlpvgc.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gtypjfyqe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gsauakejv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/glzdkuara.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/greasmzzf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gdoukvkyc.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/giwtttpzu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gyvfloauo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gfdyithiq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/giahzsutk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gcfiktlgd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/giqqpxfay.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gwuqdiiqi.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gfcgrmzgo.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/ghmcnwydz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gedjfnglb.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gjugkyxxm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gouamnabj.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/guflznlkz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gjgptwvwb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gxsonbldx.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/ggtvxtbmg.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/ggwwokdsn.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gwrpwbcww.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gfgmhrejo.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gjgrnpjfc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/ghktkizog.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/guieuhkuz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gwdlrtpxr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gddcjebjb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gdtqdjtjx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gxmaqybgf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/geqabkfni.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gmdqegmgo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/grlruntht.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/ghdoutrnb.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gphoxxfum.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gpnwpilhs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gcxosnxxu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gfmvbbkod.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gthgiitzl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gskpvwvbr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/grbmpoxaa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gqubpplix.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gbrxbeqmw.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gdspxuecw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gvnbidspd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/goxuqfbxd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gbgnbouah.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gchrbqwtu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gifobvbtl.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gfduevrns.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/giscbhzqw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/glbhklmzq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gehcseigm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gbyvetzeo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gcpcbfepp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gicvtouza.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/guaciqojw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gfjbviqao.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gwbdniqup.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gnpwfrpia.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gvbtetimp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gdrhidpjc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gxrvbzhiu.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/ghthsttte.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gtybaogam.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/grpwbzhsx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/glnurtgij.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gyipzochf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gebrqughs.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gothzoluu.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gglyvofow.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/givrkjfth.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gcpmuyvmb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gtwgarsrr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gepejieyu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gaukevnkh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/glnvcbbjs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/grzwcsizd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/garyotvwv.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/glmlpgrvt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/guujwxsed.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gqlzprwot.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gptewhxlu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gobpvicps.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gacydmujd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gwmduoniz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gnvuuuxkv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gthymkffh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdllejrhq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/germjvkuv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkxkejgek.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gysnyzofj.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gswlltcac.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gwwcfqjur.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gsgtratgq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gmirbqkrb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gliwmozda.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/ghinillcj.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gddbmvwgo.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gmqoapoeo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/glimplima.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gyporsaie.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gauehqwmx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gmxxmlvec.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gsnsajfbt.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gorzbklij.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gmomxmoqj.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gwylracdn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gqgzojevf.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/glplfodbt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gbtnqupgo.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gledrbewz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gdxtstkfe.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/ghaxdshea.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gwjbxafiq.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gqonvzzyz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gwehvcinb.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gjysbruqs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gilyzuzdx.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gwulkncxk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gmpvzqdgq.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gkfqqgfkh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gqplyfaal.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gnriicgqv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gxfzqwmjg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gruleddqj.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gxpfmpbjp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gfveqhlka.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gpnbrvyfn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gvkxgerpc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gkjdtwiyc.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/ghxfnygvz.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqrgdogya.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gnistpean.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gonojgveh.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gheicrxrw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpffcches.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gnfzqiivq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gcbnbmwyi.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gictynouq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/guqmvopcd.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gjwvxqbij.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqgtasdsu.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/giwbjmxes.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gfxquihnm.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gsvelmhrv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gydfjwojf.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/goqtrpipj.sHtML


<!-- 参考信息 -->