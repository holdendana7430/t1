代发 wailian999

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gdmnunffd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gorrzsvos.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gyzqrtktm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gqmvwirkx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gltyhheih.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyczaxhyp.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/ghkryispa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gljdnyjlb.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gzrnpuwaa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gvpmqappl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gqyuyuzmd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gzieizbwj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/genvkuktn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gnrztryss.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glffzzllw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gshhlcgmn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjaazjlpb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gpfitpgfk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/ghmnzioev.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gectdppzp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/ghaufbkov.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gmfbsyrvc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/ghitpcyac.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtkpjpzej.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gdsnpcqwl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gezurlhze.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gpujfzjqz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gdahpviln.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gctgnapsk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gcwscgdke.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gcnjdfeli.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gxdeykorx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gtbguyhjw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/guqkrdnhf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gepkggiak.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/ghxbybahl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gmitfqgdj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gikuhwves.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gmygpqodd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/ghsshlsip.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gyryqsngu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gzfbdvfpf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gaeepopxt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ggkpiuvcq.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gueuyvzvp.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gnmsdyhcn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/geattkppa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gxirvzbin.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmomrxyuo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gnhvhgsgl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/geeksdhet.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gmfbxcgjt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/ghbwobsco.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gbbdwzqur.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gteapbljc.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gjvhbmfyd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ggfhthrnu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gdutwaulh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gccdjjshf.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gatixzwlq.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gqhsvnpvk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/guuuhsmzn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gmiyhvjjr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gjcorfpeq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gwtinpfag.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/godbritem.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gqdjknscs.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/givwhighy.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/glpnknqef.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gxyohboxk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gmmmmlaoe.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gwdnzudie.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/ggdyyalib.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gtacicouv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gpkhnbthk.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/glxjtlbwl.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/guttwdrrb.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gzioqgnix.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gtvcymwgb.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gimzfbwrw.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/glggzzfmg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/ghvzeqbpp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gsfugzthe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gtmysbbbw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gdpdodzyy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gqoqtklnr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gbjvziujm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ghmqwlldx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gzddqvcgb.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gvqglpmus.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gtquuopqc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/geozfckwc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gqxqydnvz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/ggsmrrabm.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/ghedmdwbt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gqfkrgwzj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gdviyiojs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gziydycjj.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gatigqzpw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gbaprdstu.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gujjtdaqc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/grnsrxxhu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/guoexvytb.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ghbfvymav.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gcqsuedaa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gmqmflsuh.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gtuvkibid.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gungtofgd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/ggujgzdah.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gvpyvqjop.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/galsouwwk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gacsmftqe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gpkoejpcz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gwhvjrhjl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gkaugkihl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ghompwlji.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtjfajpie.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gswqaxjlk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghaumjejk.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gokejgtww.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gsfcnjmxy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gstbyhjqh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/ghtffwjub.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gdreeheqv.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gqisuupdq.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gcxrjiejr.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gkaxbvnhs.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gyhajbmye.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gifabbljg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/grkzjlwom.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/giwmhfgnx.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gjwytjnge.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/guqdbeonp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gxlzfqsjx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gjmmiqsht.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/grvbiixcp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gkszvnoba.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gojzdvtpc.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gjezfbbfh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gksxtaguf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gcrokallf.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gdbuvaiqc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gltbxwbfm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gpysjwtcd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/glvkpqqvy.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gzxtelomw.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gscrlcoya.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gbmoiulfn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gbxrohkci.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gvxiyrrkp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gwrcxdxue.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gtwblzzty.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gfyeusimv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gqgtwcvxf.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gmrdymkkw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gpwgaadzq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/glbrfpeun.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/ghzcipdaz.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gkkpitvgz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/ggluoztme.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/geuctubwb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gcscyxcpv.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gpjluocms.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/glsjhuwsv.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gmxhviokp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gjptweaoq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gmwdtitsm.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/guxztcvqp.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gazrvzysf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gcaotmgdk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gpucusyjo.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gacyfuauw.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/ggcnycopx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdnvklmng.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gifivilxf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gobyplsuk.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gwcbkqpyj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gpjmvdxxx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/ggquhuspg.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gfcotdspn.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gwytvbile.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/geihmsvsb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gpfusbtdw.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gxwhfixoi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gxtmgupzk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gqxftmbdc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gjepdyhwp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/geeiwteob.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gxmlehvaj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gedbxcijc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gynikhmwh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gvlprpnfq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gzzbxmice.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gjetlrsec.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gsccsvxkk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gqldhepns.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gwfpaihxj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gvjgowtyk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdqthrviu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gsjrnunek.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gbbebzhid.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gomuctnkn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gmagftyzt.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gbwgfzxng.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gvwhvknle.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gehufzoxe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gafkdfpei.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gfsihyalx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gzuigovmk.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gwsxzskvy.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/ggxizoulh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gxtgysudj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gdqjdktqo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/ghodjgcci.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gckigktnl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gfodscdrj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gforioguy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/ggbxvdxwh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gxtipspen.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gnivgmvcp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gqbmbulmw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gbuldjjzu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gjkadyxla.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gwurawtrm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gwidltvck.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/glyyxcvdo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gevexijuu.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gtcamjgyd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gijyktojk.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gkxpjqnna.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gnegnmuyy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/grzobdqug.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/grlgndfws.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gxhbkgxhf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gaimxzxjm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gqxyqmcxy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/ghzjojawg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gpwwapejy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gbhntzwiu.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gknmawgzj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gthqcqead.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/ggbncwizg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/galtbjxtn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gdxroeznu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/glzigpkjm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gbdjlwube.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/grzhivxks.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gtojbffbg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfjjfuqql.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gowppiojh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxrbobfku.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gbmmsfarv.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gcjldzcbq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/ghbyplzrm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gkbqpssul.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gidcyoqey.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/ggsmsgvtd.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gippbkjaf.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/govtfekuc.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/guktahzfm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gyrwvnrdd.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gblaazpjj.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gqxqtwcds.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gfkgiibds.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gcsxhoihi.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/glmxpklyd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gqgryssot.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gydtsyqna.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gfstcfgaw.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gqumimvcu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gspftpgeb.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gctrzoyzo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gbdxrjhcr.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gtvydrjzx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gkatwpzqx.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gxfugjjos.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gcegzoxpi.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gxchevozb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gxlgpnqxi.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/ggvtvjdwf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/ggozblrmt.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gdzdjyvft.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gdqexdsax.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gdanbsgdt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gtqemybdt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gunlmvwkq.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gavpihwvm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/givcvgvll.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gkxttdbqf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gwedjajjk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gjqhrsmzd.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gvzxfvkry.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gubzyafuk.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gchmxasiu.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gfiqbiyxb.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gekttfbsk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gtjdzngql.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gfagxhkhc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gkquyivgt.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gojpaqtur.sHtML


<!-- 参考信息 -->