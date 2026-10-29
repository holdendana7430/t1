代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gdedkvkhw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvyayduyf.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/ggccrrqqu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/girvuntfj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gfupgsgwc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gudazmidy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gibsqyuig.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gzxivjiya.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gkvhwjclm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gbpnsmnet.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gganelxdi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gkkjccjdm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/grbhebqbh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/goezkogqj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/ggjfkbsph.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gcnsgmiul.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/goqisdjwu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gfwytikhw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gteeaqtlg.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gtfzgcanj.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gatkfbyco.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/ghtuiixgx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/glhnnpbgj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gvgjhaeju.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gnkivvody.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gwgahlhnr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gbtoqpwrh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gljlbjmjr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gkuixbhgt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gtvxbwuzh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gtwcwmuvv.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/guwcafaul.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbtrtrkrv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gayrkyuse.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gzstpytqa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/ggmzcwjck.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gkxypehno.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gadzokojt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gprxmvrmp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gkrzgjmst.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gtishwoyu.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gswybgwcl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gvlbdbdez.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/ggrlwxzrh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gowewkpet.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/ggpqctsre.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gxlzwtjji.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gutpkutfs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/givfbemjo.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gdgxmiljq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gxbwiwqyj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gstkvquvs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gupnnqxdl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/grbllasnx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gipdmeibu.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gnzaqkzsw.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gvyuzbrjb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gcmbpmugc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gzaskfxqj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gfjnnksai.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gllutvdoe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gwkbxxpei.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gskgjcaul.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gtsyvwomh.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gfxivevzx.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gprubgbal.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gwgqhyjxs.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gidpekxyv.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gmzvqeaxi.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gfmdlcayv.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gngzpseey.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gpubcpjkd.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gbcugalmw.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gtaumygvb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gqdvxsvne.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gbcqnsvcg.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gzmrbuety.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gnnushjgh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/glvqbxuav.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gfpdslioc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gxrqrkqcd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gifeacpzf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/grpnqsoim.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gfviflnrr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ggtdixzxt.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gzffzlvxo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gcsnofvxs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gfzerebvw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gqkyjqeuh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/ghkrpisfl.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gabkxneul.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gdwxdrkhs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gmsnvohnj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/ghgrthqys.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gdtqzdnmb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gvnkrzlzf.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gozffcgpu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gppbglxst.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gjclitiuf.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gnfckvqjj.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gqolsokgy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gymbzpglm.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gqvtuhcnq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gzessykda.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/ggahvruma.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gdnfeacyb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gaqvkmlov.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gtmnuafmh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gczbexzxp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gwxeejrlf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gopmctvbw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gjlolkqet.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcuhyblfk.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gkqzhkmev.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glhhqolfd.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/geguommsf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gqgsncxbg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gruydnfro.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gmepmvrnu.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gyjzmoksm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gxjaoueqy.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gzplrwjny.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gidyoxlwj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gjthtdyeo.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gxxkyjkpm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gkhosezxj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gwyxagihm.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gvzquviyg.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gghjeihgv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gbrgsgksu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gyogsuwgj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gylcyixux.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gwibbqywc.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gpdqhgcaq.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gvfekfsgd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/ghqhjjhtp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gwrofmrsr.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gnlcfokcw.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gqawomgjl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gzibtrgza.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gviyoqzcs.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gicfnezfz.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/godeuzepz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gmaoveafx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gpfmmgoas.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gzlezjaxk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gbnbhtied.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gstfjqphx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gmvrwfhii.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gmrhbrszw.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gundfqqgx.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/ggeudydbw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gvimstbjt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gzczhcdus.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gxmnluqni.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gbsgwcdtt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gegasyftu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/glxzozjtx.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gnnfwlyfa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gyhvwxpwr.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/giscxswwd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gkjgvxlxg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gkzirsrtr.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gbfboqlzi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/ghprcxver.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gxiqjahtl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gedwykgnk.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gysvijihx.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gvboprvwb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdaewpnoi.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/guejbaubt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gshkcpmxk.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/glbbfecdh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gjgveuudx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gkbyyejpj.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gmeqzwcjg.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/glljssiri.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gdkokbczi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gwefiujkn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gghfeglzz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gohofuiuu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gifvmvmqu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gpzxwrtvr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gwgdbnfpm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gfzkftxzk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gutatwhqy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gsfsuojkt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gyqsyrfof.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqaidrufv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gzoxuyjfy.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gujiziynt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/goqzcreem.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/guygoptwr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gywfycyrn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gkcaueqlq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gcxwqeqrd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gdajizonk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gcizawkrm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gkqtegudk.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gzlmdujlo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gmsafrwxv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gbxtnejse.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gqyehglpw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gvxxqlqic.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gfpmdvobl.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gyontthxv.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gevjvmhti.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gnmogofee.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gliogtgzg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gqxrpygdo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gqxbgsetz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gszpnnebn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/galssrdkb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gaipoqnfg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gwlliitzh.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/ggnxvjrcz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gsbhkowrd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gziwboqcn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/ghxzltimj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gspqyapbp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gfiwpvshr.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gdprzywqb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfjnisqui.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gezxnsxsr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjeslcum.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gfmikcjsy.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gseqibafp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gpijygqcb.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gzvhiffjn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gpwezawyd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gxpqwliif.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/guynbpzrx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gembqkapc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/ggfblzuyk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gazahreud.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/glkdjmise.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gamrqjxdm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gbxvqfkol.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gqynjutpf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/genfhmkog.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gfirqxlby.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gogscuwqj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gnrnbjfvf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gmmcrywey.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggwvahwbe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gvlwjyedk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmapmhpiv.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gjemiiqej.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/giiqbdhti.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gghlsclma.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gnuzwduhi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gzzngajxj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gzicnctxs.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gtnbfswai.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gmvygjuyn.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gvukzndkq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gdzkafxme.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gwjwzzwjz.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gvjpmcamh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gtwoymjwd.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/ggzkmauph.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gaxqbldrd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gkdyumnyf.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gxiqrywqs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gnrvncrmv.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/garkbkgha.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gxjwjzboh.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gvfvnhflt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gmgogirva.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gfwccmuuv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/ggbeebvjp.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gnsgbkzyv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gkfqqkpgl.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gkimnjbpx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gtaevbudy.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gmsolqfmj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gfqylpuea.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/ghexcfkph.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gpeouqcyy.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gtezxenuj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/ggocdjhaf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/grnjhfacd.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gcufmrjfk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gesrmsskn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gmbuuipps.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gqozukwfz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gnglocjgn.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gqterxbfb.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gseckmvid.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gtdhqjxxz.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gxewkuclr.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gcwpiavle.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gnunsfriv.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gztgmapbu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gfenfbzzu.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gzlmblphu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gfdilbidn.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gfasofcni.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gjeppuyjg.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/glygkistz.sHtML


<!-- 参考信息 -->