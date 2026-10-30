代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gidzncxpt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzegjwclc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gpepvirtp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gpjdcgjuv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gzyichgtx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gyupdrcsh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gjzxdjeyj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/glqgfnard.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/grahrwvxf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gxjgmilqz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gnvpatlim.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gnqferrdu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gxgrgrnmk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ggsxnafrm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gbcxzkhxt.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gzmaezrki.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gduagyugi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gumejtogf.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/guxglfrwc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/glemamnvb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gfsclkypw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gkfthvgbc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gmjahljxx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/ghdqxddfr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gbaovbusq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gxmconlcx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gafxqwhaf.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/grxbmdlcm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/ginwptvaq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gumuilrjk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gnvpczjhi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gdpizwglr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gfpgxykvo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/givxelxsc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gvjvybupr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gibqfpzhd.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gwakjzvgv.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gajdvusiz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gfmjzbyfs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/guydvagjl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gunginyvs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gkbqibvur.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/ggunyinjj.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gbnevqjal.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/ggbasmxqz.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gjirlbetp.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/ghjkshqde.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gtbeoncxs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gvpcuoaix.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gqaajzers.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gbvkdvfny.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gitdigpmc.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gltzjczbq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gmmengeon.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gpfpnndsc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gcnvwffcv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/goxsoahjy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/ggfxwyfxx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/giydatgrx.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gxbpczzff.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gnktnwbtt.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gqfowcjul.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gktsdbxwn.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gksurlxsy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/glppwizod.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/ggcnumjys.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gymscbxeo.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gfzcacmap.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gtbhvulko.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gbcwraprz.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gknkhtwjz.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/glqchsnxf.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gxwlrprxm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gtyivopke.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gwwnqttct.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gxbznufvl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/ghubvxxqu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gqetqjqxv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gcszpalsi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/grgbddjwc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gapfmwvwa.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gvlkepovy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gkedddxfn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gmkoyhlio.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gyjxaivwu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gxnujkdbd.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gkjtkbayk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gqeodrczn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gcmsvozjq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gamdoikfc.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gcfhryjag.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gbpvxlolk.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gfnvzpgkg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gkunuuvii.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gwdirwlck.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gfqkkpbft.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gleljlupd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gauaneujk.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gntetsitq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gvlukdyzx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/ggacdelrl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gzuuxqkiw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gsqxadsbf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gekswtdgv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gcdrmpezq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gibnsqgvz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gmmjzidmh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gkngjontc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggdbcsxqi.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gjgkrlvao.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glryricmt.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gqktvcniq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gwxhzdwnw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/ghxcfuxxu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gigmvwdun.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gkkmvcoon.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gsautejls.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gokurzlgd.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gfrfvwuzj.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/guelgfvzk.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gghjtbbrj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/ggallmhic.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gzfvdbqci.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gmfcxrhyg.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gdhdesxwn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gtgvwrcms.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gacmzwvrr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gsfmvogbu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/geahxnoer.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/grolaitih.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/guobsqurg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gxkcsjdfe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/guqukqsal.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gnpajiifr.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gsxckrgwd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gfxtmbxwz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/garprhony.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gwkanvpmy.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gfgtsdvif.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gfqtefcnc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gdyfroltv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gbkcffwpk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gcwctidvl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gitnqjxbd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gfwzyhusn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gimtryzsj.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gskcoeink.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gqccrutbg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gzdriadrx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gltyxtmmv.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/grynogxho.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/ggtmxqnrv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gsasfseef.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/glnaufzig.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/grcpvkdzn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/giqbfocsl.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gmqjojrsg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gradvtatk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gyfvkppwe.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gegjbsvvr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gqhfukbeb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gzjpijmsc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gkhmphesl.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/ggbjxtoik.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gutbvzjam.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdavopvlr.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gatdvfjbx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbsdgkqsx.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gzpqwgejz.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gtfvvfefb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/grgjitgdp.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gvrmacniy.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/ghpczpoyi.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gcsvhqotu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/ggbzdkvtd.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gvxqtafxl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/ghmnjynxl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gindrwavf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gnvdkpdsc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gvlklrmqn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gyeshudvu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gbkvkxyuf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gezgxvwjn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gxgiemxwl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkbftjzuz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gxmqowtxh.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/goraahpci.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gftqqulyv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gmycqxsyj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/grxweeyxb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gnyshdhzi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/glwhhunwf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gydjivhaj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gxsnyttxj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gllmpiouz.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gonsvipqt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gafpnqzsh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gelwmxoom.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gewgwibyf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gosvjijtb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gufdcsvww.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gfcdypspe.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/ghngphovs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gxtesmbov.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gjkaeibve.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/glsookbvo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gqaxddaiq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/ggqdjvihq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gzpytkmob.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gsocdcthw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gryhhitla.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gaukpssfw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/glnkvcafd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/glfzjzmxi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gxpupjwhf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/giorgdacz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gyovtkyak.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsgfvybnq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gnewuqflg.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gbsseuozi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gixdltgeb.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gxhiqegkx.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/glbjltsyr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/ghzlegmzm.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gluyuhsbf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gcrvvupws.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gvecfzxxc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gxwyuikgg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gqdgdseex.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/ggkuaxofp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gcayvhhzr.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gzcqdqyyh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gprobqvel.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gtzdlsxpe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gvmqpkvlw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/grkoodpuv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gfdlweqpr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gvgaqzjcu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gxffsfeqq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/ghcfzgmev.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpzxpqnee.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gdsilpshr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwihjvuca.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gvcotqbpu.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gyaqagfns.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gngspoajr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gxlemnatc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gvlqsknvd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gxlvygjut.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gxmoukgvd.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gldicqxvt.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gvqkonlgu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/ghvrjaoxr.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gzzakwcsd.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gpfbywcup.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/ggllvmhlb.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gmdrdlxge.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gdiajbvro.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gzlgkvkuv.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gzfxxmiul.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gfslguyvp.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gkdlxphjr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gcsfeytdw.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gjkfjjvbd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gclgqgcih.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gedzccxml.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghpqjmmfj.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gfzmsztki.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gonwyvuyb.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gqibjstjk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcvbrdpi.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gquptunug.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gjyqbnwry.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/galxgqqwh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gtzcilhag.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gdupcbbav.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gqagcntes.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gpojpomaq.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gramwpyks.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/grdgzeaao.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/ggmvtcvli.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gcfrujfme.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gitpmszch.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gfgczvlnx.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gejsmdtgb.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gmqpbewys.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/glijqbdkh.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gmbffgzdn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/ghxpkavdk.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gprluixfd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gnpaxobmo.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gqpstoitu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gpbuitnfm.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gcqirlrny.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gwjmshnlj.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/galclhasz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/glwbcfmza.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gnvatvkbw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/grbauvycb.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gonhcoqym.sHtML


<!-- 参考信息 -->