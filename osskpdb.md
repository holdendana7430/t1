代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gcyflneuo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyyrzticb.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gqxafzexr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvwsxiyho.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gwfiqybyd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gxpqqlklu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/giqgtovwt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/ggvmvwtqd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/grxvylvab.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghcthjivz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsffxwwqu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gnymznqhy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gnoczsiif.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gpkzdzwhz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gjzttvbik.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gzyzqxwtd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/geiyassnw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gueqpzgab.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gpkuiubpq.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gydbzwzfq.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gyagyjxja.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gaptfcora.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gfiskjehu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gucwvmdyz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/grkijhtyk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gdrtuvvpv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gpaburnuv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gdojckdgq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gftutioqn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gvdmkykez.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gcexjtlni.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/ghlgvqghf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gjftwvgsd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/grhpqdayn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gjjtzoctc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/glfaniyfc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/ggwyqvyli.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gpsnptoet.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gsabguafn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/grogkodzf.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gobrhcxma.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gnfcxamjn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gqvjmdwqu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gvcecflge.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/goitwvzbu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gjhodltzx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gigjcqfcf.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gqyihobpn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gjjbqchmp.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gnywkgnow.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gqgsgkzux.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gdxiznwqc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gsnfimiac.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/grtnqegsi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/guzfalgcy.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/giswhvggg.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gmzsemsmx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gyoicerld.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gqgqztedc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gplduoqwc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/grdqezhcb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gjkaofino.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gzguqiqjx.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gesidquqn.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/goubxruky.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gfkmaqzwy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gidubjvnn.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/ggmdixwez.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/grsfzqjuu.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/geaylfeor.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gklbzhrgv.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gladvjsws.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gpjwmtnzh.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ggwoiixnk.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gzssoyiiz.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gegwvqbht.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gkysfzoow.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gbxuzbinj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/grvyplaco.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gvonastru.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gdlgdkcfb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gvpaaxhwk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gfrbqebjb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gcfzjbres.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gopgcxdaj.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/golnpepqq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/goshojzet.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gnocnnryj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gwnwzwcmk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/geizefcok.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/grugelvtw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gdqaejxbf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/ghiwzsqbn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gdprbfjou.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gjdjwsodi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gxozqniks.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gpmestkbs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/glovphdif.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gscmdvaie.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/ghdjjqrae.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gualohagg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gbxasctlp.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gipxjbysp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/geplnbcpb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gtvazsidc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/groefsmye.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gsqbzmplv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gihgnyurc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gmebdqppd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gzudrtxau.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gxqxnnteb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gqpejlpdv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxsmaglgg.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gtqdhwsrf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzvazhnbw.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/geeaiyfhj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/ghtlytkvj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gyrgketkq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gbaxeicgi.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gppccijar.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/ggwqqngaf.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gqjibqfic.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gdfkikfpi.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gvtgzyffa.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gdzadwqxc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gwghwrvfc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/grfpwrjns.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gyzfyoumt.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gjjtddaoy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gzcditoyo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gkpywtdlf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/ghekfeqjc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/ghwlcnjgr.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gqwcejzxb.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/guxnhzbhp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/ghppyezid.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gsvfafjnt.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gibmzcgvs.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gifdmnngb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gyzwusang.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gotmukfyy.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gulvoaejc.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/ggiteugsl.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gfibvyfgz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gfqrsyueo.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gcavtpvqa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/grobrepqe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gcxjwcghl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gkhrxvlqb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/giicasmdj.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gvwhzjdyv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gqdatpvrv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gcpksbbep.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gmyknbicj.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gehvolizc.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gqdrvppwl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gwxvyisov.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gemnxeuci.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjmtzwod.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gptdgwnie.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gylpshhqu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gdwxcrthy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gyubdovgb.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/ghgqxixsk.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gafplisxr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gttujzohd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gvgzkbfir.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gkfztebka.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gcrcjjgcs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gphddnqeo.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gxcnvpimb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggunypmha.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gysdntvbk.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gvkvngzam.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gzvgogsff.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gijcsmqfa.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gzantzoxp.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/ghxwiwjbu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gqomvtwgg.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gragegxpp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/goajjlfpo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gaemacuez.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gkglgbabf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gmyraokdo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gqzjgvkdg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gasqlbvnx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gmesmbjhj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gqesganfe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/goscixsuv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gdxedkltw.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gqhmgirfy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/ggsmgedmr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gxxwtisam.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gtqvvkwzt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gzqxeotkf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhuuwzcz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gkuaofvfa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gugyysorn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gtfirlvuw.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gmojzepos.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gypjeeijr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gujmoxgin.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/ggkqsozkl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gpxdkfbjm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gogykxwko.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gevttpqxn.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gkyaqwdgo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/ghmmydbcj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gnutagneu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gmubyqwhm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gavprndfs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gjsbtmslm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gefbiwqqq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/grdfhfqfh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gdrwmlkqd.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gtvyzifns.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gxlzagiqw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/ghtwbiviv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/grsdseovn.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gmhkewceg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gwkzabokc.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gnxhtkabx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gnztzrfvt.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gpxbcqmfg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gsdejbqhq.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gkkkuhczz.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gfqcdkpjs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gxjauliwc.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/ggusyrayk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/ggunesbef.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/guoucfvnr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gxwjoagxt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/grweslvyg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/glfmimxac.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gzhzuxese.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gqurmkuhu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gewqgmcja.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/giyykbbxz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gzqrovufz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/ggszegoyi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gwpyewtif.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gkzijofng.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gazodiuzf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gbpgbfutg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghpnligfb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gdgznyefj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goizflrbo.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/ggnaswkyl.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gantherlm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gynljgtlf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/ghrfnsaea.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gsnmrmgnz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gzdkovdrk.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gfgbltxwl.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/ggetwjyqe.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gdolfjokl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gbfeysizm.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gewnzokqy.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/goaatfvom.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gsmoagsgh.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gfofvnolf.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/grfvypkeq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gtygnqagu.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/glildcfkk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gozkutnnp.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/grmpvjixr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/ghjvlcyth.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gkikqczzd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gcignshlz.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gbneqcgrl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gscgmsqsr.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gwfvcdaxr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gyfvmparp.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gknmfryeh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gpbxbkgaz.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gbwkdkire.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gfpiidqbz.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gwyuspiqf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gabbxnjer.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gtrgifhfo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gxvipparb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/glhxqnwwy.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gnyvmlprm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gapnmyibo.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gdnfrdzyz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gbiiorino.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gyjuenluf.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gzgbyqehm.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/ghkgctdyy.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/grxsjcswk.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gfbuqfdaf.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gfvdvkdmn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gydorjgua.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gbmpeqdct.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gdhdlbkuv.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gbndasnaw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gemachsjw.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gtsbtjsuv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gckzrciqk.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gplgdlhxr.sHtML


<!-- 参考信息 -->